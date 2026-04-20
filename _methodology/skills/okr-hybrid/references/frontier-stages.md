# Frontier Stages — Guida Completa

## Origine

Il concetto di "frontier of understanding" viene da Ravi Mehta (ex CPO Tripadvisor). L'idea centrale: il tipo di goal giusto non è sempre un outcome metrico. Dipende da dove si trova il team nel ciclo di comprensione del proprio problema.

Se si mette un goal di outcome quando si è ancora a Understanding Risk, il team non sa come raggiungerlo — e questo genera frustrazione, sandbagging, e il ciclo vizioso degli OKR.

---

## I 4 Frontier Stages

### Stage 1 — Understanding Risk
*"Non sappiamo ancora quali leve muovere"*

**Situazione**: il team non ha ancora dati o ipotesi sufficienti per definire una strategia. Non si sa cosa causa il problema che si vuole risolvere.

**Goal appropriato**: qualitativo, orientato alla ricerca o alla scoperta.

**Esempi di Commitments**:
- "Identificare le 3 leve principali che guidano la retention dei nuovi utenti nei primi 14 giorni"
- "Completare 15 customer interview e sintetizzare i top 5 job-to-be-done non soddisfatti"
- "Costruire il funnel di conversione con dati granulari entro [data]"

**Segnali che sei qui**:
- Non sai ancora quale metrica dovresti muovere
- Le conversazioni sul goal si bloccano su "ma cosa causa esattamente X?"
- Hai assunzioni ma non dati
- Stai ancora facendo discovery

**Errore da evitare**: mettere un Commitment outcome tipo "aumenta retention del 15%" quando non hai ancora capito cosa causa la bassa retention. Il team non sa da dove partire e l'unica alternativa è il wishful thinking.

---

### Stage 2 — Dependency Risk
*"Sappiamo cosa fare, ma non abbiamo ancora le risorse o le capabilities per farlo"*

**Situazione**: la strategia è chiara, ma mancano strumenti, processi, persone o infrastruttura necessari per eseguirla.

**Goal appropriato**: deliverable o milestone di setup.

**Esempi di Commitments**:
- "Piattaforma di A/B testing configurata e validata con 3 test pilota entro [data]" — binario
- "Lead scoring implementato e integrato nel CRM entro [data]" — binario
- "Team di 2 growth engineer onboardati e operativi entro fine mese" — binario
- "Data pipeline per tracciare il funnel di onboarding live entro [data]" — binario

**Segnali che sei qui**:
- Sai cosa dovresti misurare ma non riesci a farlo tecnicamente
- Hai una strategia chiara ma il team non ha le skills per eseguirla
- Stai aspettando un tool, un'integrazione, un hire, un processo
- I tuoi Commitments teorici richiedono infrastruttura che non hai

**Errore da evitare**: ignorare il Dependency Risk e mettere direttamente Commitments di Execution o Strategic. Il team poi fallisce non per mancanza di effort, ma perché gli strumenti non erano pronti.

---

### Stage 3 — Execution Risk
*"Abbiamo tutto quello che serve, dobbiamo dimostrare di saper eseguire"*

**Situazione**: strategia chiara, risorse disponibili. Il test è se il team riesce a eseguire con qualità e velocità.

**Goal appropriato**: output misurabile — numero di esperimenti, feature lanciate, contenuti prodotti, processi implementati.

**Esempi di Commitments**:
- "Lanciare 4 esperimenti di retention entro fine Q2 [Leading][Execution]"
- "Pubblicare 12 case study B2B entro fine Q1 [Leading][Execution]"
- "Contattare 800 lead outbound con nuove sequenze entro [data] [Leading][Execution]"
- "Completare il redesign dell'onboarding flow e rilasciarlo in produzione entro [data]"

**Segnali che sei qui**:
- Hai una strategia, hai gli strumenti, hai le persone
- Il principale rischio è la velocità di esecuzione
- Puoi descrivere con precisione cosa produrrete
- Non sai ancora se l'output genererà l'impatto desiderato

**Errore da evitare**: mettere Commitments di outcome quando non hai ancora prove causali. "Aumenta conversion del 20%" è Strategic Risk, non Execution — usarlo quando sei a Execution crea aspettative irrealistiche.

---

### Stage 4 — Strategic Risk
*"Abbiamo prove che la nostra strategia funziona — ora dobbiamo scalare l'impatto"*

**Situazione**: il team ha già evidenza causale che le proprie azioni portano al risultato desiderato. Il goal è scalare quell'impatto.

**Goal appropriato**: outcome metrico con baseline, target e deadline chiari.

**Esempi di Commitments**:
- "Conversion rate trial-to-paid deve crescere da 8% → 14% entro fine Q2 [Lagging][Strategic]"
- "NPS deve crescere da 32 → 45 entro fine anno [Lagging][Strategic]"
- "ARR da nuovi clienti deve crescere da 400K → 700K entro fine Q3 [Lagging][Strategic]"
- "Churn mensile deve ridursi da 3,2% → 1,8% entro fine Q4 [Lagging][Strategic]"

**Segnali che sei qui**:
- Hai dati che mostrano correlazione/causalità tra le tue azioni e il risultato
- Hai già eseguito esperimenti con risultati positivi
- Sai con discreta certezza che aumentando X si muove Y
- Il rischio principale è "riusciremo a scalare la strategia?"

**Errore da evitare**: rimanere troppo a lungo a Execution (output) quando hai già prove che la strategia funziona. Se sai che ogni esperimento genera X punti di conversion, è il momento di mettere un Commitment di outcome.

---

## Come Usare i Frontier Stages nella Pratica

### Domande diagnostiche per identificare lo stage

1. "Sappiamo con certezza quale metrica dobbiamo muovere e perché?" → No = Understanding Risk
2. "Abbiamo tutti gli strumenti, le skills e le risorse per eseguire?" → No = Dependency Risk
3. "Abbiamo prove causali che le nostre azioni portano al risultato?" → No = Execution Risk
4. Tutte le risposte sono sì → Strategic Risk

### Mix consigliato in un set di Commitments

Non è necessario che tutti i Commitments siano allo stesso stage. Un mix tipico per un team early-stage:
- C1 `[Understanding]` → per scoprire le leve
- C2 `[Execution]` → per eseguire su quello che si sa già
- C3 `[Strategic]` → per uno o due outcome su cui si ha già evidenza

### Progressione nel tempo

Il Frontier Stage di un'area tipicamente evolve così nel tempo:

```
Q1: Understanding → "identifica le leve di retention"
Q2: Dependency + Execution → "costruisci il test e lancia 4 esperimenti"
Q3: Execution → "lancia 8 esperimenti con ipotesi validate"
Q4: Strategic → "aumenta retention dei nuovi utenti dal 35% al 50%"
```

Questa progressione è normale e sana. Un team che salta direttamente a Strategic Risk senza aver attraversato gli stage precedenti di solito fallisce i Commitments per ragioni strutturali, non per mancanza di impegno.

---

## Errori Frequenti per Stage

| Stage | Errore tipico | Conseguenza |
|-------|--------------|-------------|
| Understanding | Mettere Commitments di outcome | Il team non sa da dove partire, paralisi o attività random |
| Dependency | Ignorarlo, andare direttamente a Execution | I tool non sono pronti a metà ciclo, execution bloccata |
| Execution | Trattare gli output come outcome | Il team consegna ma il business non si muove, frustrazione |
| Strategic | Rimanere ad Execution quando si hanno prove causali | Si lascia sul tavolo potenziale di impatto già dimostrato |
