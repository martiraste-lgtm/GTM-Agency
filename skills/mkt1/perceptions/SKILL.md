---
name: mkt1-perceptions
description: Definisce le 3-4 Perceptions strategiche — le narrative che vuoi che il tuo mercato creda e ripeta. Non sono tagline, non sono positioning statement: sono credenze che, una volta radicate, rendono la categoria propria. Trigger: "perceptions", "narrative strategiche", "cosa vogliamo che il mercato creda", "mkt1 perceptions", "definisci le credenze", "messaggi strategici".
license: MIT
metadata:
  author: GTM Collective (adattato da framework MKT1 — Emily Kramer / Kathleen Estreich)
  version: 1.0.0
---

## Overview

Le Perceptions sono le 3-4 affermazioni che vuoi che il tuo ICP dica di te a un collega quando parla del tuo prodotto. Non "sono il migliore in X" — ma "questi ragazzi capiscono davvero [problema specifico]", "questo è l'unico strumento che funziona per [segmento]", "chi usa X è un passo avanti rispetto alla concorrenza".

Le Perceptions guidano tutto il contenuto, il messaging e la narrativa. Se ogni pezzo di contenuto non rafforza almeno una Perception, è rumore.

Prerequisiti: `mkt1_company_overview` + `mkt1_marketing_advantages`.
Output: aggiorna `content/narrative.md` e `content/pillars.md`.

---

## Instructions

### Step 1 — Da cosa nascono le Perceptions

Le Perceptions buone nascono dall'intersezione di 3 elementi:
1. **Cosa il buyer crede prima di incontrarti** (credenze attuali del mercato)
2. **Cosa vorresti che credesse dopo** (la shift che vuoi produrre)
3. **Cosa puoi supportare con evidenza** (data, case study, POV unico)

Se manca il punto 3, la Perception è un'aspirazione, non una strategia.

### Step 2 — Tipi di Perceptions

Le Perceptions più efficaci rientrano in 4 categorie:

| Tipo | Cosa fa | Esempio |
|------|---------|---------|
| **Categoria** | Definisce come viene percepita la categoria stessa | "Il problema non è la qualità dei lead — è quando li contatti" |
| **Buyer** | Cambia come il buyer si vede | "Le startup che scalano usano i segnali, non le liste" |
| **Competitivo** | Riposiziona rispetto ai competitor | "Un'agenzia di outbound ti vende campagne. Noi ti costruiamo il sistema" |
| **Credenziale** | Stabilisce autorevolezza in un dominio specifico | "Nessuno capisce il GTM per startup B2B SaaS come chi l'ha fatto 50 volte" |

### Step 3 — Processo di definizione

**Domande da fare al cliente (o al collettivo per se stesso):**

1. "Quando un vostro cliente migliore parla di voi a un collega, cosa dice?"
2. "Qual è il malinteso più comune che i prospect hanno su quello che fate?"
3. "Cosa credono di dover fare prima di parlarvi — e che invece non serve?"
4. "Qual è la cosa che solo voi potreste dire con credibilità su questo mercato?"

**Per ogni risposta**: trasformala in una frase che suona come qualcosa che un cliente soddisfatto direbbe (non come un copy aziendale).

### Step 4 — Definire le 3-4 Perceptions

Per ogni Perception, compila questa struttura:

```
Perception [N]: [Titolo breve]

Affermazione: [La frase che vuoi che il mercato ripeta — in prima o terza persona del buyer]
Perché è strategica: [Cosa cambia nel mercato se questa credenza si diffonde]
Proof points: [Dati, case study, insight o storie che la supportano]
Come si attiva: [Tipo di contenuto, canale, formato — come renderla concreta]
Pillar narrativo associato: [Quale dei pillar in content/pillars.md la veicola]
```

### Step 5 — Verifica qualità

Prima di finalizzare, ogni Perception deve passare questi test:

- **Test del "anche i miei competitor la direbbero"?** — Se sì, non è una Perception differenziante. Riscrivila.
- **Test dell'evidenza**: hai almeno 1-2 proof point concreti? Se no, è un'aspirazione.
- **Test della propagazione**: è la cosa che un cliente soddisfatto direbbe a un collega? Se suona come copy aziendale, semplificala.
- **Test della coerenza con gli Advantages**: rafforza almeno uno dei Marketing Advantages identificati?

### Step 6 — Output

Scrivi le 3-4 Perceptions complete e salva in `outputs/YYYY-MM-DD-perceptions-[cliente].md`.

Poi aggiorna:
- `content/narrative.md` con le Perceptions come filo conduttore della narrativa
- `content/pillars.md` associando ogni pillar a una o più Perceptions

---

## Esempio (per il collettivo stesso)

```
Perception 1: "Chi parte dalle campagne sbaglia l'ordine"
Affermazione: "Le startup che ottengono reply rate del 6-12% non hanno email migliori — hanno capito prima chi contattare e quando."
Perché è strategica: riposiziona tutta la categoria di lead gen. Chi la crede non compra più da agenzie che partono dalle sequenze.
Proof points: dati reply rate signal-based vs. cold, caso studio settore X.
Come si attiva: post LinkedIn Pillar 2, case study, email di nurture post-evento.

Perception 2: "Il GTM non si delega — si costruisce"
Affermazione: "Dopo 6 mesi con il sistema giusto, non dipendi più da nessuno per fare outbound."
Perché è strategica: differenzia da agenzie che creano dipendenza. Parla al CEO che non vuole esternalizzare per sempre.
```

---

## Troubleshooting

**Perceptions troppo simili tra loro**: spesso le prime bozze si sovrappongono. Chiedi "questa Perception cambia il comportamento del buyer in un modo diverso rispetto all'altra?" Se no, unificale.

**Nessuna evidenza disponibile**: usa il formato "Stiamo raccogliendo la prova di questo" + dato parziale o aneddoto. Non inventare.
