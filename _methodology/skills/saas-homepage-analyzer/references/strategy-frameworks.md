# Strategy Frameworks

## 1. ICP e Situation Mapping

Prima di scegliere l'anchor o scrivere il copy, devi capire profondamente il buyer.

### Chi è l'ICP (Ideal Customer Profile)

Identifica:
- **Persona / Ruolo**: Chi prende la decisione o la influenza? (es. Founder, Head of Product, RevOps)
- **Tipo di azienda**: Settore, dimensione, stage di funding, modello di business (es. B2B SaaS Seed-Series A)
- **Situazione**: Cosa sta cercando di fare in questo momento? (il job-to-be-done contestuale)

### Chi è il Champion

Il Champion è la persona specifica dentro l'azienda che si batterebbe internamente per adottare il tuo prodotto. Non sempre coincide con chi paga.

Caratteristiche del Champion ideale:
- Ha il problema più acuto
- Ha abbastanza influenza per spingere l'acquisto
- Guadagna personalmente dalla soluzione

### Use Case Mapping

Per ogni situazione del buyer, mappa:

| Situazione | Come lo fanno oggi (Current Way) | Limitazioni | Problemi risultanti |
|------------|----------------------------------|-------------|---------------------|
| Es. "preparare report settimanali" | Excel manuale | Richiede 4 ore, errori frequenti | Report in ritardo, decisioni sbagliate |

Questo mapping è il materiale grezzo per il Value Proposition Canvas.

---

## 2. Positioning: Competitive vs Contextual

### Competitive Positioning
Il tuo punto di riferimento è un **tool o categoria esistente** che il buyer già conosce.

- **Competitive Alternative**: "Siamo un'alternativa a [Leader dominante]"
- **Product Category**: "Siamo un [CRM / HR Software / Analytics tool]"

**Quando usarlo**: Mercato maturo, buyer con alta awareness, categorie definite su G2/Capterra.

**Esempi**: Slack vs email aziendale, nuovi CRM vs Salesforce, Linear vs Jira.

**Come differenziarsi**: Articola 2-3 talking points specifici:
- "A differenza di [Cluster competitor 1] noi..."
- "A differenza di [Cluster competitor 2] noi..."

### Contextual Positioning
Il tuo punto di riferimento è un **problema, caso d'uso o attività** che il buyer già vive.

- **Use Case**: "Ti aiutiamo a fare [X] senza [Y]"
- **Activity**: "Ti aiutiamo a fare [Attività]" (quando la soluzione è ancora manuale)

**Quando usarlo**: Mercato emergente, buyer che non cerca per categoria, job-to-be-done chiaro ma non categorizzato.

**Esempi**: Calendly vs "ping-pong di email per trovare un orario", Expensify vs "scontrini incollati su carta + Excel".

---

## 3. Fletch's Messaging Elements (i 6 mattoni del copy)

Ogni value proposition si costruisce con 6 elementi concatenati:

```
[Use Case] + [Current Tool] + [Problem]
        ↓
[Capability] + [Feature] + [Benefit]
```

| Elemento | Definizione | Esempio (PandaDoc) |
|----------|-------------|-------------------|
| **Use Case** | Cosa il buyer sta cercando di fare | Preparare contratti per e-signature |
| **Current Tool** | Come lo fa oggi senza il tuo prodotto | HelloSign |
| **Problem** | Cosa blocca il progresso | Ogni modifica richiede upload + ri-aggiungere tutti i campi |
| **Capability** | Cosa può fare con il tuo prodotto | Creare contratti nativamente in PandaDoc |
| **Feature** | Cosa rende possibile la capability | Visual designer integrato |
| **Benefit** | Il risultato dell'aver usato la capability | Creare e modificare contratti molto più velocemente |

**La logica del Reversal**: il Benefit è l'esatto opposto del Problem. Se il problema è "richiede troppo tempo", il benefit è "risparmi ore". Questa simmetria rende il copy convincente.

---

## 4. Value Proposition Canvas — Competitive

Usare quando: anchor = Competitive Alternative o Product Category.

**Struttura**: 8 colonne, righe = alternative competitor

| Persona | Company Type | Use Case | Current Tool | Problem | Capability | Feature | Desired Outcome |
|---------|-------------|----------|-------------|---------|-----------|---------|----------------|
| (Primary) | (Primary) | (Summary) | Tool principale | Problema primario | Capability primaria | Feature primaria | Outcome primario |
| (Sbiadito) | (Sbiadito) | (invariato) | Competitor 1 | Problema specifico vs C1 | Come lo risolvi tu | Feature specifica | Benefit specifico |
| (Sbiadito) | (Sbiadito) | (invariato) | Competitor 2 | Problema specifico vs C2 | Come lo risolvi tu | Feature specifica | Benefit specifico |
| (Sbiadito) | (Sbiadito) | (invariato) | Competitor 3 | Problema specifico vs C3 | Come lo risolvi tu | Feature specifica | Benefit specifico |

**Freccia Reversal**: dall'ultima colonna (Desired Outcome) torna alla colonna Problem — il risultato è l'esatta risoluzione del problema.

**Freccia Linked**: collega Current Tool e Problem nella stessa riga — strumento sbagliato genera problema specifico.

---

## 5. Value Proposition Canvas — Contextual

Usare quando: anchor = Use Case o Activity.

**Struttura**: 8 colonne, righe = sotto-fasi del use case principale

| Persona | Company Type | Use Case | Current Tool | Problem | Capability | Feature | Desired Outcome |
|---------|-------------|----------|-------------|---------|-----------|---------|----------------|
| (Primary) | (Primary) | Use case macro | Tool interno/manuale | Problema macro | Capability macro | Feature/categoria | Outcome macro |
| (Sbiadito) | (Sbiadito) | Sotto-fase 1 | (stesso) | Problema fase 1 | Come aiuti in fase 1 | Feature specifica | Benefit fase 1 |
| (Sbiadito) | (Sbiadito) | Sotto-fase 2 | (stesso) | Problema fase 2 | Come aiuti in fase 2 | Feature specifica | Benefit fase 2 |
| (Sbiadito) | (Sbiadito) | Sotto-fase 3 | (stesso) | Problema fase 3 | Come aiuti in fase 3 | Feature specifica | Benefit fase 3 |

**Nota**: le prime 2 colonne (Persona, Company Type) e spesso il Current Tool rimangono identici tra le righe. Le sotto-fasi sono i passi sequenziali che il buyer deve compiere per completare il use case principale.

---

## 6. Matrice Anchor → Canvas

| Anchor | Canvas da usare | Righe del canvas |
|--------|----------------|-----------------|
| Competitive Alternative | Competitive | Un competitor dominante + 2-3 alternative |
| Product Category | Competitive | Cluster di competitor nella categoria |
| Use Case | Contextual | Sotto-fasi del job-to-be-done |
| Activity | Contextual | Sotto-attività del processo manuale |
