# Decision Tree — Come scegliere il Primary Anchor

## Regola cardinale

> **Scegli il Primary Anchor in base a come pensano i buyer OGGI, non come vorresti che pensassero.**

Non è una discussione strategica. Non è un workshop di branding. È diagnosi.

Applica le domande sotto **in ordine, top-to-bottom**. La prima risposta SÌ chiude la decisione. Se tutte le risposte sono NO, non scegliere un anchor — fai altra ricerca sul buyer.

---

## Step 0 — Leader Dominance Test

**Q0**: Esiste un leader di mercato dominante che:
- Quasi ogni buyer già conosce?
- Possiede la maggior parte del mindshare di categoria?
- Viene citato spontaneamente nelle conversazioni?
- È il punto di paragone automatico ("è come X")?

E tu hai **un wedge chiaro** contro questo leader? (cioè: sai dire in una frase perché un buyer dovrebbe scegliere te invece del leader?)

| Risposta | Decisione |
|---|---|
| **SÌ + wedge chiaro** | → **Competitive Alternative Positioning** |
| **NO** (leader non dominante, o nessun wedge) | → Vai a Step 1 |

**Nota importante su Competitive Alternative:**

Usalo SOLO quando:
- Un leader dominante esiste ED è conosciuto da quasi ogni buyer
- Puoi articolare un wedge chiaro

Evitalo se:
- Il leader non è widely known (se devi spiegare chi è, non è dominante)
- Non riesci ad articolare un wedge concreto (ti manca la differenziazione)

**Anche se scegli Competitive Alternative, valida poi la Category Awareness (Step 1).** Molti "leader" esistono dentro categorie che i buyer cercano. Se la categoria è consolidata, stai facendo sia Competitive Alternative che Product Category — scegli quella più forte per il tuo wedge.

---

## Step 1 — Category Awareness Test

**Q1**: Quando i buyer iniziano a valutare soluzioni, fanno queste cose?
- Cercano su Google una categoria software specifica?
- Confrontano vendor su G2 o Capterra?
- Chiedono demo a più fornitori della stessa categoria?

**Esempi di categorie note a cui applicare il test:**
- CRM software
- Scheduling software
- Product analytics software
- HR software

| Risposta | Decisione |
|---|---|
| **SÌ** (i buyer ragionano già per categoria) | → **Product Category Positioning** |
| **NO** | → Vai a Step 2 |

**Come verificarlo empiricamente:**
- Keyword research: c'è search volume per "[categoria] software"?
- G2/Capterra: esiste una categoria dedicata con 10+ vendor?
- Outreach: quando parli con prospect, ti chiedono di te con termini di categoria?
- Customer interviews: ti dicono "stiamo valutando [categoria]" o ti descrivono un problema?

Se trovi segnali forti in questi 4 canali, hai category awareness.

---

## Step 2 — Problem Articulation Test

**Q2**: I buyer sanno descrivere chiaramente cosa vogliono ottenere, anche se non sanno quale tipo di software lo risolve?

**Esempi:**
- *"Dobbiamo programmare i colloqui più velocemente"* (job: scheduling recruiting)
- *"Ci servono guide di onboarding migliori"* (job: digital adoption)
- *"Dobbiamo coordinare le approvazioni più facilmente"* (job: approval workflow)

| Risposta | Decisione |
|---|---|
| **SÌ** (articolano il JTBD, ma non la categoria) | → **Use Case Positioning** |
| **NO** | → Vai a Step 3 |

**Come verificarlo:**
- Customer interviews: il buyer descrive un problema operativo specifico, ma non sa che esiste un software che lo risolve.
- Quando li chiedi "Come cercheresti una soluzione?", rispondono con problem-language, non con category-language.
- Esempi: "Dovrei chiedere in giro", "Google non sa cosa cercare", "Non esiste niente del genere".

---

## Step 3 — Manual Behavior Test

**Q3**: La soluzione dominante è ancora manuale? Quando parli con potenziali clienti, ti dicono cose come:
- *"Usiamo Excel / fogli di calcolo"*
- *"Lo gestiamo su Slack / email"*
- *"Non abbiamo uno strumento per questo"*

| Risposta | Decisione |
|---|---|
| **SÌ** | → **Activity Positioning** |
| **NO** | → Ferma. Rivaluta la comprensione del mercato. |

Se nessuno dei 4 step produce un SÌ, vuol dire che:
- Non capisci ancora abbastanza il buyer
- O il buyer ha comportamenti fragmentati (alcuni manuali, alcuni con software, alcuni con alternative)

In entrambi i casi, fai più discovery prima di scegliere.

---

## Flow visuale

```
START
  │
  ▼
Q0: Leader dominante + wedge chiaro?
  ├─ SÌ ──→ COMPETITIVE ALTERNATIVE
  └─ NO ─┐
         ▼
  Q1: Category awareness (G2, search, demo)?
  ├─ SÌ ──→ PRODUCT CATEGORY
  └─ NO ─┐
         ▼
  Q2: Buyer articola JTBD ma non categoria?
  ├─ SÌ ──→ USE CASE
  └─ NO ─┐
         ▼
  Q3: Dominant solution è manuale (Excel/Slack)?
  ├─ SÌ ──→ ACTIVITY
  └─ NO ──→ Re-evaluate (need more buyer research)
```

---

## Common Mistakes nel decision tree

### Mistake 1: Saltare lo Step 0 e andare direttamente a Product Category
Molti founder scelgono Product Category perché "è più semplice". Ma se esiste un leader dominante, la scelta giusta è quasi sempre Competitive Alternative — perché il buyer ragiona "come Leader ma con wedge".

### Mistake 2: Forzare un SÌ allo Step 1 quando non c'è vera category awareness
Se il search volume è basso e G2 non ha categoria, Product Category non funziona. Meglio Use Case. Aspettare che il mercato maturi non è un'opzione passiva — è una strategia attiva (Use Case ti permette di educare).

### Mistake 3: Confondere Use Case con Activity
- **Use Case**: il buyer sa articolare il problema operativo. C'è consapevolezza che "questa cosa va migliorata".
- **Activity**: il buyer non vede nemmeno il problema come problema. "Io faccio così, funziona, qual è il punto?".

Il test: se il buyer, messo davanti a un before/after visual, dice *"wow, non avevo idea di quanto tempo sprecavo"* → Activity. Se invece dice *"sì, è un casino, sto cercando una soluzione"* → Use Case.

### Mistake 4: Scegliere Competitive Alternative quando il leader non è davvero dominante
Segnale: se devi spiegare al buyer chi è il leader, non è dominante. Se il leader ha il 10% del mercato e non è conosciuto fuori dal tuo bubble, non è un anchor utile.

### Mistake 5: Non rivalutare il decision tree quando il mercato evolve
Il positioning può maturare nel tempo: Activity → Use Case → Product Category. Rifai il test ogni 6-12 mesi se sei in una categoria emergente.

---

## Un'euristica extra (non in Estner) — il "Google test"

Prova a cercare questi 3 pattern su Google:
1. `[nome del tuo prodotto]` — chi appare? Tu e chi altro?
2. `[categoria che vuoi occupare] software` — c'è search volume, o il keyword planner dice zero?
3. `[leader] alternative` — c'è search volume, o è vuoto?

- Se 2 ha volume + 3 ha volume → Product Category o Competitive Alternative, sei nella fase matura
- Se 2 ha poco volume + 3 ha volume → Competitive Alternative (il buyer conosce solo il leader)
- Se 2 ha zero volume + 3 ha zero volume → Use Case o Activity (stai educando il mercato)

Questo test non sostituisce il decision tree ma lo valida con evidenza esterna.
