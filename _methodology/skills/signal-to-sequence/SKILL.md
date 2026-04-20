---
name: signal-to-sequence
description: Trasforma un segnale rilevato in una campagna outbound completa con copy calibrato. Input: segnale + account (o lista) + persona. Output: sequenza email e/o LinkedIn pronta per il lancio. Trigger: "crea una campagna per [segnale]", "signal to sequence per", "costruisci la sequenza per [azienda] che ha appena [evento]".
license: MIT
metadata:
  author: GTM Collective (adattato da KarlRaf/gtm-starter-kit)
  version: 1.0.0
---

## Overview

Converte un segnale di acquisto in una sequenza outbound calibrata. Leggi `clients/[nome]/context/positioning.md`, `_methodology/signals/signal-library.md`, e il message house in `clients/[nome]/outbound/sequences/message-house.md` prima di costruire.

---

## Instructions

### Step 1 — Input

Raccogli:
1. Quale segnale è stato rilevato? (codice da signal-library.md)
2. Su quale account / lista di account?
3. Quale persona target? (ruolo)
4. Canale: email, LinkedIn, o entrambi?

### Step 2 — Valida il segnale

- Controlla il decay: è ancora rilevante? (0-90 giorni = sì; 90-180 = parziale; 180+ = scaduto)
- Ci sono segnali combinati? (scala il tier se sì)
- L'account è nel ICP? (consulta `clients/[nome]/context/icp-definition.md`)

### Step 3 — Seleziona l'angolo dal message house

Da `clients/[nome]/outbound/sequences/message-house.md`:
- Quale value pillar è più rilevante per QUESTO segnale specifico?
- Qual è il problema che il segnale implica per questa persona?
- Qual è il proof point più pertinente?

### Step 4 — Costruisci la sequenza

**Sequenza email standard (4 touch)**:

```
EMAIL 1 — Aggancio al segnale (invia subito)
Oggetto: [specifico al segnale — non generico]
Corpo: 
- Riga 1: aggancio diretto al segnale ("Ho visto che avete appena [evento]")
- Riga 2-3: problema che quel segnale tipicamente implica
- Riga 4: proposta di valore in 1 frase
- CTA: domanda leggera, non "prenota una call"
Max 5 righe totali.

EMAIL 2 — Differentiated value (+3 giorni)
Oggetto: [diverso dall'email 1]
Corpo: come risolviamo il problema che implica il loro segnale
Max 4 righe.

EMAIL 3 — Proof point (+5 giorni)
Oggetto: [specifico al settore se possibile]
Corpo: caso d'uso o risultato pertinente (anche senza numeri precisi se non hai case study)
Max 4 righe.

EMAIL 4 — Follow-up diretto (+7 giorni)
Oggetto: Re: [oggetto email 1]
Corpo: 2 righe max. "Riprovo — ha senso parlarne?"
```

**Sequenza LinkedIn (3 touch)**:

```
MESSAGGIO 1 — Connection request (se non connessi)
Nota: aggancio al segnale in 1 riga. Max 300 caratteri.

MESSAGGIO 2 — Primo DM (dopo acceptance)
Stessa logica dell'email 1 — segnale + problema + proposta leggera.
Max 5 righe.

MESSAGGIO 3 — Follow-up (+5-7 giorni)
Breve. "Riprovo — c'è interesse a parlarne?"
```

### Step 5 — QA copy

Prima di consegnare, verifica:
- [ ] Ogni messaggio risponde a: "perché questa persona dovrebbe rispondere ORA?"
- [ ] Nessun riferimento generico che potrebbe applicarsi a qualsiasi azienda
- [ ] CTA è una domanda, non una call to action aggressiva
- [ ] Tono coerente con `clients/[nome]/context/positioning.md`
- [ ] Lunghezza rispettata (email: max 5 righe prima della CTA)

### Step 6 — Salva e lancia

Salva la sequenza in: `clients/[nome]/outbound/sequences/[segnale]-[persona]-[data].md`
Registra la campagna in: `clients/[nome]/outbound/campaigns/`

---

## Examples

```
Input: "Crea una sequenza per startup che ha appena chiuso un Series A, target CEO"
Output: sequenza email 4 touch con oggetto, corpo e CTA calibrati su funding round + problema di costruire pipeline dopo il round.
```

---

## Troubleshooting

**Nessun message house disponibile**: costruisci il message house base da `clients/[nome]/context/positioning.md` prima di procedere.
**Segnale scaduto (180+ giorni)**: non costruire la sequenza. Aspetta un nuovo segnale o cambia approccio (es. contenuto LinkedIn invece di outreach diretto).
