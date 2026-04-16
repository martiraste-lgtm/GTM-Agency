# Playbook: Risposta a Nuovo Segnale

*Cosa fare quando viene rilevato un segnale su un account target. Esegui in sequenza.*

---

## Trigger

Hai rilevato un segnale su un'azienda nel tuo ICP (funding round, hiring, lancio prodotto, ecc.)

---

## Step 1 — Classifica l'account (5 minuti)

```
È già nostro cliente? → SÌ: stop, segnala al team
È in trattativa attiva? → SÌ: passa all'owner del deal
Contattato negli ultimi 45 giorni? → SÌ: cooldown, riprendi dopo
```

Se no a tutto → continua.

---

## Step 2 — Score il segnale (2 minuti)

Consulta `signals/signal-library.md`:
1. Identifica il codice segnale (S01, S02, ecc.)
2. Calcola lo score con il decay corretto (giorni dalla rilevazione)
3. Verifica se ci sono segnali combinati attivi sullo stesso account (+50%)
4. Assegna il tier: A (25+), B (15-24), C (8-14)

---

## Step 3 — Research rapido (10-20 minuti per Tier A)

Esegui `skills/account-research/`:

```
Read skills/account-research/SKILL.md and research [company.com]
```

Oppure manualmente:
- LinkedIn aziendale: dimensione, hiring recente, post fondatori
- Sito web: prodotto, clienti, positioning
- Crunchbase: funding history, investor, team
- Google: news ultimi 30 giorni

Salva in: `outbound/account-research/YYYY-MM-DD-[nome-azienda].md`

---

## Step 4 — Costruisci il messaggio (15-30 minuti)

Usa `skills/signal-to-sequence/` oppure manualmente:

1. Scegli la persona giusta (da `context/personas/`)
2. Scegli il canale (LinkedIn DM vs email — dipende dalla persona e dal segnale)
3. Seleziona la sequenza più pertinente da `outbound/sequences/`
4. Personalizza il primo messaggio con:
   - Riferimento esplicito al segnale (specifico, non generico)
   - Collegamento al problema che quel segnale implica
   - Value proposition in max 2 righe
   - CTA leggera (domanda, non "prenota una call")

**Regola d'oro**: il primo messaggio deve dimostrare che hai fatto i compiti, non che vuoi vendere qualcosa.

---

## Step 5 — Lancia e traccia

1. Importa in Instantly / Smartlead
2. Aggiorna `kpi/dashboard.md` (aggiunto a campagna X)
3. Registra in `outbound/campaigns/` se è una campagna nuova

---

## Step 6 — Gestione risposta

**Reply positivo** → vai a `playbooks/proposal-to-close.md`
**Reply neutro** ("non ora", "mandami info") → nurture: aggiungi a sequenza a 30 giorni
**Reply negativo** → segna come "non interessato" + cooldown 6 mesi
**Nessuna risposta a sequenza completa** → registra in campaign results + attendi nuovo segnale

---

## Timing consigliato

- Tier A: contatta entro **48 ore** dal rilevamento del segnale
- Tier B: entro la settimana
- Tier C: aggiungere alla lista mensile, monitorare

Ricorda: lo stesso segnale vale 2x di più nei primi 30 giorni. Il timing è parte della strategia.
