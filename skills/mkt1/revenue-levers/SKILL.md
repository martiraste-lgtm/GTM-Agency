---
name: mkt1-revenue-levers
description: Identifica e stack-ranka i 4 Revenue Lever MKT1 — i soli 4 modi ad alto livello per far crescere il revenue nel B2B marketing. Forza una scelta su dove concentrare lo sforzo adesso. Trigger: "revenue levers", "dove concentrare il marketing", "priorità marketing", "cosa fa muovere il revenue", "mkt1 levers", "stack rank marketing".
license: MIT
metadata:
  author: GTM Collective (adattato da framework MKT1 — Emily Kramer / Kathleen Estreich)
  version: 2.0.0
---

## Overview

Ci sono solo 4 modi ad alto livello per far crescere il revenue nel B2B marketing. La maggior parte delle startup cerca di azionarli tutti contemporaneamente — con le stesse risorse — e ottiene risultati marginali su tutto.

Questa skill forza una scelta: quale lever ha il maggiore impatto sul revenue adesso, in questa fase specifica? Non per sempre — ma per il prossimo trimestre. Poi lo stack rank si aggiorna.

Prerequisiti: `mkt1_company_overview` (per conoscere stage, ICP, funnel).
Output: aggiorna `kpi/dashboard.md` con il lever prioritario e i KPI trimestrali.

---

## I 4 Revenue Lever MKT1

| Lever | Descrizione | In una frase |
|-------|-------------|-------------|
| **Lever 1 — Più ToF con l'ICP core** | Acquisire più quote di mercato nel segmento già validato | "Più della stessa torta" |
| **Lever 2 — Più ToF con nuovo ICP** | Espandere il mercato indirizzabile verso nuovi segmenti | "Una torta più grande" |
| **Lever 3 — Aumenta il valore dei clienti** | Pricing più alto, upsell, expansion, shift verso segmenti premium | "Vendere torte più costose" |
| **Lever 4 — Aumenta l'efficienza** | Migliorare i conversion rate, abbassare il CAC, eliminare sprechi | "Meno torta nel cestino" |

---

## Dettaglio dei 4 Lever

### Lever 1 — Aumenta il top of funnel con l'audience core

**Cosa fa**: cattura una quota maggiore dell'ICP già validato — stesso segmento, più penetrazione.

Quando prioritizzare:
- Hai un ICP "proven" ma hai raggiunto solo una piccola parte del TAM
- Il tasso di conversione è buono ma il volume è basso
- Hai playbook che funzionano e vuoi scalare l'esecuzione

Tattiche tipiche: outbound più aggressivo sullo stesso ICP, più budget ai canali che convertono già, programmi referral, espansione geografica sullo stesso profilo.

---

### Lever 2 — Aumenta il top of funnel con nuovo ICP

**Cosa fa**: espande il mercato indirizzabile verso segmenti che non hai ancora toccato.

Quando prioritizzare:
- Il mercato core si sta saturando o il TAM è troppo piccolo per gli obiettivi di crescita
- Vuoi esplorare nuovi verticali, dimensioni aziendali o use case
- Hai prove che altri segmenti potrebbero convertire (segnali organici, deal inaspettati)

Tattiche tipiche: nuove campagne per segmento, adattamento del messaging, test su nuovi canali specifici all'ICP, partnership in nuovi ecosistemi.

**Attenzione**: il Lever 2 richiede più risorse del Lever 1 — stai essenzialmente costruendo un go-to-market parallelo. Prioritizzalo solo quando il Lever 1 è sufficientemente maturo.

---

### Lever 3 — Aumenta il valore dei clienti

**Cosa fa**: cresce il revenue dai clienti esistenti senza acquisirne di nuovi.

Quando prioritizzare:
- Il churn è gestibile ma il NRR è inferiore al 100%
- C'è opportunità di upsell o cross-sell non sfruttata
- Il mix clienti è troppo sbilanciato verso tier low-value
- Il pricing non riflette il valore erogato

Tattiche tipiche: programmi di upsell/expansion, repricing, shift verso clienti enterprise, lifecycle marketing per onboarding e adoption, CS proattivo.

---

### Lever 4 — Aumenta l'efficienza

**Cosa fa**: ottimizza il funnel esistente — più conversioni con le stesse o meno risorse.

Quando prioritizzare:
- Il volume è ok ma il conversion rate è basso
- Il CAC è troppo alto rispetto all'LTV
- Ci sono sprechi visibili nel funnel (drop-off elevato in fasi specifiche)
- Si vuole fare più con lo stesso budget prima di chiedere risorse aggiuntive

Tattiche tipiche: ottimizzazione landing page, A/B test su copy e sequenze, affinamento del targeting, riduzione del sales cycle, miglioramento del lead scoring.

---

## Instructions

### Step 1 — Assessment dello stato attuale

Per ogni lever, valuta:
- **Stato attuale**: sto già lavorando su questo lever? Con che intensità?
- **Bottleneck**: c'è un problema evidente che questo lever risolverebbe?
- **Potenziale impatto**: quanto revenue aggiuntivo può generare nei prossimi 90 giorni?
- **Risorse necessarie**: quanto effort richiede attivarlo o amplificarlo?

### Step 2 — Stack rank

Assegna priorità 1-4 ai lever. Un solo lever può essere al rango 1.

Logica di prioritizzazione per stage:

| Stage | Lever tipicamente prioritario |
|-------|-------------------------------|
| Pre-seed / Seed | Lever 1 (valida il core ICP prima di espandere) |
| Serie A | Lever 1 + Lever 4 (scala e ottimizza) |
| Growth | Lever 2 o Lever 3 (espansione o monetizzazione) |
| Qualsiasi stage | Lever 4 se il funnel è chiaramente inefficiente |

### Step 3 — Piano d'azione per il lever prioritario

Per il lever rank 1:
1. **3 tattiche specifiche** che lo spostano nei prossimi 90 giorni
2. **KPI principale** con target numerico
3. **Segnale che indica che il lever è risolto** (quando sposta di priorità)

### Step 4 — Allineamento cross-funzionale

Il stack rank dei Revenue Lever deve essere condiviso con sales, product e leadership. Il marketing non può prioritizzare il Lever 2 se sales non è pronto a gestire un nuovo ICP, né il Lever 3 se CS non ha playbook di upsell.

### Step 5 — Output

```
Revenue Lever Stack Rank — [trimestre]

Lever 1 (priorità [N]): [Lever name]
Stato attuale: [descrizione]
Perché ora: [ragione]
Tattiche: [A, B, C]
KPI: [metrica] → target: [numero] entro [data]
Segnale di risoluzione: [quando questo lever scala di priorità]

Lever 2 (priorità [N]): ...
Lever 3 (priorità [N]): ...
Lever 4 (priorità [N]): ...
```

Salva in `outputs/YYYY-MM-DD-revenue-levers-[cliente].md`.
Aggiorna `kpi/dashboard.md` con i KPI del lever prioritario come metriche primarie del trimestre.

---

## Troubleshooting

**"Tutti e 4 i lever sono importanti"**: vero, ma non tutti sono ugualmente bloccanti adesso. Chiedi "se potessi lavorare solo su uno per i prossimi 90 giorni, quale cambierebbe più il revenue?" — poi usa quello come punto di partenza.

**Lever in conflitto**: a volte Lever 1 e Lever 2 sembrano entrambi prioritari. Regola: il Lever 1 viene prima finché il TAM core non è sufficientemente penetrato (> 20% del TAM accessibile) o finché il business model non è validato su quel segmento.

**Il Lever 4 viene sempre trascurato**: è il più noioso ma spesso il più efficiente a breve termine. Se il conversion rate su un canale già attivo è basso, migliorarlo è spesso più veloce che aprire un nuovo canale.
