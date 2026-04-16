---
name: saas-homepage-analyzer
description: Expert system for creating and evaluating B2B SaaS homepages. Use when: (1) user provides product/market/audience/problem material and wants homepage strategy (anchor choice, positioning, UVP, structure, copy drafts); (2) user shares a homepage URL, screenshot, copy or description and wants structured critical analysis with improvement recommendations. Triggers: "analizza questa homepage", "crea la homepage", "che anchor usare", "valuta questa pagina", "aiutami con il posizionamento della homepage", "scrivi il copy per la homepage", "cosa non va in questa homepage".
metadata:
  author: Custom
  version: 1.0.0
  category: marketing
---

# SaaS Homepage Analyzer

Sistema esperto per creare e valutare homepage B2B SaaS. Opera in due modalità distinte.

---

## Modalità 1 — Creazione (Materiale grezzo → Homepage)

Attiva quando l'utente fornisce materiale su prodotto, target, problema, competitor, mercato, stage.

### Step 1: Analizza il Contesto

Leggi tutto il materiale fornito. Estrai:
- Chi è il buyer (ruolo, tipo azienda, situazione)
- Quale problema risolve il prodotto
- Come il buyer risolve oggi il problema (status quo / current way)
- Che livello di awareness ha il mercato sulla categoria
- Che stage è la startup

Consulta `references/strategy-frameworks.md` → sezione "ICP e Situation Mapping".

Se mancano informazioni critiche, fai domande mirate prima di procedere.

### Step 2: Scegli l'Anchor

Applica l'albero decisionale in `references/anchor-decision-tree.md` nell'ordine esatto:
1. Step 0: Esiste un leader dominante con mindshare? → **Competitive Alternative**
2. Step 1: Il buyer cerca per categoria su G2/Capterra? → **Product Category**
3. Step 2: Il buyer sa articolare il problema ma non cerca software? → **Use Case**
4. Step 3: La soluzione dominante è ancora manuale (Excel, email)? → **Activity**

Dichiara esplicitamente quale anchor hai scelto e perché, citando gli elementi del materiale che giustificano la scelta.

### Step 3: Costruisci il Value Proposition Canvas

Consulta `references/strategy-frameworks.md` → sezione "VP Canvas".

- Anchor = Competitive Alternative → **VP Canvas Competitive** (righe = alternative competitor)
- Anchor = Use Case / Activity → **VP Canvas Contextual** (righe = sotto-fasi del use case)
- Anchor = Product Category → **VP Canvas Competitive** (righe = cluster competitor nella categoria)

Compila il canvas con il materiale fornito. Le 8 colonne:
`Persona → Company Type → Use Case → Current Tool → Problem → Capability → Feature → Desired Outcome`

### Step 4: Scegli la Struttura

Consulta `references/homepage-structures.md` → matrice di decisione.

Regola rapida:
- Pre-Seed/Seed + bassa awareness → **MVW** (3 blocchi)
- Seed/Early Stage + media awareness → **Classic** (6 blocchi)
- Growth + alta awareness + categoria nota → **Perfect SaaS** (10 sezioni)

Giustifica la scelta in base a stage e anchor.

### Step 5: Mappa Canvas → Copy

Usa `references/canvas-to-copy.md` per tradurre le celle del canvas in elementi homepage:
- Riga 1 del canvas → Hero Section (H1, subheadline, social proof tagline)
- Current Way + Limitations + Problems → Problem Section (3 colonne di agitazione)
- Primary Capability + Feature + Benefit → Solution Intro
- Righe 2-4 capabilities → Value Propositions 1-3

Consulta `references/section-variants.md` per scegliere il layout giusto per ogni sezione in base all'anchor.

### Step 6: Produci l'Output

Fornisci nell'ordine:
1. **Anchor scelto** + motivazione (2-3 frasi)
2. **VP Canvas compilato** (tabella markdown)
3. **Struttura consigliata** + motivazione
4. **Bozza copy** per ogni sezione: H1, H2/subheadline, body copy, CTA
5. **Note design** per ogni sezione: layout consigliato, elementi visivi, trust signals

---

## Modalità 2 — Analisi (Homepage → Diagnosi critica)

Attiva quando l'utente fornisce URL, screenshot, copy descrittivo di una homepage (intera o parziale).

### Step 1: Raccogli il Contesto

Se non fornito, chiedi prima di analizzare:
- Stage della startup
- ICP target (chi compra, che ruolo, che tipo azienda)
- Anchor inteso (se lo sa)
- Principale competitor o alternativa che vogliono battere

### Step 2: Identifica l'Anchor Attuale

Analizza la homepage e determina quale anchor sta usando. Applica il percorso inverso:
- La hero dichiara una categoria → Product Category
- La hero attacca un leader noto → Competitive Alternative
- La hero parla di un job-to-be-done → Use Case
- La hero parla di un'attività manuale da eliminare → Activity
- Non è chiaro → mancanza di anchor = problema primario

### Step 3: Verifica Coerenza Strategica

Consulta `references/errors-by-anchor.md`:
- L'anchor scelto è giustificato dal contesto (stage, awareness del mercato)?
- Il copy di ogni sezione è coerente con l'anchor scelto?
- Ci sono mismatch tra sezioni (es. hero da use case, capabilities da category)?

### Step 4: Analisi Sezione per Sezione

Usa la rubrica in `references/evaluation-grid.md`. Per ogni sezione presente valuta:
- Cosa funziona e perché
- Cosa non funziona e perché
- Come correggere con esempio di copy alternativo

### Step 5: Verifica Errori Comuni

Consulta `references/common-mistakes.md` per la checklist finale di clarity e struttura.

### Step 6: Produci la Diagnosi

Struttura l'output così:
1. **Anchor identificato** — è quello giusto per il contesto?
2. **Score per sezione** (✅ funziona / 🆗 migliorabile / ❌ non funziona)
3. **Analisi dettagliata** sezione per sezione con motivazione
4. **Top 3 priorità di intervento** — cosa correggere prima e perché
5. **Copy alternativo** per le sezioni più critiche

---

## Note di Performance

- Non produrre output generici. Ogni raccomandazione deve essere specifica per il prodotto analizzato.
- Quando mancano informazioni, fai domande mirate invece di assumere.
- La qualità dell'analisi è più importante della completezza formale.
- Se la homepage ha problemi strategici (anchor sbagliato), segnalalo prima dei problemi tattici (copy debole).
- Sempre distinguere problemi di strategia da problemi di esecuzione.
