# Formule e Template — Framework OKR Ibrido

## Sintassi Rapida per i Commitments (da Ravi Mehta, adattata)

```
KPI [direzione] (baseline) target [deadline] [persona] [Leading/Lagging] [Frontier Stage]
```

### Simboli Direzione
- `>` deve crescere
- `><` deve rimanere entro una soglia
- `<` deve ridursi
- nessun simbolo = deve essere fatto (binario)

### Esempi con sintassi rapida

**Crescita**:
`MAU > (100K) 250K entro fine Q1 [Growth Manager] [Leading][Execution]`

**Soglia**:
`CAC >< (€10) €25 entro fine Q3 [CMO] [Lagging][Strategic]`

**Riduzione**:
`Burn rate mensile < (€710K) €550K entro fine Q4 [CFO] [Lagging][Strategic]`

**Binario**:
`Nuovo onboarding flow disponibile nella release di novembre [CPO] [Leading][Execution]`

---

## Template Documento OKR Completo

```
CICLO: [Q1/Q2/Q3/Q4 ANNO]
LIVELLO: [Company / BU: nome / Team: nome / Individuale: nome]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

NARRATIVE
[2-4 frasi che coprono: cosa + WHY + WHY NOW + fit strategico]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

OBJECTIVE
[Verbo + area + deadline + persona]

WHY: [ragionamento causale]
WHY NOW: [perché questo ciclo e non il prossimo]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

HEALTH METRICS (guardrail — non traguardi)
- [Metrica 1] deve rimanere [≥/≤] [soglia] per tutto il ciclo
- [Metrica 2] deve rimanere [≥/≤] [soglia] per tutto il ciclo
- [Metrica 3 — opzionale]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

COMMITMENTS (100% target)

C1 [Leading][Frontier Stage]:
[KPI] [direzione] ([baseline]) → [target] entro [deadline] [persona]

C2 [Lagging][Frontier Stage]:
[KPI] [direzione] ([baseline]) → [target] entro [deadline] [persona]

C3 [Leading/Lagging][Frontier Stage]:
[descrizione — può essere deliverable se Frontier Stage è Dependency/Execution]

[C4 — Moonshot opzionale, 60-70% target]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

INITIATIVES (per ogni Commitment)

→ C1:
- [Iniziativa A] → ipotesi: [meccanismo causale]
- [Iniziativa B] → ipotesi: [meccanismo causale]

→ C2:
- [Iniziativa C] → ipotesi: [meccanismo causale]

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

TASKS — WARM START (fluide, possono cambiare)

→ Iniziativa A:
- [Task 1]
- [Task 2]
- [Task 3]

→ Iniziativa B:
- [Task 1]
- [Task 2]
```

---

## Template Narrative

**Struttura in 4 elementi:**

```
[COSA il team vuole ottenere in questo ciclo].
[WHY NOW — perché è prioritario adesso, non in un altro momento].
[LEARNING RECENTE che ha informato questa priorità].
[FIT STRATEGICO — come si inserisce nella strategia annuale o Company vision].
```

**Esempio con placeholder:**
"Il team [X] punta a [obiettivo] nel [ciclo] perché [ragione strutturale — metrica, trend, gap]. [Dato o insight recente] mostra che [evidenza che supporta la priorità]. Priorità adesso perché [trigger temporale specifico — lancio, risorsa disponibile, finestra di mercato, scadenza]. Questo contribuisce a [strategic goal annuale] attraverso [meccanismo causale]."

---

## Template Health Metrics

**Categorie di guardrail da considerare:**

| Area | Esempi di Health Metric |
|------|------------------------|
| Profittabilità | CAC, margine operativo, burn rate |
| Customer experience | NPS, CSAT, tasso di churn |
| Qualità prodotto | Bug critici aperti, uptime, tempo di risposta |
| Team | Utilizzo capacità (evitare overload), velocità sprint |
| Brand/retention | Unsubscribe rate, engagement rate |

---

## Template Weighting Matrix (multi-team)

Usare quando si devono allineare più team agli stessi Company Objectives.

```
                    | Sales | Marketing | Product | CS | Ops |
--------------------|-------|-----------|---------|-----|-----|
[Company Obj 1]     |   5   |     4     |    3    |  4  |  3  |
[Company Obj 2]     |   2   |     5     |    1    |  3  |  2  |
[Company Obj 3]     |   0   |     1     |    0    |  0  |  5  |
[Company Obj 4]     |   2   |     4     |    5    |  5  |  0  |
```

**Punteggio 0-5**: impatto del Core Process su quel Company Objective.
- 4-5 = nodo critico → costruire OKR specifici per quella combinazione
- 2-3 = contributo parziale → allineare senza OKR dedicati
- 0-1 = bassa rilevanza → non serve OKR

---

## Template One Page (visione d'insieme)

```
AZIENDA: [nome] | ANNO: [anno]

┌─────────────────────────────────────────────────────────┐
│ CORE VALUES              │ UNIQUE VALUE PROPOSITION      │
│ [valore 1]               │ [promessa al cliente]         │
│ [valore 2]               │                               │
│ [valore 3]               │                               │
├─────────────────────────────────────────────────────────┤
│              20-YEAR COMPANY GOAL                        │
│ [visione a lungo termine che ispira e orienta]           │
├─────────────────────────────────────────────────────────┤
│ 3-YEAR COMPANY GOAL      │ ANNUAL STRATEGIC GOALS        │
│ [obiettivi 3 anni con    │ [3-5 priorità annuali         │
│  numeri grezzi]          │  da cui derivano gli OKR]     │
├─────────────────────────────────────────────────────────┤
│              OKR TRIMESTRALE CORRENTE                    │
│ Narrative: [sintesi]                                     │
│ Objective: [formula]                                     │
│ C1 [Leading]: [target]                                   │
│ C2 [Lagging]: [target]                                   │
└─────────────────────────────────────────────────────────┘
```

---

## Reverse Engineering — Template di Calcolo

Per verificare la fattibilità di un Commitment, scomponi il target in numeri giornalieri/settimanali.

**Esempio (Sales)**:
```
Target: chiudere 200K€ di nuove revenue in Q1

Assunzioni:
- ACV = €10.000
- Win rate = 30%
- Discovery-to-demo conversion = 50%
- Outbound contact rate = 5%
- Sales cycle = 1 mese

Calcolo a ritroso:
1. Deal da chiudere: 200K / 10K = 20 deal
2. Opportunità in pipeline: 20 / 30% = 67 opportunità
3. Discovery call: 67 / 50% = 134 call
4. Lead da contattare: 134 / 5% = 2.680 lead
5. Per settimana (13 settimane): 206 lead/settimana
6. Per giorno: 41 lead/giorno
```

Se il numero giornaliero non è operativamente raggiungibile, il Commitment è mal calibrato. Abbassa il target o aggiungi risorse.
