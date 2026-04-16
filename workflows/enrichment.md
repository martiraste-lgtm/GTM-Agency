# Workflow: Data Enrichment

*Come costruire liste qualificate e arricchire i dati prima dell'outreach.*

---

## Cascata di enrichment (ordine di priorità)

### Livello 1 — Fonti gratuite (sempre)
- **LinkedIn Sales Navigator**: ricerca per settore, dimensione, ruolo, geo
- **LinkedIn company page**: hiring, post recenti, team size
- **Sito web**: prodotto, clienti citati, tech stack visibile
- **Google**: news recenti, PR, menzioni

### Livello 2 — Tool mid-range
- **Apollo.io**: database contatti, email finder, job changes
- **Crunchbase (free tier)**: funding, team size, investor
- **Hunter.io**: verifica email, email finder

### Livello 3 — Tool avanzati (per Tier A)
- **Clay**: enrichment automatico multi-source, webhook, scoring
- **Crunchbase Pro**: funding details, investor list, funding timeline
- **LinkedIn Sales Nav avanzato**: signal detection hiring, intent

### Livello 4 — Proprietario (col tempo)
- **knowledge/**: pattern su quale segmento converte meglio
- **outbound/campaigns/**: risultati storici per segmento

---

## Dati minimi per outreach (Tier A)

| Campo | Fonte | Obbligatorio |
|-------|-------|--------------|
| Nome e cognome | LinkedIn | Sì |
| Email verificata | Apollo / Hunter | Sì |
| Azienda + sito | LinkedIn | Sì |
| Ruolo esatto | LinkedIn | Sì |
| Dimensione azienda | LinkedIn / Crunchbase | Sì |
| Segnale specifico | Fonte segnale | Sì |
| Settore | LinkedIn | Sì |
| Funding recente | Crunchbase | Se rilevante |
| Hiring recente | LinkedIn | Se rilevante |
| Tech stack | BuiltWith / job posting | Consigliato |

---

## Come usare Clay per signal-based enrichment

1. Crea una table con i criteri ICP (settore, dimensione, geo)
2. Aggiungi colonna "Segnale" collegata a Crunchbase webhook (funding) o LinkedIn (hiring)
3. Configura scoring automatico: score = somma dei segnali attivi per ogni account
4. Esporta in Instantly/Smartlead solo gli account con score > soglia Tier A

**Automazione consigliata**: webhook Crunchbase → Clay → Instantly → alert Slack quando score > 25

---

## Quality check lista

Prima di importare in qualsiasi tool outbound:
- [ ] Bounce rate stimato < 5% (verifica email con NeverBounce o simili)
- [ ] Nessun cliente attuale nella lista
- [ ] Nessun account in cooldown (contattato negli ultimi 45 giorni)
- [ ] Ogni account ha almeno un segnale valido (non scaduto)
- [ ] Ruolo corrispondente alla persona target
