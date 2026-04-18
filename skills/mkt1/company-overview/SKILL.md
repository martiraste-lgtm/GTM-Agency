---
name: mkt1-company-overview
description: Documenta i driver fondamentali della strategia — stage, modello di business, audience, competitive landscape. È il prerequisito per tutte le altre skill MKT1. Senza questa base, perceptions e channel strategy sono costruiti su sabbia. Trigger: "company overview", "documentiamo il contesto del cliente", "fondamenta strategia", "stage e business model", "chi è il cliente e come guadagna".
license: MIT
metadata:
  author: GTM Collective (adattato da framework MKT1 — Emily Kramer / Kathleen Estreich)
  version: 1.0.0
---

## Overview

Questa skill costruisce il "Company Overview" — il documento di partenza da cui tutto il resto deriva. Non è un profilo generico: è un'analisi strutturata dei 4 driver che determinano TUTTE le scelte di marketing. Senza conoscere lo stage, il modello di monetizzazione, il profilo del buyer e il competitive landscape reale, qualsiasi strategia marketing è una congettura.

Output: aggiorna `context/profile.md` e `context/icp-definition.md` con i dati raccolti.

---

## Instructions

### Step 1 — Stage aziendale

Chiedi e documenta con precisione:

1. **Fase**: pre-seed, seed, serie A, series B+, growth, scale
2. **Revenue attuale**: MRR, ARR, o "pre-revenue"
3. **Numero clienti paganti** (non trial, non pilot gratuiti)
4. **Tasso di crescita MoM o YoY** (anche approssimativo)
5. **Runway** (quanto tempo hanno con il funding attuale)
6. **Status PMF**: cercare, vicini, raggiunto, consolidando

**Domanda chiave**: "Stai ancora cercando il modello che funziona, o stai scalando qualcosa che già funziona?"

### Step 2 — Modello di business

Capire esattamente come fa soldi:

1. **Modello di revenue**: subscription (MRR), transazionale (per uso), freemium, marketplace (take rate), servizi + software, altro
2. **Piano pricing**: tier, range di prezzo, ACV medio
3. **Ciclo di vendita**: self-serve, sales-assisted, full enterprise (durata media)
4. **Expansion revenue**: c'è upsell / cross-sell? Net revenue retention?
5. **Unit economics**: CAC payback period (se lo conoscono), LTV/CAC ratio

**Domanda chiave**: "Cosa succede operativamente quando un cliente passa da free a paying, o da un tier all'altro?"

### Step 3 — Audience

Documentare il buyer reale (non quello teorico):

1. **ICP primario**: titolo, industria, dimensione azienda, fase aziendale
2. **Chi scopre il prodotto** vs. **chi firma il contratto** (spesso diversi)
3. **Chi usa il prodotto** (end user) — coincide con chi firma?
4. **Quante persone sono coinvolte nella decisione** (buying committee)
5. **Dove passa il tempo online**: community, newsletter, eventi, social
6. **Il problema principale** in parole loro (non nella formulazione del prodotto)

**Domanda chiave**: "Raccontami l'ultimo cliente che hai acquisito: chi era, come ti ha trovato, perché ha firmato?"

### Step 4 — Competitive landscape

Mappa reale delle alternative:

1. **Competitor diretti**: stessa categoria, stesso buyer
2. **Alternative indirette**: soluzioni diverse che risolvono lo stesso problema (Excel, processo manuale, nessuno)
3. **Come il mercato categorizza questo prodotto** (non come si categorizza il founder)
4. **Dove si posiziona rispetto ai competitor**: prezzo, features, segmento, go-to-market
5. **Come vincono i deal** vs. come li perdono (pattern ricorrenti)
6. **Il competitor più pericoloso** e perché

**Domanda chiave**: "Quando un prospect non compra da te, cosa fa invece?"

### Step 5 — Sintesi e documento

Produci un Company Overview strutturato in 4 sezioni (una per ogni step) e salva in `outputs/YYYY-MM-DD-company-overview-[cliente].md`.

Poi aggiorna:
- `context/profile.md` con i dati di stage, modello e differenziatori chiave
- `context/icp-definition.md` con il buyer reale documentato

---

## Troubleshooting

**Il cliente non conosce le sue metriche**: usa range ("tra X e Y") o chedi "a spanne, quanti clienti paganti avete?". Non inventare numeri, documenta "dato non disponibile".

**ICP multipli**: documenta tutti e 2-3, poi chiedi "se dovessi fare outbound solo a uno, quale sarebbe?" — quello è il primario.

**Competitive landscape vago**: fai vedere una lista di 5-6 player del settore e chiedi "chi di questi è rilevante per te, e come ti differenzi da ognuno?".
