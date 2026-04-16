---
name: brain-update
description: Sintetizza i dati di una campagna appena conclusa in learnings strutturati e aggiorna knowledge/. Il cuore del sistema di memoria accumulativa. Eseguire dopo ogni campagna (ogni 2-4 settimane). Trigger: "brain update", "aggiorna i learnings", "analizza i risultati della campagna", "update del brain".
license: MIT
metadata:
  author: GTM Collective
  version: 1.0.0
---

## Overview

Dopo ogni campagna, questa skill trasforma i dati grezzi in pattern strutturati nel sistema `knowledge/`. È il motore che fa migliorare il sistema nel tempo — ogni campagna insegna qualcosa che viene cristallizzato e usato nelle successive.

Leggi `knowledge/INDEX.md` prima di iniziare per capire lo stato attuale dei pattern.

---

## Instructions

### Step 1 — Raccolta dati campagna

Chiedi (o estrai da `outbound/campaigns/`):

1. **Quale campagna analizziamo?** (segmento, segnale usato, periodo)
2. **Metriche principali:**
   - N° contatti raggiunti
   - Open rate (email) o Acceptance rate (LinkedIn)
   - Reply rate totale
   - Reply positivi (interesse)
   - Meeting booked
3. **Qualitative:**
   - Quali risposte negative hai ricevuto più spesso? (testo obiezione)
   - C'erano risposte che indicavano interesse ma non timing? (nurture)
   - Il segnale usato come trigger ha risuonato? Come lo sai?
   - L'ICP era giusto? Hai contattato aziende che in retrospettiva non erano adatte?
4. **Deal update** (se applicabile): nuovi deal chiusi o persi da questa campagna?

### Step 2 — Analisi pattern segnali

Per ogni segnale usato nella campagna:

**Se il reply rate è > baseline del 50%** (es. baseline 3%, campagna 5%+):
- Confronta con `knowledge/signals/hypotheses.md`
- È già in test? Aggiorna il contatore (N/3 prove)
- Se è la 3a conferma → promuovi a `knowledge/signals/confirmed.md`
- Se è nuovo → aggiungi come nuova ipotesi in `knowledge/signals/hypotheses.md`

**Se il reply rate è < baseline**:
- Il segnale è debole o il copy era sbagliato? (distingui le cause)
- Se 2+ campagne con lo stesso risultato → valuta se spostare in `knowledge/signals/graveyard.md`

### Step 3 — Analisi pattern copy/sequenze

Per gli angoli di messaggio usati:

**Angolo che ha funzionato** (reply positivi che menzionano un elemento specifico):
- Aggiungi o aggiorna in `knowledge/sequences/hypotheses.md` o `confirmed.md`
- Nota: settore, persona, segnale — il pattern è specifico al contesto

**Angolo che non ha funzionato**:
- Aggiorna `knowledge/sequences/hypotheses.md` con il contatore negativo
- Dopo 2+ fallimenti → valuta `graveyard.md`

### Step 4 — Aggiorna ICP

Basandosi su chi ha risposto (positivamente) e chi ha risposto (negativamente o non ha risposto):

- Il profilo delle risposte positive corrisponde all'ICP definito?
- C'erano aziende fuori ICP che hanno risposto bene? (nuovo segmento da esplorare)
- C'erano aziende nell'ICP che non hanno risposto? (raffinare i criteri)

→ Aggiorna `knowledge/icp/hypotheses.md` o `confirmed.md` di conseguenza

### Step 5 — Aggiorna obiezioni

Dalle risposte negative ricevute:
- C'era una nuova obiezione non ancora documentata? → aggiungi a `knowledge/objections/patterns.md`
- Un'obiezione già presente ha ricevuto risposta efficace? → aggiorna con la risposta che ha funzionato

### Step 6 — Aggiorna knowledge/INDEX.md

Aggiorna la tabella con i nuovi contatori di pattern per ogni dominio.

### Step 7 — Controlla promozioni

Per ogni dominio (`signals/`, `sequences/`, `icp/`):
- Ci sono ipotesi con 3+ conferme? → Promuovi a `confirmed.md`
- Ci sono regole in `confirmed.md` contraddette dai nuovi dati? → Retrocedi a `hypotheses.md`

### Step 8 — Aggiorna CLAUDE.md

Se ci sono pattern confermati nuovi o importanti → aggiorna la sezione "Regole apprese" in `CLAUDE.md` con una sintesi in 1-2 righe.

### Step 9 — Output summary

Produci un sommario del brain update:
```
## Brain Update — [DATA]
Campagna analizzata: [nome]

**Segnali:**
- Confermati: [lista]
- In test: [lista con contatore]
- Spostati in graveyard: [lista]

**Sequenze:**
- Copy angle confermati: [lista]
- Testati: [lista]

**ICP:**
- Criteri confermati: [lista]
- Da rivedere: [lista]

**Obiezioni nuove:** [lista]
**Promozioni a confirmed:** [lista]
**CLAUDE.md aggiornato:** [sì/no + cosa]
```

---

## Troubleshooting

**Dati insufficienti** (campagna troppo piccola, <20 contatti): nota "campagna troppo piccola per pattern significativi" e aggiorna solo le note qualitative.
**Risultati contraddittori** (stesso segnale funziona in un settore e non in un altro): segmenta il pattern — non è una regola globale ma specifica al contesto. Nota il contesto nella descrizione.
