---
name: mkt1-channel-strategy
description: Determina il miglior channel mix in base a stage aziendale, audience, GTM motion e Marketing Advantages. Non tutti i canali funzionano in ogni contesto — questa skill elimina gli sprechi e indica dove investire davvero. Trigger: "channel strategy", "quali canali usare", "dove investire nel marketing", "channel mix", "mkt1 channel", "quali canali per il GTM".
license: MIT
metadata:
  author: GTM Collective (adattato da framework MKT1 — Emily Kramer / Kathleen Estreich)
  version: 1.0.0
---

## Overview

La maggior parte delle startup prova troppi canali allo stesso tempo e ottiene risultati mediocri su tutti. La Channel Strategy MKT1 lavora in 3 filtri sequenziali: prima elimina i canali sbagliati per lo stage, poi per la GTM motion, poi amplifica in base ai Marketing Advantages. Il risultato è 2-3 canali su cui concentrarsi davvero.

Prerequisiti: `mkt1_company_overview` + `mkt1_marketing_advantages`.
Output: aggiorna `signals/signal-routing.md` e orienta la configurazione di `outbound/sequences/`.

---

## Instructions

### Step 1 — Raccolta dati

Prima di filtrare, raccogli:
1. **Stage** (seed / serie A / growth)
2. **GTM motion principale** (PLG / SLG / PLS / MLG / community-led)
3. **ACV medio** (sotto 5K/anno, 5-25K/anno, 25K+/anno)
4. **ICP** (chi è il buyer, dove vive online)
5. **Marketing Advantages disponibili** (output della skill precedente)
6. **Risorse attuali** (team size marketing, budget indicativo)

### Step 2 — Filtro 1: Stage aziendale

Elimina i canali che non sono appropriati per lo stage attuale:

| Stage | Canali validi | Canali da evitare |
|-------|--------------|-------------------|
| **Pre-seed / Seed** | Outbound diretto, LinkedIn founder, community, referral programmatico | Paid ads (troppo costoso senza conversion data), SEO (troppo lento), eventi tier 1 |
| **Serie A** | Outbound, content/SEO iniziale, LinkedIn, events selezionati, partner | Mass paid senza conversion history |
| **Growth** | Tutti — ma con priorità basata su unit economics | Nessuno escluso a priori, ma testare con dati |

### Step 3 — Filtro 2: GTM motion

Ogni GTM motion favorisce canali specifici:

| GTM Motion | Canali prioritari | Logica |
|------------|-------------------|--------|
| **SLG** (Sales-Led) | Outbound with signals, LinkedIn outreach, events, referral | Il buyer si vuole parlare — incontralo dove è |
| **PLG** (Product-Led) | SEO, community, in-product, content | L'acquisizione avviene attraverso il prodotto stesso |
| **PLS** (Product-Led Sales) | PLG + outbound selettivo sui product qualified leads | Il prodotto genera il lead, sales chiude |
| **MLG** (Marketing-Led) | Content, SEO, paid, events — generate demand che poi va a sales | Volume → qualifica → sales |
| **Community-Led** | Community building, eventi, UGC, champions program | Il flywheel è la community stessa |

**Per il collettivo (SLG puro)**: outbound with signals + LinkedIn sono i canali primari.

### Step 4 — Filtro 3: Marketing Advantages

I Marketing Advantages determinano quale canale puoi rendere slealmente efficace:

| Advantage | Canale che amplifica |
|-----------|---------------------|
| Founder con audience | LinkedIn + newsletter founder |
| Community propria | Community-led, events |
| Contenuto / SEO esistente | SEO, content marketing |
| Dati proprietari | Personalizzazione outbound, reportistica settoriale |
| Ecosistema / integrazioni | Partnership, co-marketing |
| Expertise di categoria | Thought leadership, speaking, media |
| Effetti di rete | Referral, viral loop, in-product |

Aggiungi ai canali già filtrati il canale amplificato dall'Advantage — e mettilo in cima alla priorità.

### Step 5 — ACV e canale

L'ACV (valore medio del contratto annuale) influenza il rapporto effort/ritorno per canale:

| ACV | Canali a ROI positivo |
|-----|-----------------------|
| < 5K/anno | PLG, SEO, community, contenuto self-serve |
| 5-25K/anno | Outbound, LinkedIn, content + sales assist |
| 25K+/anno | Outbound personalizzato, events, referral |

### Step 6 — Selezione finale e prioritizzazione

Dopo i 3 filtri, dovresti avere 3-5 canali candidati. Seleziona i top 2-3 usando questa logica:

1. **Canale primario**: quello con il miglior rapporto tra probabilità di funzionare e risorse necessarie
2. **Canale secondario**: complementare al primario, diverso per formato (es. email + LinkedIn)
3. **Canale sperimentale** (opzionale): uno da testare con budget/tempo limitato

### Step 7 — Output

Documenta il channel mix selezionato:

```
Channel primario: [nome]
Perché: [logica basata su stage + motion + advantage]
Come si attiva: [tattiche specifiche, frequenza, KPI]

Channel secondario: [nome]
Perché: [logica]
Come si attiva: [tattiche specifiche]

Channel sperimentale: [nome o "nessuno per ora"]
```

Salva in `outputs/YYYY-MM-DD-channel-strategy-[cliente].md`.
Aggiorna `signals/signal-routing.md` con i canali selezionati come output dei trigger.

---

## Troubleshooting

**"Vogliamo fare tutto"**: usa il filtro dell'ACV. Se l'ACV è sotto 10K, non puoi permetterti canali ad alta intensità di sales. Se è sopra 30K, il contenuto organico non converte abbastanza veloce.

**Canale che "ha sempre funzionato" nel passato**: valida se era vero o solo apparentemente. Se era referral di reti personali, non è un canale scalabile — è un advantage di network che si esaurisce.
