---
name: mkt1-gaccs
description: Genera un GACCS Brief — Goal, Audience, Channels, Content, Success — per allineare il team prima di iniziare qualsiasi campagna, lancio o progetto marketing. È il documento di partenza per ogni iniziativa operativa. Trigger: "GACCS", "brief di campagna", "allineamento prima del lancio", "brief per il team", "mkt1 gaccs", "prepara il brief", "GACCS brief per".
license: MIT
metadata:
  author: GTM Collective (adattato da framework MKT1 — Emily Kramer / Kathleen Estreich)
  version: 1.0.0
---

## Overview

Il GACCS Brief è il documento operativo più usato del sistema MKT1. Va compilato PRIMA di iniziare qualsiasi campagna, lancio o progetto marketing — anche piccolo. Evita il problema più comune: team che lavora su tattiche senza un obiettivo condiviso, audience vaga, canali scelti per abitudine, contenuto generico, e metriche di successo mai definite.

5 minuti a compilarlo risparmiano settimane di lavoro mal diretto.

Output: `outbound/campaigns/YYYY-MM-DD-gaccs-[nome-campagna].md`

---

## Instructions

### Step 1 — Trigger

Usa questa skill prima di:
- Lanciare una sequenza di outbound email o LinkedIn
- Produrre un nuovo asset (report, case study, webinar)
- Avviare una campagna paid
- Organizzare o partecipare a un evento
- Fare un lancio (feature, prodotto, partnership)

### Step 2 — Le 5 sezioni del GACCS

Compila in ordine. Non saltare sezioni — ognuna dipende dalla precedente.

---

**G — Goal (Obiettivo)**

Un solo obiettivo principale. Non "aumentare la brand awareness e generare lead e costruire la community" — uno.

Domande guida:
- Cosa vogliamo che accada come risultato diretto di questa campagna?
- Come misuri se ha funzionato?
- Entro quando?

Formato:
> "Obiettivo: [azione specifica] — [target numerico] — entro [data]"

Esempi:
> "Obiettivo: generare 8 meeting qualificati con founder SaaS HR-tech — entro 30 giorni"
> "Obiettivo: raccogliere 150 risposte alla survey outbound — entro 2 settimane"

---

**A — Audience (Chi)**

Chi raggiunge questa campagna, con precisione chirurgica.

Domande guida:
- Qual è il profilo firmografico esatto? (settore, dimensione, fase, mercato geografico)
- Qual è il profilo del decisore? (ruolo, livello di seniority, pain principale)
- Qual è il segnale che li qualifica come rilevanti ora? (non "in generale", ma "in questo momento")
- Quante persone corrispondono a questo profilo? (stima della lista)

Formato:
> "Audience: [ruolo] in [tipo azienda] con [segnale qualificante] — stima lista: [N] contatti"

---

**C — Channels (Come li raggiungiamo)**

Quale canale o combinazione di canali è il più efficace per raggiungere questa Audience con questo Goal.

Domande guida:
- Dove si trova questa audience? (LinkedIn, email, eventi, community...)
- Quale canale ha la maggiore probabilità di conversione per questo specifico obiettivo?
- Qual è la sequenza? (es. LinkedIn connection → email 1 → email 2 → follow-up LinkedIn)

Formato:
> "Channel primario: [canale]"
> "Sequenza: [step 1] → [step 2] → [step 3]"

---

**C — Content (Cosa diciamo)**

Quale messaggio, angolo e formato usiamo per raggiungere questa Audience attraverso questi Channels.

Domande guida:
- Qual è il hook principale? (la prima frase che fa fermare il reader)
- Quale Perception strategica rafforza questo contenuto?
- Qual è il formato? (email, post LinkedIn, PDF, video, landing page)
- Qual è la call-to-action? (cosa vogliamo che il reader faccia adesso)

Formato:
> "Hook: [prima frase o angolo]"
> "Perception target: [quale delle Perceptions strategiche rafforza]"
> "Formato: [tipo di contenuto]"
> "CTA: [azione richiesta]"

---

**S — Success (Come misuriamo)**

Due metriche: una di input (che possiamo controllare) e una di output (il risultato).

Domande guida:
- Qual è la metrica di input? (es. N email inviate, N post pubblicati, N DM mandati)
- Qual è la metrica di output? (es. reply rate, meeting booked, download, iscrizioni)
- Qual è il target per ognuna?
- Come e quando raccogliamo i dati?

Formato:
> "Input: [metrica] — target: [numero]"
> "Output: [metrica] — target: [numero]"
> "Review: [data o frequenza]"

---

### Step 3 — GACCS Brief completo (template)

```
# GACCS Brief — [nome campagna]
Data: [YYYY-MM-DD]
Big Bet associato: [titolo Big Bet, se applicabile]

## G — Goal
[obiettivo + target + data]

## A — Audience
[profilo + segnale qualificante + stima lista]

## C — Channels
Primario: [canale]
Sequenza: [step 1] → [step 2] → [step 3]

## C — Content
Hook: [prima frase o angolo]
Perception target: [quale Perception]
Formato: [tipo]
CTA: [azione richiesta]

## S — Success
Input: [metrica] — target: [N]
Output: [metrica] — target: [N]
Review: [quando]
```

### Step 4 — Salva e condividi

Salva in `outbound/campaigns/YYYY-MM-DD-gaccs-[nome-campagna].md`.

Prima di iniziare l'esecuzione, condividi il brief con il team e verifica:
- [ ] Tutti concordano sull'obiettivo?
- [ ] L'audience è abbastanza specifica da costruire una lista reale?
- [ ] Il contenuto è allineato con il canale scelto?
- [ ] Le metriche di successo sono misurabili?

---

## Esempi

**GACCS completo per campagna outbound:**

```
# GACCS Brief — Campagna Funding Signal Q2 2026
Data: 2026-04-18

## G — Goal
Generare 6 meeting qualificati con founder/CEO di startup SaaS
che hanno chiuso un round negli ultimi 45 giorni — entro 30 aprile.

## A — Audience
CEO/co-founder di startup B2B SaaS (HR-tech, travel, healthcare)
Seed o Serie A chiusa negli ultimi 45 giorni
Italia o mercato DACH con sede italiana
Stima lista: 30-50 contatti

## C — Channels
Primario: cold email
Sequenza: email 1 (hook signal) → wait 3gg → email 2 (social proof) → wait 5gg → LinkedIn DM

## C — Content
Hook: "Ho visto che avete chiuso il round — di solito nei prossimi 90 giorni arriva la pressione su pipeline."
Perception target: "Chi parte dalle campagne sbaglia l'ordine"
Formato: email testo plain, max 120 parole
CTA: "Ha senso una call di 20 min per vedere se siamo rilevanti per voi?"

## S — Success
Input: 40 email inviate — target: 40
Output: reply rate ≥ 8%, meeting booked ≥ 6
Review: ogni 7 giorni
```

---

## Troubleshooting

**Goal vago**: "aumentare la visibilità" non è un Goal GACCS. Chiedi "visibilità come si misura? entro quando? con quale azione specifica del buyer?". Riformula finché non è misurabile.

**Audience troppo larga**: "startup B2B" non è un'Audience. Aggiungi settore + fase + segnale qualificante. Se la lista supera 500 contatti per una singola campagna, è troppo larga — riduci.

**Metriche mancanti**: se non sai come misurare il successo prima di iniziare, posticipa il lancio finché non lo sai. Campagne senza metriche non insegnano niente.
