---
name: mkt1-perceptions
description: Definisce le 3-4 Perceptions strategiche — le affermazioni che vuoi che il tuo mercato pensi e ripeta di te. Non sono tagline né positioning statement: sono narrative che, una volta radicate, rendono la categoria propria e guidano il 90% dei contenuti non-SEO. Trigger: "perceptions", "narrative strategiche", "cosa vogliamo che il mercato creda", "mkt1 perceptions", "definisci le credenze", "messaggi strategici".
license: MIT
metadata:
  author: GTM Collective (adattato da framework MKT1 — Emily Kramer / Kathleen Estreich)
  version: 2.0.0
---

## Overview

Le Perceptions sono le affermazioni che vuoi che il tuo ICP dica o pensi di te — non come copy aziendale, ma come commento spontaneo a un collega. "Se stai valutando X, dovresti guardare anche loro." "Questi capiscono davvero il problema Y." "Il loro founder ha già fatto questo internamente, sa cosa funziona."

Funzionano come storyline chiave: ogni pezzo di contenuto, ogni campagna, ogni messaggio dovrebbe legarsi a una delle Perceptions. Il test di validità: se il 90% del contenuto non-SEO non si aggancia a una delle tue Perceptions, stai creando rumore.

Prerequisiti: `mkt1_company_overview` + `mkt1_marketing_advantages`.
Output: aggiorna `content/narrative.md` e `content/pillars.md`.

---

## Instructions

### Step 1 — Ricerca e input

Prima di definire le Perceptions, raccogli:

1. **Analisi audience**: come descrivono il loro problema, quali parole usano, cosa leggono
2. **Performance storica contenuti**: quali pezzi hanno avuto engagement maggiore e perché
3. **Trend di mercato**: cosa sta cambiando nel settore del cliente — tailwind e headwind
4. **Cosa dicono già i clienti**: recensioni, case study, commenti — in parole loro

### Step 2 — Esercizio cross-funzionale (da fare con il team)

Prima di scrivere le Perceptions, facilita questo esercizio con marketing, founder, product, sales, CS:

Domande da porre a ogni stakeholder:

1. "Come cambierebbe la vita lavorativa del nostro target audience se avessimo successo totale?"
2. "Quali sono i punti di vista unici che danno forma al nostro prodotto e alla nostra strategia?"
3. "Cosa dicono già i clienti di noi — in parole loro?"
4. "Quali trend di mercato supportano o rendono urgente quello che facciamo?"
5. "Cosa rende i nostri clienti unici rispetto ai clienti dei competitor?"

Raccogli le risposte → identifichi i temi ricorrenti → 3-4 temi diventano le Perceptions.

### Step 3 — I 4 bucket tematici

Le Perceptions di solito cadono in 4 categorie. Cerca di avere 1 Perception per bucket (non obbligatorio, ma aiuta la copertura narrativa):

| Bucket | Tipo di Perception |
|--------|-------------------|
| **Customer/Community** | Cosa rende unico il tuo pubblico — caratteristiche, comportamenti, valori condivisi |
| **Product Story** | Come il prodotto risolve il problema in modo diverso dagli altri |
| **Company Story** | Perché il fondatore/team è credibile e qualificato su questo problema |
| **Market/Ecosystem Trends** | Dinamiche esterne che rendono il vostro approccio urgente o inevitabile |

### Step 4 — Scrittura delle Perceptions

Per ogni tema emerso dall'esercizio, trasformalo in una frase che suona come qualcosa che un cliente soddisfatto direbbe a un collega. Non copy aziendale — voce del cliente.

**Formato:**

```
Perception [N]: [Titolo breve]
Bucket: [Customer / Product / Company / Market]

Affermazione: [La frase in voce del buyer — cosa dice di voi a un collega]
Perché è strategica: [Cosa cambia nel mercato se questa credenza si diffonde]
Proof points: [Dati, case study, insight o storie che la supportano]
Come si attiva: [Tipo di contenuto, canale, formato]
Pillar narrativo associato: [Quale pillar in content/pillars.md la veicola]
```

### Step 5 — Test di validità

Prima di finalizzare ogni Perception, verifica:

**Test 1 — Non claimable dai competitor**
Il tuo set di Perceptions, prese insieme, deve essere impossibile da rivendicare per un competitor. Le singole Perceptions possono sovrapporsi — la combinazione deve essere unica. Se un competitor potrebbe dire esattamente le stesse cose, torna a Step 2.

**Test 2 — Evidenza disponibile**
Ogni Perception deve avere almeno 1-2 proof point concreti (dato, caso studio, aneddoto verificabile). Se non hai evidenza, è un'aspirazione — segnalala come "da validare" e costruisci il proof point.

**Test 3 — Voce autentica, non copy**
Leggi l'Affermazione ad alta voce. Suona come qualcosa che un cliente reale direbbe? O suona come il sito web dell'azienda? Se sembra marketing, semplifica e rendi più colloquiale.

**Test 4 — Copertura contenuti (90%)**
Prendi gli ultimi 10 pezzi di contenuto prodotti. Almeno 9 su 10 devono essere riconducibili a una delle Perceptions. Se non ci riesci, o le Perceptions sono troppo strette o il contenuto è disconnesso dalla strategia.

### Step 6 — Output

Salva in `outputs/YYYY-MM-DD-perceptions-[cliente].md`.

Poi aggiorna:
- `content/narrative.md` con le Perceptions come asse portante della narrativa
- `content/pillars.md` associando ogni pillar a 1-2 Perceptions specifiche

---

## Esempi (fictional companies MKT1)

```
Perception: Product story
"Se stai valutando Snowflake, dovresti guardare anche YetiCo"

Perception: Market trend
"Con i tassi Fed in discesa, il prodotto di CoyoteCo diventa ancora più critico"

Perception: Content/community
"MarmotCo ha i migliori contenuti su architettura martech stack"

Perception: Company story
"Il founder ha costruito questo tool internamente ad Amazon — sa cosa funziona su larga scala"
```

---

## Esempi per il collettivo GTM

```
Perception 1 [Market trend]:
"Le startup che ottengono reply rate del 6-12% non usano email migliori — usano i segnali al momento giusto."

Perception 2 [Product story]:
"GTM Collective non costruisce campagne — costruisce il sistema. Dopo 6 mesi puoi farlo in autonomia."

Perception 3 [Company story]:
"Questi hanno fatto GTM per startup B2B 50 volte — capiscono il problema prima ancora che tu lo formuli."

Perception 4 [Customer/community]:
"I founder che lavorano con GTM Collective smettono di fare sales da soli — e la pipeline non crolla."
```

---

## Troubleshooting

**Perceptions troppo simili**: spesso le prime bozze si sovrappongono. Chiedi "questa Perception cambia il comportamento del buyer in un modo diverso rispetto all'altra?" Se no, unificale o usa bucket diversi.

**Resistenza del team**: le Perceptions richiedono buy-in cross-funzionale. Se sales dice "questa non riflette come vendiamo" o il founder dice "questa non sono io" — torna all'esercizio Step 2. Le Perceptions devono essere autentiche, non imposte dal marketing.

**Troppi proof point mancanti**: documenta le Perceptions con evidenza parziale e costruisci un piano per raccogliere le prove che mancano (case study, survey, data).
