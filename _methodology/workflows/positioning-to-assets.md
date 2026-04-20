# Workflow: Da Positioning a Asset Operativi

*Come trasformare l'output della skill `b2b-positioning-diagnostic` in materiale che lavora.*
*Eseguire dopo ogni positioning sprint (interno o cliente).*

---

## Input: cosa produce il positioning sprint

La skill `b2b-positioning-diagnostic` produce:

1. **Competitive alternatives** — con chi si confronta davvero il buyer
2. **Differentiated value** — cosa offriamo che le alternative non offrono
3. **Target customers** — chi trae più valore e perché
4. **Market category** — come ci presentiamo al mercato
5. **Positioning canvas** — frase di positioning completa

---

## Step 1 — Da positioning a Signal Map

**Input**: Differentiated value + Target customers
**Output**: `signals/signal-library.md` (aggiornato o creato)

Per ogni target customer confermato:
- Quali eventi nella loro azienda indicano che stanno cercando quello che offriamo?
- Quali hiring segnalano un problema che noi risolviamo?
- Quali funding rounds indicano budget disponibile per il nostro tipo di soluzione?
- Quali tech adoption indicano maturità digitale sufficiente?

→ Aggiungi i segnali specifici alla signal library con score e hook contestuale.

---

## Step 2 — Da positioning a Message House

**Input**: Differentiated value + Competitive alternatives
**Output**: documento message house (salvare in `outbound/sequences/message-house.md`)

Struttura:
```
HEADLINE (cosa facciamo, per chi, diversamente da chi)
  ├── Value pillar 1: [beneficio principale vs. alternativa 1]
  │   └── Proof point: [dato / esempio / caso]
  ├── Value pillar 2: [beneficio principale vs. alternativa 2]
  │   └── Proof point: [dato / esempio / caso]
  └── Value pillar 3: [differenziatore unico]
      └── Proof point: [dato / esempio / caso]
```

---

## Step 3 — Da positioning a Copy Homepage

**Input**: Market category + Positioning canvas + Message house
**Output**: struttura copy per homepage (da passare a `skills/saas-homepage-analyzer/`)

Mappatura sezioni:
- **Hero headline**: positioning canvas → adattato per il buyer (non per noi)
- **Hero subheadline**: problema che risolviamo + come (1 frase)
- **Social proof**: proof points dal message house
- **Feature/benefit section**: differentiated value → tradotto in benefici per il buyer
- **CTA**: coerente con il market category (se nuova categoria → educa; se esistente → confronta)

---

## Step 4 — Da positioning a Deck Commerciale

**Input**: Tutto il positioning canvas + Target customers + Competitive alternatives
**Output**: struttura deck (da passare a `skills/sales-deck-creator/`)

Slide mapping:
1. **Problema** (dal punto di vista del buyer, non di noi)
2. **Perché le soluzioni attuali non funzionano** (competitive alternatives)
3. **Il nostro approccio** (differentiated value → tradotto)
4. **Come funziona** (processo, non feature)
5. **Risultati** (proof points, case study)
6. **Per chi è** (target customers)
7. **Next step**

---

## Step 5 — Da positioning a Sequenze Email

**Input**: Message house + Signal map + Target customers
**Output**: sequenze in `outbound/sequences/`

Una sequenza per ogni combinazione prioritaria:
- [Segnale trigger] + [Persona] + [Angolo messagio dal message house]

Struttura ogni sequenza:
- Email 1: aggancio al segnale specifico + problema rilevante
- Email 2: differentiated value (non feature, benefit)
- Email 3: proof point o case study
- Email 4: follow-up diretto ("ha senso parlarne?")

---

## Checklist di completamento

- [ ] Signal map aggiornata con segnali specifici per ICP confermato
- [ ] Message house completato e salvato
- [ ] Brief homepage scritto e pronto per saas-homepage-analyzer
- [ ] Struttura deck pronta per sales-deck-creator
- [ ] Almeno 1 sequenza email per il segmento prioritario
- [ ] Content pillar aggiornati per riflettere il nuovo positioning
