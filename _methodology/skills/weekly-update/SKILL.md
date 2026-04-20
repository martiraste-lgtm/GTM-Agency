---
name: weekly-update
description: Mantiene context/ e kpi/ aggiornati ogni lunedì. Identifica contenuti obsoleti, aggiorna dashboard metriche, propone aggiustamenti. Trigger: "weekly update", "aggiorna il contesto", "lunedì update", "esegui il weekly".
license: MIT
metadata:
  author: GTM Collective (adattato da KarlRaf/gtm-starter-kit)
  version: 1.0.0
---

## Overview

Eseguire ogni lunedì mattina. Legge context/ e kpi/ esistenti, identifica cosa è obsoleto, chiede aggiornamenti solo per elementi che Claude non può trovare autonomamente, e aggiorna i file.

---

## Instructions

### Step 1 — Leggi lo stato attuale

Leggi questi file:
- `CLAUDE.md` (sezione "Stato corrente")
- `_agency/context/icp-definition.md`
- `_methodology/signals/signal-library.md`
- `kpi/dashboard.md`
- `_agency/outbound/campaigns/` (campagne attive)
- `_agency/knowledge/INDEX.md`

### Step 2 — Ricerca aggiornamenti pubblici

Per il collettivo o per il cliente (a seconda del repo):
- LinkedIn aziendale: nuovi post, cambi team, hiring
- News recenti (Google Alert sul dominio/brand)
- Segnali nuovi o aggiornati (verifica decay su quelli esistenti)

### Step 3 — Identifica obsolescenze

Elementi da aggiornare:
- Segnali con decay scaduto (180+ giorni) → rimuovere da lista attiva
- Campagne terminate → archiviare in `_agency/outbound/campaigns/archivio/`
- ICP o persona non aggiornata da più di 60 giorni → segnalare
- Competitor con novità rilevanti (funding, lancio, cambi) → aggiornare radar

### Step 4 — Chiedi solo quello che non puoi trovare

Poni domande solo per dati non pubblicamente disponibili:
- "Ci sono nuovi deal chiusi o persi da aggiornare in `_agency/knowledge/deals/`?"
- "Ci sono nuove obiezioni emerse nelle call questa settimana?"
- "Le metriche campagna sono aggiornate? (open rate, reply rate, meeting)"
- "C'è qualcosa di rilevante sul cliente/prospect che non è online?"

### Step 5 — Aggiorna i file

Aggiorna direttamente:
- `kpi/dashboard.md`: colonna "Valore corrente" con nuovi dati
- `_methodology/signals/signal-library.md`: rimuovi segnali scaduti, aggiorna note su segnali performanti
- `CLAUDE.md` sezione "Stato corrente": data, ICP prioritario, campagne attive, next actions

### Step 6 — Summary

Produci un sommario in 5-7 punti:
- Cosa è stato aggiornato
- Cosa richiede attenzione questa settimana
- Segnali nuovi o in scadenza
- Next actions prioritarie

---

## Troubleshooting

**Nessun dato nuovo**: va bene. Registra "nessuna novità rilevante" e aggiorna solo la data.
**Dati campagna mancanti**: chiedi all'utente di aggiornare `kpi/dashboard.md` con le metriche prima di procedere.
