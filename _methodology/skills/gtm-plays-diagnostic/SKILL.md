---
name: gtm-plays-diagnostic
description: Fase diagnostica GTM — dato un cliente (o il collettivo stesso), decide QUALI plays/motion automatizzate ha senso attivare, prima di costruire qualsiasi campagna. Legge il context già popolato e produce 5-8 plays prioritizzati e opinati. Usare in onboarding dopo strategia/positioning e prima della prima campagna. Trigger: "quali plays per [cliente]", "che motion attiviamo per", "diagnosi GTM plays", "quali automazioni outbound hanno senso", "da dove partiamo con l'outbound per [cliente]", "gtm-plays-diagnostic". NON usare per costruire la singola campagna (usa signal-to-sequence + campaign-build) né per lo scoring dei segnali (usa signal-library).
license: MIT
metadata:
  author: GTM Collective (adattato da gtm-plays-brainstorm / Growth Unhinged)
  version: 1.0.0
---

## Overview

Questa è la **fase diagnostica** del metodo del collettivo: *capire prima, agire dopo*. Prima di scegliere segnali e sequenze, decide **quali plays GTM** ha senso attivare per uno specifico cliente — date la sua GTM motion, il suo stage e i segnali a cui ha realmente accesso.

Non è esecuzione. Produce una scommessa opinata: i 5-8 plays su cui concentrarsi adesso, e quali lasciare per dopo. I plays signal-based che escono da qui poi confluiscono nel sistema operativo del collettivo (`signal-library` → `signal-routing` → `campaign-build`).

**Posizione nel flusso**: onboarding cliente, **Step 4b** — dopo l'analisi strategica/positioning (Step 4), prima dell'infrastruttura e della prima campagna (Step 5-6). Vedi `workflows/client-onboarding.md`.

---

## Confine vs signal-library (leggere prima di iniziare)

Due risorse che sembrano simili ma operano a livelli diversi. Non confonderle:

| | **Questa skill (plays-library)** | **signal-library.md** |
|---|---|---|
| Livello | Strategico — *quale motion scegliere* | Operativo — *come eseguire l'outbound* |
| Quando | In onboarding, una volta per cliente | Ad ogni campagna, in continuo |
| Cosa dà | 5-8 plays prioritizzati per il cliente | Scoring, decay, hook, combinazioni dei segnali |
| Output | Diagnosi GTM | Lista scorata + sequenza |

In una frase: **questa skill decide COSA fare, la signal-library è COME lo fai.** I due si completano — non si sovrappongono.

---

## Guiding Principles

Questi principi guidano ogni raccomandazione. Interiorizzali prima di produrre output.

- **Signal-based batte cold.** Le campagne innescate da un segnale superano il cold outreach di 2x-10x. Priorità ai plays dove esiste un segnale chiaro e tempestivo. I migliori segnali sono spesso quelli che il cliente già genera ma non ha ancora operazionalizzato (engagement sui contenuti, dati prodotto, storico CRM).
- **Pochi contatti buoni vincono.** L'obiettivo dell'automazione è precisione, non volume. 50-250 contatti targettati con messaggio rilevante e tempestivo convertono molto più di 5.000 contatti generici.
- **Allinea i plays alla GTM motion.** Le aziende PLG hanno segnali di prodotto che le sales-led non hanno. Le sales-led possono fare plays cold che le PLG non dovrebbero prioritizzare. Filtra sempre attraverso la motion reale.
- **Parti da ciò che hanno già.** Prima i plays che usano dati esistenti (CRM, contenuti LinkedIn, storico closed-won), poi quelli che richiedono nuove acquisizioni di dati. La complessità va guadagnata.
- **Un-silo dei canali.** Il flywheel GTM: l'outbound targetta gli hand-raiser dei contenuti, i contenuti migliori diventano ads, gli ads rinforzano la lista outbound. Fai emergere i plays che connettono marketing, sales e prodotto.
- **Scala la complessità allo stage.** Early-stage: 1-2 plays ad alto segnale, falli funzionare. Growth: si stratificano i segnali. Scaling: signal stack completo e micro-campagne (50-250 contatti, molto specifiche, rinfrescate spesso).

---

## Modi d'uso

**Modo A (primario) — Diagnosi per un cliente.**
Quali plays attivare nel GTM di un cliente del collettivo. È l'uso in onboarding.

**Modo B (secondario) — Pressure-test dell'outbound del collettivo.**
Mettere alla prova il nostro outbound (noi → trovare clienti) contro la library, per scoprire plays che non stiamo ancora sfruttando. Usa `_agency/context/` + `signals/signal-library.md` come fonte.

---

## Step 1 — Carica il contesto dai file esistenti

**Non ripartire da zero.** Prima di chiedere qualsiasi cosa, leggi ciò che è già stato popolato.

**Modo A (cliente)** — leggi:
- `clients/[nome]/context/profile.md` → cosa fa il prodotto, chi è il buyer
- `clients/[nome]/context/icp-definition.md` → ICP / segmento target
- `clients/[nome]/context/positioning.md` → categoria, differenziazione
- `clients/[nome]/context/competitor-radar.md` → alternative competitive (utile per il play di displacement)

**Modo B (collettivo)** — leggi:
- `_agency/context/profile.md`, `_agency/context/icp-definition.md`, `_agency/context/positioning.md`
- `signals/signal-library.md` → segnali già operativi (per evitare di "scoprire" ciò che già facciamo)

Estrai dai file le 4 dimensioni che servono alla diagnosi:
1. **Prodotto + buyer primario**
2. **ICP / segmento target**
3. **GTM motion**: sales-led / product-led / marketing-led / hybrid
4. **Stage**: Early (<1M ARR o <10 dip.) / Growth (1-20M ARR, 10-100) / Scaling (20M+ ARR, 100+)

---

## Step 2 — Colma SOLO i gap

Se e solo se una delle 4 dimensioni non è desumibile dai file, chiedila con **AskUserQuestion**. Tipicamente i due gap più frequenti sono **GTM motion** e **stage** (spesso non scritti esplicitamente nel context).

Non ri-chiedere ciò che hai già letto. Non riempire i buchi con assunzioni: se manca, chiedi.

---

## Step 3 — Leggi la plays library

Leggi `references/plays-library.md` per intero. Contiene i plays attivi (signal-based, warm outbound, personalization, social) con segnale, meccanismo, tool, difficoltà e fit con la motion — più la mini-tabella di mapping verso i nostri codici segnale (Sxx) e una sezione "Future State" (product-led/expansion) che **non** entra nelle raccomandazioni di default.

---

## Step 4 — Seleziona e prioritizza

Con contesto + library, seleziona **5-8 plays** in ordine di priorità. Applica questi filtri:

- Il cliente ha **realmente accesso** al segnale sottostante? Se no, va in "Future State", non scartato del tutto.
- Il play **combacia con la motion**?
- Il livello di sofisticazione è **adatto allo stage**? (early = 1-2 plays max; non over-engineerizzare)
- C'è una ragione **specifica e ad alta convinzione** per cui questo play calza a QUESTO cliente?

Sii opinato. Salta i plays che non calzano. Niente liste-cuscinetto con opzioni generiche. Se due plays sono simili, scegli il migliore. Indica l'uno o i due plays su cui metteresti la faccia per questo cliente.

**Default per stage** (da rispettare salvo motivo esplicito):
- **Early**: 1-2 plays attivi adesso, il resto in Future State. Per il nostro ICP tipico (startup B2B early, sales-led) i naturali sono job postings (#8), LinkedIn connections/engagement (#6/#5), website visitor de-anon (#1), closed-lost reopen (#11).
- **Growth**: 3-5 plays in parallelo, si iniziano a stratificare i segnali.
- **Scaling**: signal stack completo + micro-campagne.

---

## Step 5 — Output

Usa esattamente questo formato (italiano):

---

## Plays GTM consigliati per [Nome Cliente/Prodotto]

**GTM motion**: [Sales-led / PLG / Marketing-led / Hybrid]
**Stage**: [Early / Growth / Scaling]
**Segnale più inutilizzato**: [una frase sul segnale a più alta leva che il cliente non sta ancora operazionalizzando]

---

### Plays prioritari

**[Rank]. [Nome play]** · [Categoria] · Difficoltà: [Beginner / Intermediate / Advanced]

**Segnale**: [cosa lo innesca — sii specifico]
**Come funziona**: [2-3 frasi sul workflow di automazione, incluso come fluiscono i dati]
**Tool**: [tool che lo abilitano — vedi nota stack nel reference]
**Perché calza a voi**: [1-2 frasi ancorate al loro prodotto/ICP/motion — non generico]
**Mapping segnale**: [se il play ha un nostro codice Sxx in signal-library, indicalo — es. "≈ S02/S03"]

---

[Ripeti per ogni play]

---

### Da dove partire

[1-2 frasi: quale play lanciare per primo e perché, in base a facilità di setup e impatto atteso dato stage e dati esistenti]

### Bridge all'esecuzione

I plays signal-based qui sopra **non finiscono in questo documento**. Per ciascuno:
1. Verifica/aggiungi il segnale corrispondente in `signals/signal-library.md` (con score, decay, hook).
2. Applica `signals/signal-routing.md` per classificazione → tier → azione.
3. Costruisci la campagna con `workflows/campaign-build.md` (e `skills/signal-to-sequence/` per il copy).

I plays NON signal-based (warm intro, personalizzazione, social) si appoggiano allo stesso `campaign-build`, con il segnale sostituito dal criterio di warm/relazione.

### Future State

[2-3 plays da costruire una volta che i prioritari girano — richiedono più accesso ai dati o più sofisticazione. Includi qui i plays product-led/expansion SE e SOLO SE il cliente avrà accesso ai product usage data.]

---

## Tono

Scrivi come un practitioner GTM senior che dà consigli diretti — specifico, ancorato, opinato. Niente linguaggio da consulenza che si copre su tutto. Se un play è un chiaro vincitore per questo cliente, dillo. Se un play è tentante ma sbagliato per lo stage, di' perché l'hai lasciato fuori. Italiano, sempre.

---

## Promemoria sul posizionamento del collettivo

Questa library **non** è un menu di tattiche da spuntare. Il nostro differenziatore è "non partiamo dalle campagne, partiamo dall'analisi". Usa la skill come **strumento diagnostico che gira DOPO** ICP e positioning — mai come scorciatoia per saltare l'analisi. Altrimenti diventiamo l'agenzia che critichiamo.
