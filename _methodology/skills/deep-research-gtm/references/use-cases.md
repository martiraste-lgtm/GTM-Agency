# GTM Use-Case Playbooks

Due pattern coperti come playbook completi (i due che sono il mestiere del collettivo), con scaffold di prompt, regole di source-priority e shape del deliverable. Più una nota sui pattern coperti altrove e il source-priority ladder generale.

---

## 1. Playbook di progetto interno

**Quando:** serve eseguire un grande progetto GTM mai fatto prima — marketing attribution, lead scoring, territory design, onboarding flow, comp plan, migrazione tool, processi di GTM planning. Utile anche per costruire i processi *del collettivo stesso*.

**Research questions:**
- Quali sono i work stream / le decisioni principali da prendere?
- Quali approcci esistono per ciascuno, e quali sono i trade-off?
- Qual è il percorso consigliato per la situazione specifica di questa azienda?
- Come si presenta concretamente l'esecuzione step-by-step?

**Source priority:**
1. Blog di practitioner e contenuti op-ex di leader GTM (primary)
2. Documentazione dei tool nello stack del committente
3. Talk di conferenze, podcast di operator che l'hanno spedito
4. Evitare: contenuto SEO generico "cos'è X", marketing dei vendor travestito da thought leadership

**Deliverable:**
- Overview delle decisioni chiave + work stream
- Per ogni work stream: opzioni confrontate in tabella, raccomandazione, step-by-step del percorso consigliato
- Artefatti concreti dove rilevante (SQL mock, convenzioni UTM, spec oggetti Salesforce, formule di comp)

**Scaffold:**
```
<goal>
Metti insieme una guida tattica e approfondita su come costruire [X] in-house.
La guida deve aiutare un team con conoscenza operativa dei tool rilevanti
ma zero esperienza pregressa con [X] ad arrivare a un'implementazione v1.
</goal>

<context>
[Stage azienda, ARR, motion, stack, geografia]
[Vincoli — dimensione team, timeline, tool che devono tenere / non possono comprare]
</context>

<structure>
1. Overview delle decisioni chiave e dei work stream principali
2. Per ogni work stream: tabella opzioni, raccomandazione, step-by-step dettagliato
3. Artefatti concreti dove rilevante (es. snippet SQL, convenzioni di naming)
</structure>

<style>
Pyramid Principle. Prima le raccomandazioni, poi le evidenze.
Tabelle e bullet dove battono la prosa. Summary in cima a ogni sezione.
</style>
```

---

## 2. Teardown competitor (positioning / ads / GTM motion)

**Quando:** vuoi capire come un competitor si posiziona, messaggia, fa ads o va a mercato. Per il collettivo: alimenta `context/competitor-radar.md` e la battlecard di `playbooks/competitor-switch.md`.

**Research questions:**
- Come si posizionano (core promise, differenziatori, categoria)?
- Chi targettano (persona, segmenti, dimensioni azienda)?
- Quali canali/tattiche usano e che aspetto hanno le creatività?
- Quali offer e CTA funzionano per loro?
- Quali segnali indicano shift di strategia?

**Source priority:**
1. Sito proprio del competitor — homepage, pricing, pagine prodotto, blog, careers (primary)
2. Ad library — LinkedIn Ads Library, Meta Ad Library, Google Ads Transparency
3. Loro contenuto recente — annunci, comunicati, apparizioni podcast
4. Review site (G2, TrustRadius) per il gap posizionamento vs realtà
5. Evitare: pagine SEO "alternative a X" di terzi, vecchi post comparativi

**Deliverable:**
- Sintesi posizionamento (un paragrafo)
- Persona / ICP target (con evidenza)
- Pilastri di messaggio con quote dirette
- Strategia di canale con esempi concreti (link a ads, post)
- Pattern di offer/CTA
- Screenshot o link a ~20 esempi concreti

**Orchestrazione — hand-off alle skill specializzate (importante):**
Il teardown produce la lettura GTM d'insieme. Quando una dimensione richiede profondità, **non rifarla qui a metà: passa la palla** e poi reincorpora il risultato nel report (sezione dedicata + citazione).

| Dimensione del competitor da approfondire | Hand-off a |
|---|---|
| Homepage / landing / pricing page (audit sezione per sezione) | `saas-homepage-analyzer` (Modo B — analisi) |
| Headline / H1 della loro hero | `b2b-h1-writer` (valutazione) |
| Confronto feature testa a testa noi-vs-loro / compete page | `battlecard` / `pm-go-to-market-competitive-battlecard` |
| Deconstruzione del loro positioning (5-step) | `b2b-positioning-diagnostic` o `positioning-framework-estner` |
| Dimensione mercato/categoria che presidiano | `pm-market-research-market-sizing` |

Regola pratica: nel research plan (Step 3) dichiara quali hand-off prevedi. Se il committente chiede "analizza il competitor X" in modo aperto, **proponi tu** quali di queste viste approfondire, non darle tutte per scontate. L'output finale resta un unico report a piramide: le analisi delegate diventano sue sezioni, non documenti separati.

**Scaffold (ads-specific):**
```
<goal>
Capire come [Azienda] usa le ads [LinkedIn / Google / Meta] per crescere.
Sfrutta l'ad library rilevante per costruire un report completo su
positioning, messaggio, targeting e tattiche.
</goal>

<context>
La pagina di dettaglio di ogni ad mostra formato, date di flight, impression
per regione e dettagli creativi. Usa tutto.
[Contesto della nostra azienda se vogliamo insight tarati]
</context>

<content>
Copri almeno:
- Formati ad (single image, video, message, document) e tipi (case study, thought leadership, demo offer)
- Buyer persona e segmenti targettati
- Positioning e pilastri di messaggio
- Pattern di CTA e offer / incentivi
Linka inline a 20+ esempi specifici di ads.
</content>

<instructions>
Rivedi 50+ ads prima di scrivere. Punta a ~3.000 parole.
</instructions>
```

---

## Pattern coperti altrove (non duplicare qui)

Questi tre pattern del playbook originale Deep Research **non** sono coperti come playbook dedicati: hanno già skill globali. Usa quelle. La *metodologia* di questa skill (source ladder, plan-first, piramide) si applica comunque come wrapper di rigore.

| Pattern | Skill da usare |
|---|---|
| Page/site audit (homepage, pricing, signup flow) | `saas-homepage-analyzer` (+ `b2b-h1-writer` per le headline) |
| Feature comparison / compete page | `battlecard` / `pm-go-to-market-competitive-battlecard` (+ `pm-market-research-competitor-analysis`) |
| Market / espansione (TAM-SAM-SOM, ranking mercati) | `pm-go-to-market-beachhead-segment` + `pm-market-research-market-sizing` + `pm-product-strategy-ansoff-matrix` |

---

## Quick reference: source-priority ladder

In ordine grezzo di credibilità per la maggior parte dei task di ricerca GTM:

1. **Dati primari:** sito/docs propri dell'azienda, ad library, dati di bureau statistici/governativi, il prodotto stesso
2. **Contenuto di practitioner:** blog, podcast, talk di operator che l'hanno fatto
3. **Research org:** Gartner, Forrester, IDC (credibili ma spesso a pagamento e a volte stantii)
4. **Aggregatori di review:** G2, TrustRadius (per sentiment, non per la verità sulle feature)
5. **News / press:** utili per eventi e timing, meno per l'analisi
6. **Contenuto SEO generico:** "Top 10 tips for X" — di solito si salta
7. **Post social:** utili per pulse check e voce reale degli utenti, non per i claim
