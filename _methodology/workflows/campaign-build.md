# Workflow: Campaign Build

*Come si costruisce una campagna outbound dall'audience al lancio.*

---

## Input necessari prima di iniziare

- [ ] ICP confermato (da `context/icp-definition.md`)
- [ ] Signal library aggiornata (da `signals/signal-library.md`)
- [ ] Message house disponibile (da `outbound/sequences/message-house.md`)
- [ ] Stack outbound configurato e warm-up completato

---

## Step 1 — Definizione audience

1. Scegli il segmento target (Tier A del tuo ICP)
2. Scegli il segnale trigger (da `signals/signal-library.md`)
3. Costruisci la lista con i criteri:
   - Firmografici: settore, dimensione, fase
   - Segnale: tipo + finestra temporale (es. "funding round negli ultimi 30 giorni")
   - Persona: ruolo + seniority
4. Score ogni account con `skills/icp-scoring/`
5. Approva la lista (solo Tier A e B per la prima campagna su un segmento nuovo)

**Tool consigliati**: Apollo, Clay, LinkedIn Sales Nav, Crunchbase

---

## Step 2 — Copy e sequenza

1. Seleziona l'angolo dal message house che corrisponde al segnale
2. Scrivi o adatta la sequenza (da `outbound/sequences/`)
3. Struttura standard:
   - **Email 1**: aggancio al segnale specifico + problema rilevante (max 5 righe)
   - **Email 2** (+3 giorni): differentiated value — non feature, benefit (max 4 righe)
   - **Email 3** (+5 giorni): proof point o caso d'uso specifico (max 4 righe)
   - **Email 4** (+7 giorni): follow-up diretto (2 righe: "Ha senso parlarne?")
4. Revisione copy: ogni email deve rispondere a "perché questa persona dovrebbe rispondere ORA?"

---

## Step 3 — QA pre-lancio

- [ ] Open rate checker (es. Mail Tester) — spam score <2
- [ ] Link checker — tutti i link funzionano
- [ ] Personalizzazione verificata — nessun `{{field}}` rimasto vuoto
- [ ] Tono coerente con il message house
- [ ] CTA chiara e unica per email
- [ ] Unsubscribe link presente
- [ ] Reply-to configurato correttamente

---

## Step 4 — Lancio

1. Imposta limiti giornalieri di invio (max 30-50 email/dominio/giorno in fase warm-up, 50-100 a regime)
2. Schedulare preferibilmente: martedì-giovedì, 8-10 o 14-16 (orario buyer)
3. Registra campagna in `outbound/campaigns/[DATA]-[segmento]-[segnale]/`
4. Aggiorna `kpi/dashboard.md` con campagna attiva

---

## Step 5 — Monitoraggio e ottimizzazione

**Dopo 3-5 giorni**: controlla open rate
- Se open rate <25% → problema di deliverability o oggetto → intervieni
- Se open rate >35% ma reply rate <2% → problema di copy → testa variante oggetto/prima riga

**Dopo 7-10 giorni**: controlla reply rate
- Se reply rate <2% → rivedi angolo o segmento
- Se reply rate >5% → scala la campagna

**Dopo la sequenza completa**: esegui `skills/brain-update/` con i dati della campagna

---

## Nomenclatura campagne

```
outbound/campaigns/YYYY-MM-DD-[segmento]-[segnale]/
├── brief.md        → contesto, obiettivo, audience, segnale usato
├── sequence.md     → copy completo della sequenza
└── results.md      → metriche finali + note qualitative
```
