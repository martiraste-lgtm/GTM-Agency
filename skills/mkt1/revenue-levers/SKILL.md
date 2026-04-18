---
name: mkt1-revenue-levers
description: Identifica e stack-ranka i 4 revenue lever — Awareness, Engagement, Conversion, Retention/Expansion — per capire dove il marketing può avere il massimo impatto adesso. Evita di fare tutto a metà. Trigger: "revenue levers", "dove concentrare il marketing", "priorità marketing", "cosa fa muovere il revenue", "mkt1 levers", "stack rank marketing".
license: MIT
metadata:
  author: GTM Collective (adattato da framework MKT1 — Emily Kramer / Kathleen Estreich)
  version: 1.0.0
---

## Overview

Il problema più comune nelle startup è cercare di fare tutto contemporaneamente: generare awareness, nurturare i lead, convertire, e anche fare retention — con le stesse 2-3 persone e lo stesso budget. Il risultato è che ogni lever viene azionato a metà e nessuno produce risultati significativi.

Questa skill forza una scelta: quale lever ha il maggiore impatto sul revenue adesso, in questa fase specifica? Non per sempre — ma per il prossimo trimestre.

Prerequisiti: `mkt1_company_overview` (per conoscere stage, funnel, unit economics).
Output: aggiorna `kpi/dashboard.md` con la priorità dei lever e i KPI associati.

---

## Instructions

### Step 1 — I 4 Revenue Lever

| Lever | Cosa fa | Metriche chiave |
|-------|---------|-----------------|
| **Awareness** | Porta nuove persone a sapere che esisti e a capire cosa fai | Brand awareness, reach, first-touch attribution, traffic top of funnel |
| **Engagement** | Trasforma chi ti conosce in chi è interessato — nurture, educazione, trust building | Email open rate, content engagement, return visits, MQL volume |
| **Conversion** | Converte l'interesse in azione: trial, demo, acquisto | Conversion rate, demo booked, pipeline generata, CAC |
| **Retention / Expansion** | Mantiene i clienti, riduce il churn, aumenta l'ACV nel tempo | Churn rate, NRR, expansion MRR, NPS |

### Step 2 — Diagnosi del funnel attuale

Prima di scegliere dove investire, mappa lo stato attuale del funnel:

**Domande diagnostiche:**

1. "Quante persone nel vostro ICP sanno che esistete?" → misura Awareness gap
2. "Di chi vi conosce, quanti si impegnano attivamente (leggono il vostro contenuto, aprono le email, tornano sul sito)?" → misura Engagement gap
3. "Di chi si impegna, quanti convertono in lead/trial/demo?" → misura Conversion gap
4. "Di chi diventa cliente, quanti restano e crescono nel tempo?" → misura Retention gap

### Step 3 — Identificazione del bottleneck

Il lever da prioritizzare è quello dove c'è il bottleneck principale. Usa questa logica:

```
Se il problema è: "Nessuno sa chi siamo"
→ Lever 1 (Awareness) è il bottleneck

Se il problema è: "Le persone ci trovano ma non si interessano / non tornano"
→ Lever 2 (Engagement) è il bottleneck

Se il problema è: "Abbiamo molti lead ma pochi si convertono"
→ Lever 3 (Conversion) è il bottleneck

Se il problema è: "Acquistiamo clienti ma il churn è alto"
→ Lever 4 (Retention) è il bottleneck
```

**Regola di stage**: in fase seed, quasi sempre il bottleneck è Awareness + Conversion. Retention diventa critica dopo i primi 20-30 clienti. Engagement è spesso trascurato — ma è quello che differenzia i sistemi che scalano.

### Step 4 — Stack rank

Assegna una priorità 1-4 ai lever (1 = massima priorità). Poi per ogni lever, indica:
- **Effort attuale** (alto / medio / basso / zero)
- **Impatto potenziale** (alto / medio / basso)
- **Cambio consigliato** (aumentare / mantenere / ridurre / non fare)

### Step 5 — Implicazioni per il piano di marketing

Per il lever prioritario (rank 1), definisci:
1. **3 tattiche specifiche** che lo spostano
2. **KPI di riferimento** (metrica principale + target a 90 giorni)
3. **Segnale che indica che il lever è stato risolto** (quando smettere di prioritizzarlo)

### Step 6 — Output

```
Funnel diagnostics:
- Awareness: [stato attuale]
- Engagement: [stato attuale]
- Conversion: [stato attuale]
- Retention: [stato attuale]

Bottleneck principale: [Lever X]

Stack rank:
1. [Lever] — perché ora — tattiche: [A, B, C] — KPI: [metrica + target]
2. [Lever] — mantenere con sforzo limitato
3. [Lever] — secondario
4. [Lever] — non prioritario per questo trimestre

Segnale di risoluzione bottleneck: [quando si passa al lever successivo]
```

Salva in `outputs/YYYY-MM-DD-revenue-levers-[cliente].md`.
Aggiorna `kpi/dashboard.md` con i KPI del lever prioritario come metriche primarie del trimestre.

---

## Troubleshooting

**"Tutti i lever sono importanti"**: è vero, ma non tutti sono ugualmente bloccanti. Chiedi "se dovessi scegliere UNO e solo uno su cui lavorare nei prossimi 90 giorni, quale sposterebbe più il revenue?" — questo scioglie il blocco.

**Il cliente vuole fare Awareness ma il vero problema è la Conversion**: succede spesso. Mostra i dati: se hanno già traffico e lead ma bassa conversion, l'awareness aggiuntiva non risolve niente. Il numero è il modo più rapido per convincere.
