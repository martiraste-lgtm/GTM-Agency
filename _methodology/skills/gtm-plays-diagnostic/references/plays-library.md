# GTM Plays Library

Catalogo di 26 plays di outbound/GTM automatizzato, sintetizzati da ricerca Growth Unhinged e playbook di practitioner. Ogni play include segnale, meccanismo, tool, difficoltà e fit con la GTM motion.

**Uso**: questo è un catalogo *strategico* (per scegliere quale motion attivare in fase diagnostica). Non è la `signal-library` operativa del collettivo — vedi il box "Confine" nella SKILL.md.

---

## Nota sui tool

La lista tool di ogni play è una **reference US-centric**. Lo stack di default del collettivo resta **Apollo / Clay / Instantly / HeyReach** (vedi `workflows/campaign-build.md` ed `workflows/enrichment.md`). Cita i tool della library solo quando aggiungono una capability che non copriamo già.

## Mapping verso i nostri codici segnale

Diversi plays si sovrappongono ai segnali già scorati nella nostra `signals/signal-library.md`. Quando consigli un play con un mapping, citalo — connette la diagnosi all'esecuzione.

| Play | Segnale nostro (Sxx) |
|------|----------------------|
| #2 Competitor / Tech Stack | S09 (cambio tool/stack) |
| #8 Relevant Job Postings | S02 / S03 / S03b (hiring sales, SDR, fractional PMM) |
| #5 LinkedIn Engagement (own content) | S07 / S13 (post founder su GTM / content indifferenziato) |
| #7 Social Listening (keyword) | S07 / S14 (post GTM / confronto con peer) |
| #9 Geo/Event-based | S08 (partecipazione evento) |
| Funding-adjacent (vari) | S01 (funding round) |
| #11 Closed-lost reopen / #12 Champion tracking | nessun Sxx ancora — candidati a nuovi segnali |

---

## Panoramica categorie

- **Signal-based** (1-9): innescati da segnali comportamentali o firmografici di intento d'acquisto
- **Warm outbound** (10-14): targettano persone con relazione, brand o prossimità di network pregressa
- **Personalization** (15-17): aumentano la rilevanza di qualsiasi outreach con dati contestuali
- **Social** (18-19): sfruttano attività LinkedIn ed engagement sui contenuti
- **Product-led** (20-24) e **Expansion** (25-26): richiedono product usage data → **FUORI SCOPE ATTUALE**, vedi sezione finale

---

## Signal-Based Plays

I plays signal-based superano costantemente il cold outreach di 2x-10x. Priorità a questi quando esiste un segnale chiaro e tempestivo.

### 1. Website Visitor De-anonymization
**Segnale**: un'azienda o persona visita il sito — specie pagine ad alto intento (pricing, integrazioni, enterprise)
**Come funziona**: tool di de-anonimizzazione identifica le aziende (a volte i contatti) in visita. Arricchisci con Clay. Scora con AI. Tier 1 → Slack per cold call immediata; Tier 2-3 → sequenze email/LinkedIn automatiche.
**Tool**: Warmly, RB2B, Apollo, CommonRoom, Koala (de-anon); Clay (enrichment); Instantly / HeyReach (sequenze)
**Difficoltà**: Beginner
**Best for**: tutte le motion
**Pro-tip**: non dire "ti ho visto sulla pagina pricing". Riferisciti al tema sottostante (scalare le vendite, ridurre il churn) in modo naturale.

### 2. Competitor Displacement via Tech Stack
**Segnale**: l'azienda usa un competitor o tool complementare (via BuiltWith, job posting, intent data)
**Come funziona**: costruisci una lista di aziende che usano uno stack specifico. Arricchisci con i contatti rilevanti. Campagna di displacement/espansione su un use case o pain point legato a quello stack.
**Tool**: BuiltWith, Theirstack, Sumble (tech signals); Clay; Apollo (contatti)
**Difficoltà**: Intermediate
**Best for**: Sales-led, marketing-led
**Pro-tip**: i job posting sono un ottimo proxy dello stack — un ruolo Data Engineer che menziona Snowflake rivela lo stack anche se BuiltWith non lo rileva.

### 3. Look-alike Targeting (Closed-won Similarity)
**Segnale**: l'azienda combacia col profilo dei closed-won recenti
**Come funziona**: estrai i closed-won dal CRM. Usa l'AI per capire cosa condividono (settore, dimensione, stack, hiring, growth signals). Costruisci una lista look-alike e fai cold outreach sui loro profili.
**Tool**: Clay, Apollo (list building); ChatGPT (pattern matching); CRM
**Difficoltà**: Intermediate
**Best for**: Sales-led, marketing-led

### 4. Job Change of Champions
**Segnale**: un champion passato (contatto closed-won) si sposta in una nuova azienda ICP-fit
**Come funziona**: traccia quando i contatti dei closed-won cambiano lavoro. Quando atterrano in un'azienda ICP-fit, contattali — conoscono già il prodotto e diventano champion interni.
**Tool**: Champify, UserGems, Clay, CommonRoom, Koala
**Difficoltà**: Beginner
**Best for**: tutte le motion
**Pro-tip**: invia un piccolo gift di benvenuto nel nuovo ruolo — automatizzabile con Postal, Reachdesk, Sendoso.

### 5. LinkedIn Engagement (Own Content)
**Segnale**: una persona ICP-fit ha messo like/commento/repost a un contenuto LinkedIn del tuo team
**Come funziona**: traccia l'engagement sui post dei dipendenti con Trigify. Profile visitor con Teamfluence. Webhook verso Clay. Qualifica e arricchisci. Enroll in sequenze a tier in base al lead score.
**Tool**: Trigify (engagement), Teamfluence (profile visitor), Clay, Findymail, HeyReach / Instantly
**Difficoltà**: Intermediate
**Best for**: Marketing-led, sales-led
**Dato**: le connessioni LinkedIn dei founder — play affine — hanno generato un 25,4% di reply rate (Workflows.io, 2025).

### 6. LinkedIn Connections of Founders/Execs
**Segnale**: persona connessione di 1° grado di un founder/exec E ICP-fit
**Come funziona**: esporta nativamente le connessioni LinkedIn (no tool extra). Qualifica azienda e persona con Clay. Scora con ChatGPT. Tier 1 → cold call, Tier 2-3 → email + LinkedIn automatici. Messaggio conversazionale: si sono già scaldati sui contenuti.
**Tool**: LinkedIn (export nativo), Clay, ChatGPT, HubSpot, Instantly, HeyReach
**Difficoltà**: Beginner
**Best for**: tutte le motion

### 7. Social Listening (Keyword Monitoring)
**Segnale**: persona ICP-fit interagisce con post LinkedIn contenenti keyword rilevanti (nome competitor, pain point, keyword di categoria)
**Come funziona**: Clay monitora LinkedIn per keyword specifiche. Cattura chi interagisce. Arricchisce contatto e azienda. ChatGPT qualifica l'ICP fit. Assegna a sequenze in base allo score.
**Tool**: Clay (keyword + enrichment), ChatGPT, HubSpot, HeyReach, Instantly, Findymail
**Difficoltà**: Intermediate
**Best for**: Marketing-led, sales-led

### 8. Relevant Job Postings
**Segnale**: l'azienda pubblica un ruolo che segnala il bisogno di ciò che vendi o l'uso di una tecnologia
**Come funziona**: monitora le job board per i ruoli rilevanti. Quando un'azienda pubblica un ruolo target (es. VP Sales per un vendor di sales tool; Data Engineer + Snowflake per un data product), innesca outreach alla buyer persona giusta.
**Tool**: Clay, Theirstack, Sumble
**Difficoltà**: Intermediate
**Best for**: Sales-led, marketing-led
**Esempio**: un vendor di candidate database scansiona gli account target ogni giorno. Quando uno cerca un AE, manda al VP Sales 3 candidati pre-vagliati con "se ne vuoi altri così, ti faccio un tour".

### 9. Geo/Event-based Outreach
**Segnale**: conferenza/evento imminente o recente, o milestone cittadina rilevante per l'ICP
**Come funziona**: lista ICP-filtered di prospect in una città o a un evento. Personalizza l'outreach usando l'evento come motivo per connettersi di persona o riconoscere un contesto condiviso.
**Tool**: Apollo (liste geo); Clay (enrichment)
**Difficoltà**: Beginner
**Best for**: Sales-led

---

## Warm Outbound Plays

Targettano persone con relazione, brand awareness o prossimità di network pregressa. Richiedono meno trust-building del cold.

### 10. Customer Alumni
**Segnale**: la persona ha lavorato in un account closed-won ed è passata a una nuova azienda ICP-fit
**Come funziona**: estrai i closed-won dal CRM. Con Clay trova chi ci lavorava. Qualifica l'azienda attuale. Scora con ChatGPT. Tier 1 → prospecting manuale, Tier 2-3 → email + LinkedIn automatici.
**Tool**: HubSpot, Clay, ChatGPT, Instantly, HeyReach
**Difficoltà**: Intermediate
**Best for**: Sales-led, marketing-led

### 11. Closed-lost Reopen (cadenza 9 mesi)
**Segnale**: opportunità persa esattamente 9 mesi fa
**Come funziona**: automazione CRM segnala i closed-lost al 9° mese. Tier 1 → notifica all'owner, Step 1 manuale. Altri → sequenza automatica. OpenAI API riassume l'ultima call e inserisce una riga personalizzata ("per rinfrescarti la memoria, avevamo parlato di…").
**Tool**: HubSpot o qualsiasi CRM (trigger nativo), OpenAI API (riassunto call), sales engagement tool
**Difficoltà**: Beginner
**Best for**: Sales-led
**Pro-tip**: il riassunto della call è un hook fortissimo — dimostra che li ricordi senza essere generico.

### 12. Champion Tracking (job change — tutti i buyer)
**Segnale**: qualsiasi buyer persona chiave nel CRM cambia azienda — non solo i closed-won
**Come funziona**: traccia ogni contatto CRM che combacia con una buyer persona chiave e cambia lavoro. Outreach automatico per dargli il benvenuto e capire se userebbe di nuovo il prodotto nella nuova azienda.
**Tool**: Champify, Clay, CommonRoom, Koala, UserGems
**Difficoltà**: Beginner
**Best for**: tutte le motion

### 13. Warm Intro via Investor/Advisor comuni
**Segnale**: l'account target condivide un investor, advisor o cliente comune
**Come funziona**: mappa il network di investor/advisor contro la lista account target. Identifica i warm path. Richiedi intro o segnala gli account ai rep per Sales Navigator.
**Tool**: Cabal, Commsor, The Swarm (network mapping); Sales Navigator
**Difficoltà**: Intermediate
**Best for**: Early-stage sales-led; efficace anche in growth per Tier 1

### 14. Ex-colleghi di nuovi flagship customer
**Segnale**: un nuovo flagship customer ha appena firmato — i suoi ex-colleghi possono essere ICP-fit
**Come funziona**: alla chiusura di un deal-landmark, lookup automatico di dove i contatti chiave hanno lavorato prima. Trova ex-colleghi ora in aziende ICP-fit. Outreach citando la connessione comune.
**Tool**: Clay, LinkedIn
**Difficoltà**: Intermediate
**Best for**: Sales-led

---

## Personalization Plays

Aumentano la rilevanza di qualsiasi outreach con dati contestuali. Funzionano meglio sopra una strategia di targeting signal-based.

### 15. Pre-call Research Brief
**Segnale**: primo meeting prenotato nel CRM
**Come funziona**: prima della prima call, pull automatico di un brief sul prospect — news recenti, intel competitiva, attività LinkedIn, milestone, ruoli aperti. Consegnato al rep via Slack/CRM.
**Tool**: Clay, ChatGPT, HubSpot, Slack
**Difficoltà**: Intermediate
**Best for**: Sales-led
**Nota collettivo**: questo è esattamente ciò che fa la nostra `skills/account-research/`.

### 16. Account-specific Landing Pages
**Segnale**: account target in una sequenza attiva
**Come funziona**: landing page dinamiche personalizzate su azienda, settore e pain point del prospect. Linkate dalle email outbound come CTA primaria.
**Tool**: Mutiny, Intellimize
**Difficoltà**: Advanced
**Best for**: Sales-led (Tier 1), marketing-led at scale

### 17. 1:1 Video Outreach (automatizzato)
**Segnale**: account target in sequenza attiva — tipicamente Tier 1 o 2
**Come funziona**: video brevi personalizzati che citano il nome azienda, uno screenshot del sito o un pain point specifico. Tool AI-assisted semi-automatizzano la produzione a scala.
**Tool**: Sendspark, Vidyard, Loom
**Difficoltà**: Intermediate
**Best for**: Sales-led (Tier 1/2)

---

## Social Plays

### 18. LinkedIn Connection Request con Content Reference
**Segnale**: persona ICP-fit, nessuna connessione LinkedIn esistente
**Come funziona**: campagna di connection request che cita un post specifico con cui la persona ha interagito — o un tuo post — come motivo per connettersi.
**Tool**: HeyReach, Expandi, Dripify
**Difficoltà**: Beginner
**Best for**: Sales-led, marketing-led

### 19. Influencer/Creator Audience Prospecting
**Segnale**: creator LinkedIn attivo nel tuo spazio ICP che genera engagement rilevante
**Come funziona**: identifica persone ICP-fit che sono creator LinkedIn attivi o con seguito. Costruisci una lista prospect dalla loro audience ingaggiata (liker, commenter, follower).
**Tool**: Clay, Trigify
**Difficoltà**: Advanced
**Best for**: Marketing-led, aziende content-heavy

---

## Quick Reference: GTM Motion → Plays migliori

### Sales-led (SDR/AE outbound)
Parti da: website de-anon (#1), LinkedIn connections founder (#6), closed-lost reopen (#11), champion tracking (#12)
Stratifica: social listening (#7), competitor displacement (#2), job postings (#8), LinkedIn engagement (#5)
Avanzato: look-alike (#3), warm intro (#13), video personalizzato (#17), customer alumni (#10)

### Marketing-led (inbound + content)
Parti da: LinkedIn engagement own content (#5), LinkedIn connections founder (#6), closed-lost reopen (#11)
Stratifica: social listening (#7), look-alike (#3), champion tracking (#12)
Avanzato: influencer/creator prospecting (#19), account-specific landing pages (#16)

### Product-led / Hybrid
I plays PLG-specifici sono in Future State (sotto). Nel frattempo i plays cross-motion utili: website de-anon (#1), champion tracking (#12), LinkedIn engagement (#5).

---

## Quick Reference: Stage azienda → Sofisticazione

### Early (pre-1M ARR, <10 dipendenti)
1-2 plays max. Usa dati esistenti. Non over-engineerizzare.
Migliori fit: closed-lost reopen (#11), LinkedIn connections founder (#6), website visitor (#1), champion tracking (#12), job postings (#8)

### Growth (1-20M ARR, 10-100 dipendenti)
3-5 plays in parallelo. Inizia a stratificare segnali e costruire lo stack.
Aggiungi: LinkedIn engagement (#5), social listening (#7), job postings (#8), customer alumni (#10)

### Scaling (20M+ ARR, 100+ dipendenti)
Signal stack completo. Micro-campagne (50-250 contatti, specifiche e rinfrescate spesso). Segnali impilati per lead scoring a tier.
Aggiungi: look-alike (#3), warm intro (#13), account-specific landing pages (#16), + plays PLG/expansion se applicabili

---

# FUORI SCOPE ATTUALE — Future State

> I plays seguenti richiedono **product usage data del cliente** (PLG/hybrid). Fuori dallo scope outbound-for-hire early-stage del collettivo. **Non includerli nelle raccomandazioni di default** — proponili solo se il cliente avrà accesso ai dati di prodotto e ha una motion PLG/hybrid. Mantenuti qui per completezza del catalogo.

## Product-led Plays

### 20. PQL Outbound (End User + Decision Maker)
**Segnale**: un utente raggiunge una soglia PQL (es. completa un evento di attivazione chiave)
**Come funziona**: al rilevamento del PQL, tre azioni automatiche: (1) il PQL entra in una sequenza info-gathering, (2) altri end user nella stessa azienda vengono identificati e aggiunti a sequenze, (3) i decision maker vengono trovati e aggiunti a una sequenza DM-specifica. Outbound multi-threaded sull'account.
**Tool**: Apollo, Clay, CommonRoom, Koala (contatti); data warehouse + reverse-ETL (Census/Hightouch)
**Difficoltà**: Advanced
**Best for**: PLG, hybrid PLG

### 21. Non-user Expansion (account esistente)
**Segnale**: l'account ha 1+ utenti ma molti potenziali utenti non adottati
**Come funziona**: identifica i non-user dentro account che hanno già utenti. Outreach con use case o angolo di team — o segnala l'account a un rep per expansion.
**Tool**: Product data + CRM; Apollo
**Difficoltà**: Intermediate
**Best for**: PLG, hybrid PLG

### 22. Aha Moment Trigger
**Segnale**: account free/trial raggiunge una milestone di attivazione chiave
**Come funziona**: quando un admin raggiunge l'aha moment, innesca outreach di vendita per convertirlo a paid, citando la sua azione in-product.
**Tool**: instrumentation + CRM; Pocus, Koala, CommonRoom; sales engagement tool
**Difficoltà**: Intermediate
**Best for**: PLG

### 23. High-intent Page Visit (utente di prodotto esistente)
**Segnale**: un utente di prodotto esistente (free/trial) visita una pagina ad alto intento — pricing, integrazioni, enterprise
**Come funziona**: quando un utente noto visita una pagina ad alto intento, innesca outreach all'admin/decision maker citando l'interesse specifico.
**Tool**: visitor tracking + product data; CRM; Warmly
**Difficoltà**: Intermediate
**Best for**: PLG, hybrid PLG

### 24. Multi-domain Roll-up (Exec Buyer)
**Segnale**: più account o signup dallo stesso parent domain/organizzazione
**Come funziona**: quando più utenti dalla stessa org sono identificati, innesca una campagna verso un exec buyer per consolidare in un deal enterprise.
**Tool**: CRM (roll-up detection); Clay; sales engagement tool
**Difficoltà**: Intermediate
**Best for**: PLG, hybrid PLG

## Expansion Plays

### 25. Usage Limit Approaching
**Segnale**: l'uso dell'account (seat, credit, API call) si avvicina al limite di piano
**Come funziona**: outreach programmatico all'admin quando l'uso si avvicina al limite. Alto ACV → notifica Slack all'Account Manager. Basso ACV → automazione completa.
**Tool**: Product data + CRM; Pocus, Koala, CommonRoom; sales engagement tool
**Difficoltà**: Intermediate
**Best for**: PLG, hybrid PLG

### 26. Free Trial di Upsell Package
**Segnale**: l'account inizia un trial di un tier/package superiore
**Come funziona**: all'avvio dell'upsell trial, innesca una sequenza che offre setup assistance, training o check-in call per massimizzare trial-to-paid.
**Tool**: Product data + CRM; sales engagement tool
**Difficoltà**: Beginner
**Best for**: PLG, hybrid PLG
