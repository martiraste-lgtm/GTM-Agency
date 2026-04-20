---
name: preventivo
description: Genera preventivi personalizzati per il servizio GTM Engineering + Outbound with Signals. Usa per nuovi prospect dopo la discovery call o per adattare il preventivo base a un nuovo cliente. Trigger: "crea un preventivo per", "prepara la proposta per", "genera il preventivo per [cliente]".
license: MIT
metadata:
  author: GTM Collective
  version: 1.0.0
---

## Overview

Skill per generare preventivi su misura per il servizio GTM Engineering + Outbound with Signals. Il preventivo si basa su un intake di 7 domande e produce un documento in 10 sezioni, leggibile anche per chi non conosce il GTM engineering.

Leggi `references/template-preventivo.md` e `references/benchmark-outbound.md` prima di generare.

---

## Instructions

### Step 1 — Intake

Se non hai già le informazioni, fai queste 7 domande. Se il contesto è già disponibile (appunti call, note), estrai le risposte direttamente e chiedi conferma solo su ciò che manca.

1. **Chi è il cliente?** Nome azienda, settore, prodotto (2 righe max)
2. **Fase e trazione?** Pre-PMF / post-PMF / early growth + ARR o revenue indicativo + n° clienti paganti
3. **Problema principale?** Cosa li ha portati a cercare questo servizio — in parole loro se possibile
4. **Stato attuale GTM?** Hanno già outbound? CRM? Sequenze? Infrastruttura email? Asset (homepage, deck)?
5. **ICP e verticali?** Hanno già un ICP definito o è da costruire? Target geografico?
6. **Team commerciale?** Founder-led sales? Sales interno? Nessuno? Chi gestirà le call con i prospect?
7. **Urgenza e scadenze?** Round in corso? Obiettivo trimestrale? Evento specifico entro quando?

### Step 2 — Analisi e inquadramento

Prima di generare il preventivo:
- Identifica il gap strategico principale (tensione tra dove sono e dove vogliono arrivare)
- Calibra la timeline in base a cosa hanno già (se hanno asset → accelera; se partono da zero → aggiungi le settimane di fondazione)
- Nota se il team interno gestirà le call con i prospect o lo faremo noi (impatta la sezione "Ritmo operativo")
- Proponi l'inquadramento all'utente prima di generare il documento completo

### Step 3 — Generazione preventivo

Segui la struttura in `references/template-preventivo.md`. Personalizza ogni sezione con i dati del cliente. Non usare frasi generiche che potrebbero applicarsi a qualsiasi azienda.

**Regole di personalizzazione**:
- L'apertura deve citare il gap specifico emerso in discovery — mai complimenti
- La timeline deve riflettere il punto di partenza reale del cliente
- I segnali nella sezione outbound devono essere specifici al loro settore/ICP
- I benchmark nella sezione metriche vengono da `references/benchmark-outbound.md`

### Step 4 — Review e iterazione

Presenta la bozza e chiedi:
- "C'è qualcosa che non rispecchia quello che è emerso in call?"
- "Vuoi aggiungere o modificare qualche sezione?"
- Itera fino a conferma

---

## Examples

**Scenario A — Startup SaaS B2B post-PMF, 400K ARR, ha già un deck ma nessun outbound**
Input dall'utente: "Devo fare il preventivo per Acme, SaaS per HR tech, 400K ARR, hanno un founder che fa sales ma non hanno mai fatto outbound. Vogliono costruire il sistema."
Output: preventivo con timeline che parte dalla settimana 1 di analysis (ICP, signals, positioning) e comprende infrastruttura email da zero. Segnali specifici per HR tech (hiring HR Manager, scale-up in crescita, ESG declarations).

**Scenario B — Startup no-team, settore energia, strategia B2B**
Input: contesto della call (settore, problema, fase)
Output: preventivo con nota esplicita che il collettivo gestisce anche le call con i prospect, timeline adattata.

---

## Troubleshooting

**Non ho abbastanza informazioni sul cliente**: usa solo le 7 domande di intake — non inventare contesto. Scrivi [DA COMPLETARE] dove mancano dati specifici.

**Il cliente ha già molti asset**: comprimi le settimane 1-4 e anticipa il lancio outbound. Nota esplicitamente nella timeline cosa viene saltato o accelerato.

**Il cliente non vuole gestire call con i prospect**: aggiungi nella sezione "Ritmo operativo" che il collettivo gestisce le prime call di discovery in autonomia.
