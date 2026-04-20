---
name: account-research
description: Brief approfondito su un prospect specifico prima dell'outreach. Produce un documento con contesto, segnali attivi, persona giusta da contattare, e angolo di messaggio consigliato. Trigger: "research [company.com]", "fai la ricerca su", "prepara il brief per [azienda]".
license: MIT
metadata:
  author: GTM Collective (adattato da KarlRaf/gtm-starter-kit)
  version: 1.0.0
---

## Overview

Ricerca approfondita su un singolo account prima dell'outreach. Output: file datato in `clients/[nome]/outbound/account-research/`. Leggi `clients/[nome]/context/icp-definition.md` e `_methodology/signals/signal-library.md` prima di iniziare.

---

## Instructions

### Step 1 — Input

Ricevi: dominio o nome azienda da ricercare. Chiedi se non fornito.

### Step 2 — Ricerca (5-10 minuti per account)

Fonti da consultare:
- **Sito web**: prodotto, clienti, CTA, tech stack
- **LinkedIn aziendale**: team size attuale, hiring recente, post ultimi 30 giorni
- **LinkedIn fondatori**: post recenti, argomenti trattati, engagement
- **Crunchbase**: funding, investor, data ultimo round
- **Google**: news ultimi 60 giorni, PR, menzioni

### Step 3 — Identifica segnali attivi

Consulta `_methodology/signals/signal-library.md` e identifica:
- Quali segnali sono attivi su questo account?
- Quando sono stati rilevati? (calcola il decay)
- Score totale (incluse combinazioni se multiple)
- Tier risultante (A/B/C)

### Step 4 — Identifica la persona giusta

Consulta `clients/[nome]/context/personas/` e identifica:
- Ruolo più adatto da contattare (in base al segnale e al tipo di azienda)
- Nome specifico se trovato su LinkedIn
- Livello di attività LinkedIn (attivo? silente?)

### Step 5 — Raccomanda l'angolo

In base a segnale + persona + ICP del cliente:
- Canale consigliato (email vs. LinkedIn DM)
- Angolo del messaggio (aggancio al segnale specifico)
- Sequenza da usare (da `clients/[nome]/outbound/sequences/` se esiste)

### Step 6 — Salva output

Salva in: `clients/[nome]/outbound/account-research/YYYY-MM-DD-[nome-azienda].md`

Struttura output:
```markdown
# Research: [Nome Azienda]
Data: [DATA]
Tier: [A/B/C] | Score: [N]

## Overview
[3-4 righe su chi sono e cosa fanno]

## Segnali attivi
- [Segnale]: [quando] — score [N] — decay [%]

## Persona target
- Nome: [se trovato] | Ruolo: [ruolo] | LinkedIn: [URL]

## Angolo consigliato
- Canale: [email / LinkedIn]
- Hook: [prima riga consigliata]
- Sequenza da usare: [nome sequenza]

## Note
[Qualsiasi informazione rilevante non categorizzata]
```

---

## Troubleshooting

**Account non trovabile online**: se il sito è scarso e LinkedIn è vuoto, segnala "informazioni limitate" e basa l'angolo solo sui dati firmografici + segnale rilevato.
**Persona non trovata**: consiglia il ruolo tipo da contare in base alla persona in `clients/[nome]/context/personas/`.
