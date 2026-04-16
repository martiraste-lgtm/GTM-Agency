# Anti-patterns — Errori Comuni nel Goal Setting

## Anti-pattern 1: Output travestiti da Outcome

**Come si presenta**:
- KR: "Lanciare 3 nuove feature entro Q2"
- KR: "Fare 10 customer interview"
- KR: "Creare una dashboard di analytics"
- KR: "Scrivere 8 articoli di blog"

**Perché è un problema**: completare questi KR non garantisce nessun miglioramento del business. Il team può fare tutto e il needle non si muove. Non c'è prova causale tra l'azione e il risultato.

**Test diagnostico**: chiedi "se raggiungiamo questo KR, sappiamo con certezza che il business è migliorato?" Se la risposta è no o "dipende", è un output.

**Come correggere**:
- "Lanciare 3 feature" → "Tasso di adozione nuove feature ≥ 25% degli utenti attivi entro fine Q2" `[Leading][Strategic]`
- "Fare 10 interview" → diventa una Task sotto un'Initiative di discovery
- "8 articoli di blog" → "Traffico organico da contenuti deve crescere da 1.2K → 3K visite/mese `[Leading][Execution]`"

---

## Anti-pattern 2: Objective senza WHY e WHY NOW

**Come si presenta**:
- "Migliorare la customer experience"
- "Accelerare la crescita"
- "Aumentare l'efficienza operativa"
- "Ottimizzare il prodotto"

**Perché è un problema**: senza WHY e WHY NOW, l'Objective non dà nessuna direzione su dove concentrare l'energia. Due team possono avere lo stesso Objective e lavorare su cose completamente diverse — e avere entrambi ragione formalmente.

**Come correggere**: aggiungi sempre la sezione WHY (ragione causale) e WHY NOW (trigger temporale specifico). Se non riesci a scriverla, la strategia non è sufficientemente chiara — lavora sulla strategia prima degli OKR.

---

## Anti-pattern 3: Tutti i Commitments sono Lagging

**Come si presenta**:
- C1: Revenue da nuovi clienti +30%
- C2: Churn mensile ≤ 2%
- C3: NPS ≥ 45

**Perché è un problema**: si misura solo il passato. A metà ciclo non si sa se si sta andando nella direzione giusta — i Lagging arrivano tardi. Se a fine Q3 si scopre che il churn è peggiorato, è troppo tardi per intervenire.

**Come correggere**: aggiungi almeno 1-2 Commitment Leading che predicono i Lagging.
- Revenue +30% → Leading: "Conversion rate trial-to-paid deve crescere da 8% → 14%" `[Leading][Strategic]`
- Churn ≤ 2% → Leading: "% utenti che completano l'onboarding entro 7 giorni deve crescere da 42% → 65%" `[Leading][Execution]`

---

## Anti-pattern 4: Goal Probabilistici (50-70%) presentati come Committments

**Come si presenta**:
- "Puntiamo ad aumentare gli MQL del 40%, ma se arriviamo al 60% è già un successo"
- "Il target è ambizioso, ci aspettiamo di raggiungere il 70%"
- "Questi sono stretch goals"

**Perché è un problema**: crea una zone of confusion. Leadership e team non sanno cosa sarà davvero fatto a fine ciclo. Rende impossibile il course correction durante il ciclo perché non è chiaro quando si è davvero off-track.

**Come correggere**: separa i Commitments (100%, deterministic) dal Moonshot (1 solo, 60-70%, etichettato esplicitamente come tale). Riduci i target dei Commitments a qualcosa che il team è davvero convinto di poter raggiungere.

---

## Anti-pattern 5: Baseline Assente

**Come si presenta**:
- KR: "Aumentare il fatturato del 20%"
- KR: "Ridurre i bug del 30%"
- KR: "Migliorare il tasso di conversione"

**Perché è un problema**: senza baseline è impossibile verificare se il goal è stato raggiunto. "20% di aumento" rispetto a cosa? All'anno scorso? Al quarter precedente? Alla media mensile degli ultimi 3 mesi?

**Come correggere**: ogni Commitment deve avere una baseline esplicita tra parentesi.
- "Fatturato +20%" → "Fatturato mensile deve crescere da (€45K) → €54K entro fine Q2"
- "Bug -30%" → "Bug critici aperti devono ridursi da (23) → 16 entro fine Q1"

---

## Anti-pattern 6: KR di Stage Sbagliato (Strategic Risk quando si è a Understanding)

**Come si presenta**: team che non ha ancora dati su cosa causa un problema che mette Commitments di outcome aggressivi.
- "Aumenta retention dei nuovi utenti dal 30% al 50%" — ma il team non ha ancora analizzato il funnel, non sa dove droppano gli utenti, non ha mai testato niente in questo spazio.

**Perché è un problema**: il team non sa da dove partire. L'unico modo per "raggiungere" il goal è la fortuna o attività random. Quando non ci riesce, si sente frustrato perché il goal era strutturalmente irraggiungibile con le informazioni disponibili.

**Come correggere**: identifica il Frontier Stage reale. Se sei a Understanding, il Commitment corretto è "Identifica le 3 principali cause di drop nell'onboarding nei primi 7 giorni". Poi nel ciclo successivo puoi mettere un Commitment di outcome.

---

## Anti-pattern 7: Health Metrics Assenti — Ottimizzazione che Rompe Altro

**Come si presenta**: team con Commitments aggressivi su crescita (revenue, MQL, acquisition) senza nessun guardrail su metriche che potrebbero deteriorarsi come effetto collaterale.

**Esempi di danni:**
- Sales che fa sconti aggressivi per aumentare la revenue → margine crolla
- Marketing che aumenta il volume di lead abbassando la soglia di qualifica → CAC esplode, SDR sommersi
- Product che lancia feature velocemente per hit un deadline → NPS crolla, bug in produzione
- Growth che aumenta i signup con incentivi → retention a 30 giorni precipita

**Come correggere**: per ogni Commitment aggressivo, chiedi "cosa potrebbe rompersi se ottimizziamo questo in modo aggressivo?" Quella risposta è la tua Health Metric.

---

## Anti-pattern 8: Initiatives senza Ipotesi Causale

**Come si presenta**:
- Initiative: "Fare cold outreach"
- Initiative: "Migliorare il prodotto"
- Initiative: "Fare content marketing"
- Initiative: "Ottimizzare il funnel"

**Perché è un problema**: senza ipotesi causale, non si capisce perché queste iniziative dovrebbero portare al Commitment. Se l'iniziativa fallisce nel muovere il Commitment, non si sa se è perché l'esecuzione era sbagliata o perché l'ipotesi era sbagliata.

**Come correggere**: ogni Initiative deve avere un'ipotesi causale esplicita.
- "Fare cold outreach → ipotesi: contattare 200 ICP/settimana con messaging personalizzato genererà 15 nuovi meeting al mese, che a sua volta porterà 4-5 nuove opportunità qualificate"

---

## Anti-pattern 9: Cascata Meccanica

**Come si presenta**: Company KR "Aumentare ARR del 30%" → Team Marketing Objective: "Aumentare ARR del 30%"

**Perché è un problema**: il team Marketing non controlla direttamente l'ARR. Questo crea un Objective che o è un lagging metric su cui il team non ha agency diretta, o spinge il team a ottimizzare per il numero senza capire quale leva azionare.

**Come correggere**: il Company KR alimenta la Narrative del team, non diventa il suo Objective. Il team Marketing dovrebbe chiedersi "come contribuiamo noi all'ARR +30%?" e rispondere con un Objective specifico per la propria leva (es: "Accelerare la pipeline qualificata attraverso inbound + referral").

---

## Anti-pattern 11: OKR come Strumento di Performance Evaluation

**Come si presenta**:
- I KR vengono collegati a bonus, compensation o promozioni
- I manager li presentano come "contratti" con il team
- Il team viene valutato in base al completion rate degli OKR a fine ciclo

**Perché è un problema**: collegare gli OKR alla valutazione distrugge l'ambizione strutturalmente. Le persone fanno sandbagging — abbassano i target preventivamente per garantirsi la valutazione positiva. Nessuno metterà mai un Moonshot se rischia di penalizzare il proprio bonus. L'effetto è esattamente l'opposto di quello desiderato: i goal diventano più conservativi, non più ambiziosi.

Secondo meccanismo: chi non raggiunge un Commitment per ragioni fuori dal proprio controllo (pivot strategico, dipendenze di altri team, mercato) viene penalizzato per decisioni aziendali che non controllava. Il sistema smette di essere collaborativo e diventa burocratico e difensivo.

**Come correggere**: separare nettamente i due sistemi.
- OKR → strumento per alignment, focus e apprendimento collettivo. Non misura la persona, misura la direzione del team.
- Performance evaluation → basarsi su comportamenti, qualità di esecuzione, ownership, impatto sul team — non sul completion rate di KR.

Se manca accountability, la soluzione è il check-in frequente durante il ciclo (settimanale o bisettimanale) — non la valutazione annuale. Il problema non è l'assenza di conseguenze: è l'assenza di tracking in tempo reale.

---

## Anti-pattern 10: OKR Scritti a Gennaio, Riesumati a Dicembre

**Come si presenta**: planning elaboratissimo a inizio ciclo, zero tracking durante, valutazione superficiale a fine ciclo.

**Perché è un problema**: nessun course correction possibile. Le iniziative che non funzionano non vengono abbandonate. Si finisce per completare le Tasks (esecuzione) ma mancare i Commitments (impatto).

**Come correggere**: il framework ibrido richiede check-in settimanali/bisettimanali sui Commitments. Se un Commitment è sotto il ritmo necessario, il team deve avere la struttura per identificarlo e aggiustare le Initiatives — non a fine ciclo, ma durante.

Cadenza consigliata:
- Settimanale: aggiornamento progress su ogni Commitment (% completato, trend)
- Bisettimanale: review delle Initiatives (stanno funzionando? serve cambiare approccio?)
- Fine ciclo: scoring + retrospettiva + input per ciclo successivo
