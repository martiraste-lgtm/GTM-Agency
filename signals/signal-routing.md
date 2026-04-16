# Signal Routing — Albero decisionale

*Quando un segnale viene rilevato, segui questo albero per decidere cosa fare.*

---

## Step 1 — Classificazione account

Prima di agire su un segnale, classifica l'account:

```
È un nostro cliente attuale?
├── SÌ → Sopprimi. Segnala al team per upsell se rilevante.
└── NO → continua

È un'opportunità attiva (in trattativa)?
├── SÌ → Passa all'AE/founder responsabile. Non contattare in autonomia.
└── NO → continua

Abbiamo già contattato questo account negli ultimi 45 giorni?
├── SÌ → Cooldown. Aspetta altri 45 giorni prima di riprendere.
└── NO → continua

L'account è nel nostro ICP?
├── NO o INCERTO → Esegui `skills/icp-scoring/` prima di procedere
└── SÌ → vai allo Step 2
```

---

## Step 2 — Scoring e tier

```
Score totale del segnale (vedi signal-library.md):
├── 25+ punti → Tier A → azione immediata (entro 48h)
├── 15-24 punti → Tier B → azione entro la settimana
├── 8-14 punti → Tier C → aggiungere alla lista mensile
└── sotto 8 punti → monitorare, non agire ancora
```

Se l'account ha **due segnali concorrenti** attivi: upgrade automatico al tier superiore.

---

## Step 3 — Azione per tier

### Tier A (azione entro 48h)

1. Esegui `skills/account-research/` sull'account
2. Identifica il canale migliore (LinkedIn DM vs email — vedi persona)
3. Seleziona la sequenza corretta da `outbound/sequences/` in base a:
   - Segnale rilevato
   - Persona target
   - Settore
4. Personalizza il primo messaggio con il segnale specifico
5. Lancia e traccia in `outbound/campaigns/`

### Tier B (azione entro la settimana)

1. Aggiungi l'account alla coda settimanale
2. Esegui `skills/account-research/` in batch
3. Assegna alla sequenza più pertinente
4. Lancia nel prossimo ciclo campagna

### Tier C (lista mensile)

1. Aggiungi a una lista di monitoraggio
2. Ricontrolla ogni 30 giorni — il segnale potrebbe aggiornare o scadere
3. Se arriva un secondo segnale → upgrade a Tier B automatico

---

## Step 4 — Dopo il primo contatto

```
Reply ricevuto?
├── Positivo (interesse) → Passa a `playbooks/proposal-to-close.md`
├── Neutro (non ora, richiesta info) → Nurture: aggiungi a sequenza follow-up a 30 giorni
├── Negativo (no grazie) → Segna come "non interessato" + aggiungi cooldown 6 mesi
└── Nessuna risposta dopo sequenza completa → Segnala in `outbound/campaigns/` come "no reply"
    → Ricontatta solo se arriva nuovo segnale forte (Tier A)
```

---

## Metriche da tracciare per ogni campagna

Dopo ogni campagna, registra in `outbound/campaigns/`:

- Segnale usato come trigger
- Persona contattata
- Canale (email / LinkedIn)
- N° contatti raggiunti
- Open rate (email) / Acceptance rate (LinkedIn)
- Reply rate totale
- Reply positivi
- Meeting booked
- Note qualitative (obiezioni ricorrenti, feedback, tono delle risposte)

Questi dati alimentano la `skills/brain-update/`.
