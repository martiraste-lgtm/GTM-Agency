---
name: mkt1-marketing-advantages
description: Identifica i Marketing Advantages del business — le dinamiche nel prodotto, nel business model o nel mercato che, se sfruttate, accelerano la crescita in modo slealmente efficace. Framework originale MKT1 con 9 advantage in 3 categorie. Trigger: "marketing advantages", "cosa ci rende unici nel marketing", "vantaggi competitivi marketing", "perché il nostro marketing funziona meglio", "mkt1 advantages".
license: MIT
metadata:
  author: GTM Collective (adattato da framework MKT1 — Emily Kramer / Kathleen Estreich)
  version: 2.0.0
---

## Overview

I Marketing Advantages sono "dinamiche nel business, nel prodotto o nel mercato di un'azienda che, quando sfruttate, guidano la crescita in modo intrinseco." Non sono punti di differenziazione generici — sono asset reali che rendono il marketing più efficace di quello dei competitor, spesso in modo difficile da copiare.

Principio critico: **senza Marketing Advantages, una startup non può vincere nel marketing**. Se non ne hai, devi aggiustare il prodotto, la business strategy o l'approccio GTM.

Prerequisito: `mkt1_company_overview` completato.
Output: aggiorna `context/positioning.md` con la sezione Marketing Advantages.

---

## I 9 Marketing Advantages (framework MKT1)

### Categoria 1 — Product-Led Growth

**1. Network Effects o Product Virality**
- **Virality**: gli utenti condividono il prodotto internamente o esternamente come parte naturale dell'uso
- **Network effects**: il prodotto diventa più utile all'aumentare degli utilizzatori (advantage più forte della virality)
- Esempio: Slack (network effects interni), Calendly (virality esterna)

**2. Free Plan o Trial**
Il prodotto ha una versione gratuita che permette agli utenti di sbloccare valore prima dell'acquisto. Richiede un "trigger" di conversione a pagamento (scadenza tempo, limite utenti, feature gate). Fondamentale che il free plan non canibalizzi il paid.

**3. Wedge into a Larger Market**
Il prodotto entra in un segmento specifico (nicchia) con l'obiettivo di conquistare un mercato più ampio nel tempo. Richiede un piano di espansione dal wedge iniziale verso altri audience o use case. Vedi: Carta (cap table → equity management), Stripe (API developer → fintech infrastruttura).

---

### Categoria 2 — Market / Ecosystem

**4. Integrations / Co-Marketing**
Il prodotto ha partner naturali nell'ecosistema — e questo crea opportunità di co-marketing. Si può sfruttare la distribuzione dei partner anche senza collaborazione diretta (es. content marketing sui loro prodotti, presence nelle loro marketplace).

**5. Channel Partnerships & Sales**
È possibile far sì che altri attori dell'ecosistema promuovano o vendano il prodotto in cambio di commissioni, referral bonus o sconti. Richiede incentivazione dei partner e materiali di enablement marketing dedicati.

**6. Forcing Function: Trend o Regolamentazioni**
Dinamiche esterne che creano urgenza d'acquisto naturale. I trend di mercato (es. adozione AI, crisi finanziarie) rendono il messaging più rilevante. Le nuove regolamentazioni sono forcing function ancora più potenti perché creano scadenze non negoziabili.

---

### Categoria 3 — Brand & Story

**7. Audience che cerca Community o Contenuto Educativo**
Il pubblico target è sottodotato di contenuti educativi di qualità o di spazi di connessione tra pari. Trattare community e content marketing come un "prodotto" — non come tattiche — per costruire crescita top-of-funnel organica e difendibile.

**8. Founder Story o Founder/Market Fit**
Il founder ha già relazioni, credibilità o personal brand consolidati con il target audience. I founder con following esistenti diventano canali di distribuzione diretti. Questo advantage è difficile da forzare — o esiste o non esiste.

**9. Capacità di Creare/Possedere una Categoria**
Il prodotto occupa uno spazio completamente nuovo, non sostituendo prodotti esistenti ma definendo una nuova categoria. Se il brand diventa sinonimo della categoria (es. "fare Zoom"), il vantaggio competitivo è strutturale.

---

## Instructions

### Step 1 — Inventario

Per ognuno dei 9 advantage, chiedi: "Ce l'abbiamo? In che forma? È reale (non solo desiderato)?"

Usa questa griglia:

| Advantage | Presente? | Forza (1-3) | Sfruttato ora? | Note |
|-----------|-----------|-------------|----------------|------|
| Network Effects / Virality | | | | |
| Free Plan / Trial | | | | |
| Wedge → Larger Market | | | | |
| Integrations / Co-Marketing | | | | |
| Channel Partnerships | | | | |
| Forcing Function | | | | |
| Community / Educational Content | | | | |
| Founder Story / Market Fit | | | | |
| Category Creation | | | | |

### Step 2 — Valutazione e prioritizzazione

Per gli advantage presenti, valuta su 2 dimensioni:
- **Forza potenziale** (1-3): quanto può accelerare la crescita se sfruttato appieno?
- **Livello di sfruttamento attuale** (1-3): lo stai già usando o è dormiente?

Gap tra potenziale e uso attuale = priorità di attivazione.

Analizza anche: il competitor ha lo stesso advantage? Se sì, chi lo sta sfruttando meglio?

### Step 3 — Implicazioni strategiche

Per ognuno dei 2-3 advantage prioritari:
- **Come si attiva** (quale tattica, canale o formato lo sfrutta)
- **Come si mantiene e rafforza** nel tempo
- **Come alimenta le Perceptions** (quale narrativa strategica supporta)

### Step 4 — Red flag

Prima di finalizzare, verifica che gli advantage identificati siano reali:
- "Vogliamo costruire una community" ≠ "abbiamo una community" — il futuro non conta
- "Il CEO è brillante" ≠ advantage se non ha audience o visibilità misurabile
- Alcuni advantage non si possono forzare (founder story, category creation): se non esistono naturalmente, non sprecare risorse a costruirli

### Step 5 — Output

Documenta gli advantage in questo formato:

```
Advantage 1: [Nome — dalla lista MKT1]
Descrizione: [cosa è concretamente per questo business]
Evidenza: [dato o prova che lo conferma]
Forza potenziale: [1-3] | Sfruttamento attuale: [1-3]
Azione prioritaria: [come attivarlo o amplificarlo]

Advantage 2: ...
```

Salva in `outputs/YYYY-MM-DD-marketing-advantages-[cliente].md`.
Aggiorna `context/positioning.md` con la sezione "Marketing Advantages".

---

## Nota sulla creazione di advantage

Alcuni advantage sono intrinseci al modello (network effects, wedge). Altri possono essere costruiti (free plan, co-marketing con partner) se il ROI lo giustifica. Founder story e category creation sono quasi impossibili da forzare — se non sono naturali, non investire.

---

## Troubleshooting

**"Non abbiamo nessun advantage"**: ogni business ne ha almeno uno. Spesso è nascosto. Cerca: il founder ha relazioni nel settore? C'è un trend di mercato che rende il vostro prodotto urgente? Avete integrazioni con prodotti che hanno già l'audience che volete? Ricerca fino a trovarne almeno 1-2 reali.

**Troppi advantage**: se ne emergono 6+, stai descrivendo caratteristiche del prodotto, non advantage. Torna al filtro "questo crea crescita intrinseca difficile da replicare dai competitor?" — se non lo passa, non è un advantage.
