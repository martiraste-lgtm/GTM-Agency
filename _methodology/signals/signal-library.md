# Signal Library

*Ogni segnale ha: categoria, descrizione, score, decay, fonte di rilevamento, hook per il messaggio.*
*Aggiornare con performance reali dopo ogni campagna tramite `skills/brain-update/`.*

---

## Come funziona lo scoring

**Score base (0-30 punti)**: valore al momento del rilevamento
**Decay**: lo score scende nel tempo — un segnale rilevato a 180+ giorni vale 0
**Combinazioni**: due segnali concorrenti valgono più della loro somma (+50% se entrambi attivi)

### Finestre di decay

| Giorni dalla rilevazione | Score residuo |
|--------------------------|---------------|
| 0-30 giorni | 100% |
| 31-60 giorni | 75% |
| 61-90 giorni | 50% |
| 91-180 giorni | 25% |
| 180+ giorni | 0% — rimuovere dalla lista attiva |

---

## Segnali Tier 1 (score base 25-30) — priorità massima

### S01 — Funding Round annunciato
**Score**: 30 | **Finestra ottimale**: 0-30 giorni
**Fonte**: Crunchbase, LinkedIn, PR Newswire, comunicati stampa
**Cosa indica**: budget disponibile, pressione a mostrare crescita, team in espansione
**Hook**: "Complimenti per il round. Di solito in questa fase il challenge principale passa da 'trovare il prodotto giusto' a 'costruire il sistema per scalarlo. Come state affrontando il GTM?"
**Combinazioni potenti**: S01 + S03 (hiring commercial) = score combinato massimo

### S02 — Hiring Head of Sales / VP Sales / CRO
**Score**: 28 | **Finestra ottimale**: 0-45 giorni
**Fonte**: LinkedIn job posting, LinkedIn post del founder
**Cosa indica**: la startup vuole strutturare il commerciale — hanno bisogno di qualcosa su cui lavorare da subito
**Hook**: "Ho visto che state cercando un [ruolo]. Di solito chi arriva in quel ruolo vuole avere una machine GTM funzionante da subito, non costruirla da zero. Possiamo aiutare."
**Combinazioni potenti**: S02 + S01 = segnale fortissimo

### S03 — Hiring SDR / BDR / Sales Development
**Score**: 25 | **Finestra ottimale**: 0-45 giorni
**Fonte**: LinkedIn job posting
**Cosa indica**: vogliono fare outbound ma non hanno ancora il sistema. SDR senza sistema è denaro bruciato.
**Hook**: "Costruire un team SDR senza un sistema di signals e sequenze calibrate porta spesso a risultati deludenti. Possiamo impostare l'infrastruttura prima che arrivino."

---

## Segnali Tier 2 (score base 15-24) — alta priorità

### S04 — Nuovo mercato / espansione geografica
**Score**: 22 | **Finestra ottimale**: 0-60 giorni
**Fonte**: LinkedIn post aziendale, comunicati, job posting in nuova geo
**Cosa indica**: devono acquisire clienti in un mercato che non conoscono ancora
**Hook**: "Entrare in un nuovo mercato senza outbound strutturato significa dipendere dai referral anche lì. Come state impostando l'acquisizione?"

### S05 — Lancio nuovo prodotto / feature principale
**Score**: 20 | **Finestra ottimale**: 0-60 giorni
**Fonte**: LinkedIn post, Product Hunt, blog aziendale
**Cosa indica**: momento di go-to-market attivo, bisogno di generare awareness e pipeline
**Hook**: "Il lancio è fatto. La domanda è: come trasformate l'awareness in pipeline qualificata? Noi lavoriamo esattamente su questo."

### S06 — Nuovo round di hiring generale (3+ posizioni aperte)
**Score**: 18 | **Finestra ottimale**: 0-60 giorni
**Fonte**: LinkedIn company page, Glassdoor, Indeed
**Cosa indica**: azienda in crescita, probabilmente con funding recente o revenue in crescita
**Hook**: contestualizzare su una delle posizioni aperte più rilevanti

### S07 — Post LinkedIn del founder su sfide di crescita / GTM
**Score**: 22 | **Finestra ottimale**: 0-15 giorni (segnale molto fresco)
**Fonte**: LinkedIn monitoring
**Cosa indica**: il founder sta pensando attivamente al problema — finestra di attenzione molto alta
**Hook**: rispondere direttamente al post con un commento utile, poi DM

---

## Segnali Tier 3 (score base 8-14) — media priorità

### S08 — Partecipazione a conferenza / evento di settore
**Score**: 12 | **Finestra ottimale**: 0-30 giorni (pre o post evento)
**Fonte**: LinkedIn post, evento website, speaker list
**Cosa indica**: attivi nel settore, in modalità networking e business development
**Hook**: "Ho visto che eravate a [evento]. Di solito chi partecipa a [evento] sta lavorando su [tema] — stiamo aiutando alcune startup nella stessa situazione."

### S09 — Cambio tool / stack (es. CRM migration, nuovo stack sales)
**Score**: 15 | **Finestra ottimale**: 0-45 giorni
**Fonte**: LinkedIn post, job posting che menziona tool specifici, G2 reviews
**Cosa indica**: stanno riorganizzando il loro GTM stack — momento ideale per proporre un sistema integrato
**Hook**: "Cambiare il CRM senza rivedere anche il processo di acquisizione è un'opportunità persa. Possiamo aiutare a impostare entrambi in modo integrato."

### S10 — Menzione in media / press coverage
**Score**: 10 | **Finestra ottimale**: 0-30 giorni
**Fonte**: Google Alert, Mention.com, LinkedIn
**Cosa indica**: visibilità aumentata, possibile interesse da parte del mercato
**Hook**: contestualizzare sull'articolo specifico

---

## Segnali negativi (da escludere o rimandare)

| Segnale | Azione |
|---------|--------|
| Azienda in downsizing / layoff annunciati | Rimuovere da lista attiva — non il momento |
| Founder attivo su LinkedIn con post negativi su vendor/agenzie | Approccio molto cauto, DM informale prima |
| Job posting chiuso da più di 60 giorni | Segnale scaduto, rimuovere |
| Azienda già con team GTM strutturato (5+ persone commercial) | Probabilmente Tier C — valutare caso per caso |

---

## Come aggiungere nuovi segnali

Dopo ogni campagna, esegui `skills/brain-update/` e rispondi alle domande sui segnali. Se un segnale porta reply positivi in 3+ campagne diverse, aggiungilo qui con score validato.

Template per nuovo segnale:
```
### [CODICE] — [Nome segnale]
**Score**: [0-30] | **Finestra ottimale**: [giorni]
**Fonte**: [dove si trova]
**Cosa indica**: [comportamento di acquisto]
**Hook**: "[esempio di messaggio]"
**Combinazioni potenti**: [se applicabile]
```
