---
name: setup
description: Popola automaticamente context/ ricercando un dominio pubblicamente. Usare all'inizio di ogni nuovo engagement cliente o per aggiornare il profilo del collettivo. Trigger: "set up this repo for [domain]", "popola il contesto per", "setup per nuovo cliente [nome]".
license: MIT
metadata:
  author: GTM Collective (adattato da KarlRaf/gtm-starter-kit)
  version: 1.0.0
---

## Overview

Ricerca pubblica su un dominio e popola automaticamente i file `clients/[nome]/context/`. Tempo stimato: 30-60 minuti. Richiede conferma prima di sovrascrivere file esistenti.

---

## Instructions

### Step 1 — Ricevi il dominio

Chiedi se non fornito: "Per quale dominio devo fare il setup? (es. acme.com)"

### Step 2 — Ricerca pubblica

Ricerca le seguenti fonti nell'ordine:

1. **Sito web** (`dominio.com`): prodotto, clienti citati, pricing (se visibile), tech stack visibile, CTA principale
2. **LinkedIn aziendale**: dimensione team, hiring recente, post fondatori, settore dichiarato
3. **Crunchbase**: funding history, investor, founding date, team size, descrizione
4. **Job posting**: cercare su LinkedIn/Indeed per capire stack usato, ruoli in espansione, problemi che stanno risolvendo internamente
5. **Google News**: notizie recenti, PR, menzioni in media
6. **G2 / Capterra** (se SaaS): categorie, recensioni, competitor elencati

### Step 3 — Popola context/

Crea o aggiorna questi file con i dati trovati:

**`clients/[nome]/context/profile.md`**:
- Chi sono, cosa fanno, prodotto principale
- Clienti citati (se presenti)
- Team size e fondatori
- Stage e funding (se disponibile)

**`clients/[nome]/clients/[nome]/context/icp-definition.md`** (prima bozza):
- Da job posting e clienti citati, ipotizza chi è il loro ICP
- Settore, dimensione azienda, ruolo decisore
- Nota esplicitamente che è una bozza da validare in kick-off

**`clients/[nome]/clients/[nome]/context/competitor-radar.md`** (prima bozza):
- Competitor menzionati sul sito o su G2
- Come si posizionano rispetto a loro (se visibile)

**`clients/[nome]/clients/[nome]/context/positioning.md`** (prima bozza):
- Headline del sito → che problema risolvono?
- CTA principale → a chi si rivolgono?
- Linguaggio usato → tecnico? business? consumer?

### Step 4 — Chiedi le 5 domande di raffinamento

Dopo la ricerca automatica, chiedi queste domande (opzionali — l'utente può saltarle):

1. C'è qualcosa di importante sul prodotto che non trovo online?
2. Chi è il vostro cliente ideale — quello che porta più valore?
3. Qual è la principale obiezione che sentite nelle call?
4. Quali competitor considerate più pericolosi?
5. C'è un deal recente (vinto o perso) che ha insegnato qualcosa?

### Step 5 — Conferma e salva

Mostra un sommario di cosa hai popolato. Chiedi conferma prima di salvare se ci sono file esistenti da sovrascrivere.

---

## Examples

```
Prompt: "Read skills/setup/SKILL.md and set up this repo for acme.com"
Output: clients/[nome]/context/profile.md, clients/[nome]/context/icp-definition.md, clients/[nome]/context/competitor-radar.md, clients/[nome]/context/positioning.md popolati con dati da ricerca pubblica.
```

---

## Troubleshooting

**Sito non informativo**: usa LinkedIn aziendale come fonte principale. Job posting sono spesso più descrittivi del sito.
**Nessun funding trovato**: non è un problema. Nota "funding: non noto" e procedi.
**Competitor non trovati**: lascia `competitor-radar.md` con la struttura vuota — verrà compilato in kick-off.
