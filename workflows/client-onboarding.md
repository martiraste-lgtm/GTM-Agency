# Workflow: Client Onboarding

*Come si adatta questo sistema per un nuovo cliente. Dalla firma alla prima campagna.*

---

## Pre-requisiti

- Preventivo firmato
- Accesso confermato: dominio email, LinkedIn, CRM (se esiste), tool outbound
- Kick-off call schedulata

---

## Step 1 — Fork del repo (Giorno 0)

```bash
# Clona questo repo come base
git clone [URL questo repo] client-[nome-cliente]
cd client-[nome-cliente]

# Disconnetti dal repo collettivo e inizializza nuovo
rm -rf .git
git init
git remote add origin [URL nuovo repo privato cliente]
```

**File da aggiornare subito dopo il fork:**
- `CLAUDE.md` → cambia "Chi siamo" con il profilo del cliente
- `context/profile.md` → descrizione prodotto, team, clienti attuali cliente
- Svuota `knowledge/` (tutti i file confermati/hypotheses/graveyard → lascia solo la struttura)
- Svuota `outbound/campaigns/` e `outputs/`

---

## Step 2 — Setup automatico (Giorno 1-2)

Esegui la skill di setup sul dominio del cliente:

```
Read skills/setup/SKILL.md and set up this repo for [dominio-cliente.com]
```

Claude ricerca automaticamente:
- Sito web e prodotto
- LinkedIn aziendale e fondatori
- Crunchbase (funding, team size)
- Job posting recenti
- Competitor menzionati o impliciti
- Tech stack (G2, BuiltWith, job posting)

→ Popola `context/profile.md`, `context/icp-definition.md` (prima bozza), `context/competitor-radar.md`

**Tempo stimato**: 30-60 minuti

---

## Step 3 — Kick-off call (Giorno 3-5)

**Domande da fare in kick-off** (integrano ciò che Claude non può trovare online):

1. Chi è il cliente che ha portato più valore al vostro business fino ad oggi? Perché?
2. Quali deal avete perso? Perché hanno scelto un'altra soluzione?
3. Qual è l'obiezione più frequente nelle prime call?
4. Quali verticali volete attivare per primi?
5. Avete già provato outbound? Cosa ha funzionato / non funzionato?
6. Quali strumenti avete già (CRM, email, LinkedIn)?
7. Chi gestirà le call di discovery con i prospect? (founder? sales interno? noi?)

→ Affina `context/icp-definition.md` e `context/positioning.md` con le risposte

---

## Step 4 — Positioning Sprint (Settimana 1-2)

Esegui `skills/b2b-positioning-diagnostic/` con il cliente:

```
Read skills/b2b-positioning-diagnostic/SKILL.md e facilita il positioning sprint per [nome cliente]
```

→ Al termine, esegui il workflow `workflows/positioning-to-assets.md`:
- Aggiorna `signals/signal-library.md` con segnali specifici per il loro ICP
- Crea `outbound/sequences/message-house.md`
- Prepara brief per homepage e deck

---

## Step 5 — Setup infrastruttura (Settimana 2-3, in parallelo)

- [ ] Registra 2-3 domini dedicati per cold email
- [ ] Configura SPF, DKIM, DMARC su ogni dominio
- [ ] Imposta warm-up (4-6 settimane per piena deliverability)
- [ ] Configura stack outbound (Instantly / Smartlead)
- [ ] Configura LinkedIn outreach (HeyReach / Expandi)
- [ ] Importa/crea CRM base (HubSpot o equivalente)
- [ ] Imposta webhook per signal detection (Crunchbase, LinkedIn)

---

## Step 6 — Prima campagna (Settimana 4-5)

1. Esegui `skills/icp-scoring/` sulla prima lista di prospect
2. Seleziona Tier A (score 60+) — priorità assoluta
3. Esegui `skills/account-research/` sui top 20 account Tier A
4. Usa `skills/signal-to-sequence/` per costruire la prima campagna
5. Lancia e traccia in `outbound/campaigns/`

---

## Step 7 — Weekly cadence (da Settimana 1 in poi)

**Ogni lunedì:**
- Esegui `skills/weekly-update/` — aggiorna context/ e kpi/dashboard.md
- Review metriche campagne attive
- Decisioni e next step

**Dopo ogni campagna (2-4 settimane):**
- Esegui `skills/brain-update/` — aggiorna knowledge/
- Identifica ipotesi da testare nel ciclo successivo

---

## Checklist onboarding completato

- [ ] Repo forkato e rinominato
- [ ] `context/` popolato (profile, icp, positioning, competitor, personas)
- [ ] Positioning sprint completato
- [ ] Signal library creata con segnali specifici per ICP cliente
- [ ] Infrastruttura email impostata (domini + warm-up avviato)
- [ ] Prima sequenza costruita e lanciata
- [ ] KPI baseline registrato in `kpi/dashboard.md`
- [ ] Weekly cadence avviata
