---
name: sales-deck-creator
description: Crea Sales Deck professionali pronti per Gamma a partire da descrizioni grezze di prodotti o servizi. Applica un framework completo di posizionamento, storytelling e struttura slide. Usa quando l'utente dice "crea un sales deck per", "trasforma in sales deck", "prepara il deck per", "sales deck per [prodotto]". Do NOT use for investor deck, pitch deck per investitori, o presentazioni interne non commerciali.
license: MIT
metadata:
  author: utente
  version: 1.0.0
---

## Overview

Questa skill trasforma informazioni grezze e disordinate su un prodotto/servizio in un Sales Deck strutturato, pronto per essere copiato su Gamma e generare le diapositive. Applica un framework professionale che copre posizionamento, storytelling, pain points, social proof e struttura narrativa.

## Instructions

### Step 1: Leggi i file di reference

Prima di generare qualsiasi contenuto, leggi TUTTI i file nella cartella `references/`:

1. `references/01-elementi-essenziali.md` — Gli 8 elementi che ogni buon Sales Deck deve avere
2. `references/02-cosa-non-fare.md` — Errori ricorrenti da evitare e flag di allarme
3. `references/03-fondamenti-posizionamento.md` — Come posizionare il prodotto tra le alternative
4. `references/04-struttura-sales-deck.md` — I 12 "pezzi del puzzle": struttura slide-by-slide

Questi file contengono il framework completo, le linee guida, i criteri di qualita e le regole di valutazione. Applicali integralmente.

Opzionalmente consulta `references/esempio-sales-deck.pdf` come riferimento visivo di un deck reale ben fatto.

### Step 2: Raccogli le informazioni dall'utente

Chiedi all'utente di incollare le informazioni sul prodotto/servizio. Possono essere grezze, disordinate, incomplete. Accetta qualsiasi formato.

Se le info sono troppo scarse per costruire un deck efficace, fai domande mirate su:
- **Cosa fa il prodotto** (categoria, use case principale)
- **Per chi e** (target/ICP: chi ha il problema che risolve)
- **Cosa sostituisce** (alternativa attuale: tool, processo, workaround)
- **In cosa e migliore** (differenziazione rispetto alle alternative)
- **Dati disponibili** (metriche, case study, social proof, numeri)
- **Pricing/offerta** (se disponibile e se il cliente vuole includerlo)

### Step 3: Analisi e posizionamento

Prima di scrivere le slide, analizza le informazioni ricevute applicando i fondamenti di posizionamento (file 03):

1. Valuta la **maturita del mercato** (immaturo/emergente/maturo)
2. Identifica il **livello di consapevolezza del buyer**
3. Definisci i **4 elementi di posizionamento**: cos'e, per chi e, cosa sostituisce, in cosa e migliore
4. Identifica il **POV** (opinione sul mercato) piu efficace
5. Individua i **pain points reali** del segmento target
6. Seleziona l'**ECP** (Early Customer Profile) corretto

Condividi questa analisi con l'utente in modo sintetico prima di procedere, per validarla.

### Step 4: Genera il Sales Deck

Genera il deck seguendo la struttura dei 12 pezzi del puzzle (file 04), adattandola al caso specifico. Non tutte le slide sono obbligatorie: alcune si possono comprimere, saltare o espandere in base al contesto.

**Formato output per ogni slide:**

```
## Slide [N]: [Titolo della slide]

[Descrizione concisa del contenuto — 2-3 frasi che spiegano cosa comunicare in questa slide]

- Bullet point 1
- Bullet point 2
- Bullet point 3
```

**Struttura tipo (adattabile):**

1. **Cover** — Nome prodotto/azienda + tagline
2. **Company Profile** — Biglietto da visita rapido e credibile
3. **Insight sul mercato** — Cosa sta cambiando, dato che cattura attenzione
4. **Problema + POV** — Cosa non funziona + la vostra opinione sul mercato
5. **Status Quo (Old Way)** — Come si fa oggi e perche crea limiti
6. **Alternative disponibili** — Cosa puo scegliere il cliente oggi e i limiti
7. **Scenario ideale (New Way)** — Come dovrebbe essere il nuovo modo
8. **Introduzione alla soluzione** — Il prodotto come risposta naturale
9-11. **Capacita + Benefici** — Cosa permette di fare + vantaggi (2-4 slide)
12. **Demo** (opzionale) — Riferimento a demo/screenshot se disponibili
13. **Trust & Proof** — Social proof, dati, testimonianze, KPI
14. **Offerta & Pricing** — Cosa offri e a che prezzo (se applicabile)
15. **FAQ / Obiezioni** — Risposte alle domande tipiche
16. **Next Step** — Prossimi passi chiari e azionabili

### Step 5: Verifica qualita

Prima di consegnare, verifica il deck contro questa checklist (derivata dai file 01 e 02):

**DEVE avere:**
- [ ] Chiarezza estrema (linguaggio diretto, semplice, comprensibile)
- [ ] Narrazione empatica (connessione, non solo informazione)
- [ ] Contesto di mercato prima del prodotto (mai partire dal prodotto)
- [ ] POV chiaro e motivato
- [ ] Pain points reali e specifici del segmento
- [ ] Capacita e benefici separati dalle feature
- [ ] Social proof / dati concreti
- [ ] Storytelling problema-soluzione
- [ ] Next step chiarissimi

**NON deve avere:**
- [ ] Zero contesto (prodotto troppo presto)
- [ ] Sovraccarico di feature
- [ ] Linguaggio da investor deck
- [ ] Tecnicismi inutili
- [ ] Mancanza di alternative
- [ ] Mancanza di proof points
- [ ] Obiezioni non anticipate

### Step 6: Consegna

Presenta il deck completo in un unico blocco nella conversazione.

Subito dopo, invia automaticamente il contenuto a Gamma tramite il workflow n8n usando il Bash tool con Python:

```python
import urllib.request, json, sys

deck_content = """INCOLLA_QUI_IL_TESTO_COMPLETO_DEL_DECK"""

payload = json.dumps({"deck_content": deck_content}).encode("utf-8")
req = urllib.request.Request(
    "https://stefano1479.app.n8n.cloud/webhook/sales-deck-to-gamma",
    data=payload,
    headers={"Content-Type": "application/json"},
    method="POST"
)
try:
    res = urllib.request.urlopen(req, timeout=10)
    print("✓ Deck inviato a Gamma:", res.read().decode())
except Exception as e:
    print("✗ Errore invio a Gamma:", e)
```

Sostituisci `INCOLLA_QUI_IL_TESTO_COMPLETO_DEL_DECK` con il testo del deck generato. Dopo l'invio, comunica all'utente che Gamma sta elaborando la presentazione (tempo stimato: 30-60 secondi) e che potrà trovarla nel suo workspace Gamma.

Se l'utente chiede modifiche, itera mantenendo la coerenza del framework e reinvia il deck aggiornato al webhook.

## Examples

### Esempio 1: Prodotto SaaS B2B

**Input utente:** "Ho un software che automatizza la gestione del catalogo prodotti per eCommerce. Usiamo AI per generare descrizioni, ottimizzare SEO e tradurre in 50 lingue. I nostri clienti risparmiano il 90% del tempo. Abbiamo case study con +160% click e +30% vendite."

**Output atteso:** Deck di 14-16 slide che parte dal contesto (costi acquisizione in crescita, cataloghi non ottimizzati), passa al problema (pagine prodotto scarse = soldi persi), presenta il POV (il PIM non basta piu, serve un motore di crescita), introduce la soluzione come naturale evoluzione, mostra capacita/benefici con dati concreti, e chiude con proof points e next step.

### Esempio 2: Servizio consulenziale

**Input utente:** "Faccio consulenza strategica per PMI che vogliono internazionalizzarsi. Ho 15 anni di esperienza, ho aiutato 40 aziende a entrare in nuovi mercati. Il mio approccio si basa su analisi di mercato + rete di partner locali."

**Output atteso:** Deck che parte dallo scenario (PMI italiane perdono opportunita internazionali), identifica il problema (approccio fai-da-te fallisce nell'80% dei casi), mostra le alternative (fiere, agenzie generiche, fare da soli) e i loro limiti, presenta il metodo come new way, e chiude con case study e next step.

## Troubleshooting

### "Le info che ho sono troppo poche"
**Soluzione:** La skill fara domande mirate sui 4 elementi di posizionamento. Bastano risposte brevi per costruire un deck iniziale da iterare.

### "Il deck sembra generico"
**Causa:** Probabilmente mancano dati specifici (numeri, case study, nomi clienti).
**Soluzione:** Aggiungi anche solo 2-3 dati concreti. Il framework li posizionera nei punti giusti.

### "Non ho social proof / dati"
**Soluzione:** La skill suggerira alternative: testimonianze informali, metriche di processo, confronti qualitativi. Un deck senza proof e debole ma comunque strutturabile.

### "Voglio un deck piu corto / piu lungo"
**Soluzione:** I 12 pezzi sono modulari. Specifica quante slide vuoi e la skill comprimera o espandera di conseguenza, mantenendo il filo logico.
