---
name: mkt1-gaccs
description: Genera un GACCS Brief — Goals, Audience, Channels, Creative, Stakeholders — per allineare il team prima di iniziare qualsiasi campagna, lancio o progetto marketing. È il documento operativo più usato del sistema MKT1 e il connettivo tra strategia e esecuzione. Trigger: "GACCS", "brief di campagna", "allineamento prima del lancio", "brief per il team", "mkt1 gaccs", "prepara il brief", "GACCS brief per".
license: MIT
metadata:
  author: GTM Collective (adattato da framework MKT1 — Emily Kramer / Kathleen Estreich)
  version: 2.0.0
---

## Overview

Il GACCS Brief è il documento operativo più usato del sistema MKT1. Va compilato PRIMA di iniziare qualsiasi progetto marketing — anche piccolo. È il connettivo tra strategia (piani, OKR, Marketing Decision Dashboard) ed esecuzione quotidiana.

**GACCS** = **G**oals · **A**udience · **C**hannels · **C**reative · **S**takeholders

Senza un GACCS Brief: scope creep, team misallineato, lavoro fatto in silos, difficoltà a misurare il successo e a capire cosa ha funzionato.

Output: `outbound/campaigns/YYYY-MM-DD-gaccs-[nome-campagna].md`

---

## Quando usare il GACCS Brief

Segnale chiaro: ogni volta che apri un nuovo documento, file o task in project management per un'iniziativa marketing — scrivi prima il GACCS.

Esempi:
- Campagne outbound email o LinkedIn
- Lancio di una feature o prodotto
- Produzione di un asset (report, case study, webinar, template)
- Evento (organizzato o partecipazione)
- Campagna paid
- Qualsiasi Big Bet o iniziativa strategica

---

## Le 5 componenti del GACCS

### G — Goals (Obiettivi)

Un solo obiettivo principale. Non "generare awareness e lead e costruire brand" — uno.

**Domande guida:**
- Perché stiamo facendo questo progetto?
- Quale outcome definisce il successo?
- Come si collega agli KPO Goals annuali/trimestrali? (Lever prioritario? KPI goal? Project goal?)

**Formato:**
> "Obiettivo: [azione specifica] — [target numerico se possibile] — entro [data]"

Esempi:
> "Obiettivo: generare 8 meeting qualificati con CEO di startup SaaS che hanno chiuso un round — entro fine mese"
> "Obiettivo: raccogliere 200 risposte alla survey outbound — entro 2 settimane"
> "Obiettivo: lanciare il case study e generare 3 richieste di demo da prospect nel settore HR-tech"

---

### A — Audience (Chi)

Chi raggiunge questa campagna, con precisione.

**Domande guida:**
- Qual è il profilo firmografico? (settore, dimensione, fase, geografia)
- Chi è il decisore o il persona target? (ruolo, seniority, pain)
- Qual è il segnale che li qualifica adesso — non "in generale" ma "in questo momento"?
- Quante persone corrispondono? (stima della lista)
- Da quale tier ICP provengono? (proven/scaling/testing)

**Formato:**
> "Audience: [ruolo] in [tipo azienda] con [segnale qualificante] — tier ICP: [X] — stima: [N] contatti"

---

### C — Channels (Come li raggiungiamo)

Quale canale o combinazione di canali è più efficace per questa Audience con questo Goal.

**Domande guida:**
- Dove si trova questa audience?
- Quale canale ha la più alta probabilità di conversione per questo obiettivo specifico?
- Stiamo usando un solo Engine o una combinazione (pairing)?
- Qual è la sequenza esatta dei touchpoint?

**Riferimento:** usa `mkt1_channel_strategy` per la scelta dei canali primari. Considera i 10 channel pairing documentati nella skill.

**Formato:**
> "Engine primario: [canale]"
> "Sequenza: [step 1] → [step 2] → [step 3]"

---

### C — Creative (Cosa diciamo)

Il contenuto, il messaggio e il formato — il Fuel di questa campagna.

**Domande guida:**
- Qual è l'hook principale? (prima frase, angolo, insight)
- Quale Perception strategica rafforza? (da `mkt1_perceptions`)
- Qual è il formato? (email testo, post LinkedIn, PDF, landing page, video...)
- Qual è la call-to-action? (cosa vogliamo che faccia dopo)
- Il creative è coerente con il positioning e lo Story Stack?

**Formato:**
> "Hook: [prima frase o angolo]"
> "Perception target: [quale Perception rafforza]"
> "Formato: [tipo di creative/fuel]"
> "CTA: [azione richiesta]"

**Nota — 30% Juice Rule**: il creative non deve parlare solo del prodotto. Solo il ~30% del contenuto dovrebbe essere direttamente sul prodotto ("the juice") — il restante 70% copre problemi, trend, vision, storie, use case.

---

### S — Stakeholders (Chi è coinvolto)

Chi deve essere nel loop, chi prende decisioni, chi esegue.

**Domande guida:**
- Chi è il DRI (Directly Responsible Individual) — una sola persona?
- Chi deve approvare prima del lancio?
- Chi contribuisce all'esecuzione?
- Chi deve essere informato dell'output?
- Ci sono dipendenze esterne (product, sales, CS)?

**Formato:**
> "DRI: [nome/ruolo]"
> "Approvatori: [lista]"
> "Contributori: [lista]"
> "Informati: [lista]"

---

## GACCS Brief — Template completo

```
# GACCS Brief — [nome campagna]
Data: [YYYY-MM-DD]
Big Bet associato: [titolo Big Bet, se applicabile]
KPO Goal associato: [KPI / Project / Ops goal]

## G — Goals
[obiettivo specifico + metrica + data]
Collegamento agli obiettivi trimestrali: [quale KPO Goal serve]

## A — Audience
[profilo firmografico + persona + segnale qualificante]
Tier ICP: [proven / scaling / testing]
Stima lista: [N] contatti

## C — Channels (Engine)
Engine primario: [canale]
Engine secondario: [canale, se applicabile]
Sequenza: [step 1] → [step 2] → [step 3]

## C — Creative (Fuel)
Hook: [prima frase o angolo]
Perception target: [quale Perception rafforza]
Formato: [tipo]
CTA: [azione richiesta]
Note creative: [tono, vincoli, riferimenti]

## S — Stakeholders
DRI: [nome/ruolo]
Approvatori: [lista]
Contributori: [lista]
Informati: [lista]
```

---

## Processo di utilizzo

**Versione breve prima** — usa il template per allineare il team e ottenere buy-in iniziale.

**Versione espansa dopo** — sviluppa il GACCS in piano campagna completo con timeline, task e milestone.

**Review con stakeholders** — usa il GACCS come rubrica di review: ogni componente è allineato? Il Goal è misurabile? L'Audience è sufficientemente specifica? Il Creative riflette le Perceptions?

---

## Esempio completo

```
# GACCS Brief — Campagna Funding Signal Aprile 2026
Data: 2026-04-18
Big Bet: Big Bet 1 — "Report Outbound B2B Italia"
KPO Goal: KPI — meeting qualificati Q2

## G — Goals
Generare 6 meeting qualificati con CEO/co-founder di startup B2B SaaS
che hanno chiuso un round seed/serie A negli ultimi 45 giorni.
Entro: 30 aprile 2026.
Collegamento: KPI goal Q2 — meeting booked.

## A — Audience
CEO/co-founder, startup B2B SaaS (HR-tech, travel, healthcare)
Seed o Serie A chiusa negli ultimi 45 giorni, Italia
Tier ICP: proven (segnale funding = trigger primario)
Stima: 35-50 contatti

## C — Channels (Engine)
Engine primario: cold email
Engine secondario: LinkedIn DM (follow-up)
Sequenza: email 1 (hook signal) → +3gg email 2 (social proof) → +5gg LinkedIn DM

## C — Creative (Fuel)
Hook: "Ho visto che avete chiuso il round — nei prossimi 90 giorni di solito arriva la pressione su pipeline."
Perception target: "Chi parte dalle campagne sbaglia l'ordine"
Formato: email testo plain, max 120 parole
CTA: "Ha senso una call di 20 min?"
Note: tono diretto, no complimenti, no "vi scrivo perché...", aggancia il segnale nella prima riga

## S — Stakeholders
DRI: [nome GTM engineer del collettivo]
Approvatori: [nome PMM senior]
Contributori: [nome junior per list building]
Informati: tutto il team
```

---

## Troubleshooting

**Goal vago**: "aumentare la brand awareness" non è un Goal GACCS. Aggiungi sempre una metrica e una scadenza. Se non riesci a misurarlo, posticipa il lancio.

**Audience troppo larga**: se la lista supera 300-400 contatti per una campagna outbound, è troppo generica — aggiungi un segnale qualificante o un filtro di fase.

**DRI assente o multipli**: ogni progetto deve avere UN solo DRI. Se ci sono due persone "responsabili", nessuno è davvero responsabile. Nomina uno, l'altro è contributore.

**Creative non allineato alle Perceptions**: se il messaggio non rafforza almeno una Perception strategica, chiediti se vale la pena farlo. Il test rapido: questo contenuto potrebbe essere prodotto da un competitor? Se sì, ripensa l'angolo.
