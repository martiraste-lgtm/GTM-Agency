---
name: mkt1-big-bets
description: Progetta 1-3 Big Bets — campagne coordinate ad alto impatto che combinano Marketing Advantages, Perceptions e ICP in un'unica iniziativa coerente. Alternativa alle tattiche sparse che producono rumore senza risultati. Trigger: "big bets", "campagne strategiche", "iniziative ad alto impatto", "mkt1 big bets", "pianifica le campagne principali", "cosa fare nei prossimi 6 mesi".
license: MIT
metadata:
  author: GTM Collective (adattato da framework MKT1 — Emily Kramer / Kathleen Estreich)
  version: 1.0.0
---

## Overview

Le startup disperdono l'energia su 10-15 tattiche parallele e ottengono risultati marginali su tutto. I Big Bets sono l'opposto: 1-3 iniziative ad alto impatto, ognuna con un obiettivo chiaro, un'audience specifica, un canale primario e un pezzo di contenuto/fuel che le alimenta. Non è una campagna singola — è un sistema coordinato che spinge la stessa Perception su più touchpoint contemporaneamente.

Prerequisiti: `mkt1_marketing_advantages` + `mkt1_perceptions` + `mkt1_channel_strategy`.
Output: `clients/[nome]/outbound/campaigns/big-bets.md` — piano delle campagne principali del trimestre/semestre.

---

## Instructions

### Step 1 — Definizione di Big Bet

Un Big Bet ha 4 componenti obbligatorie:

| Componente | Definizione |
|-----------|-------------|
| **Fuel** | Il contenuto, insight o asset che alimenta la campagna (es. report di settore, caso studio, webinar, framework originale) |
| **Engine** | Il canale o meccanismo di distribuzione principale (es. outbound email, LinkedIn, evento, partner) |
| **Audience** | Il segmento ICP specifico che questa campagna vuole raggiungere (non "tutte le startup", ma "CTO di startup SaaS HR-tech con round seed negli ultimi 60 giorni") |
| **Perception** | Quale delle 3-4 Perceptions strategiche questa campagna rafforza |

Senza uno di questi 4, non è un Big Bet — è una tattica.

### Step 2 — Quante Big Bets

| Stage | N. Big Bets consigliati |
|-------|------------------------|
| Seed / early | 1 (massima concentrazione) |
| Serie A | 1-2 |
| Growth | 2-3 |

**Regola**: se stai pensando a 4+, stai pianificando tattiche, non Big Bets. Torna a ridurre.

### Step 3 — Processo di ideazione

Per ogni Big Bet, rispondi a queste domande in sequenza:

1. **Quale Perception vogliamo rafforzare con questa campagna?** (scegli dalla lista definita con `mkt1_perceptions`)
2. **Chi è l'audience specifica?** (segmento ICP + segnale che li qualifica + momento temporale)
3. **Qual è il Fuel?** (cosa produciamo che vale la pena di consumare — non una landing page, ma un insight reale)
4. **Qual è l'Engine?** (come distribuiamo il Fuel all'Audience — outbound, LinkedIn, evento, partner)
5. **Cosa fa il buyer dopo il primo contatto?** (sequenza di azioni che vogliamo che compia)
6. **Come misuri il successo?** (metrica principale + target a 90 giorni)

### Step 4 — Template per ogni Big Bet

```
BIG BET [N]: [Titolo della campagna]

Perception target: [quale delle Perceptions strategiche rafforza]
Audience: [segmento ICP specifico + segnale qualificante]
Fuel: [tipo di contenuto o asset — cosa produciamo]
Engine: [canale primario di distribuzione]
Sequenza attesa:
  1. [Prima azione del buyer]
  2. [Seconda azione]
  3. [Conversione target]
KPI: [metrica principale] → target: [numero] entro [data]
Risorse necessarie: [chi fa cosa, in quanto tempo]
```

### Step 5 — Validazione del Big Bet

Prima di procedere, verifica che ogni Big Bet superi questi criteri:

- [ ] Il Fuel è qualcosa che il buyer trova genuinamente utile o interessante (non solo noi)
- [ ] L'Engine raggiunge davvero l'Audience (non "in teoria", ma concretamente)
- [ ] La Perception target è differenziante — un competitor potrebbe fare la stessa campagna? Se sì, rivedila
- [ ] Il team ha le risorse per eseguirla bene — preferibile 1 Big Bet ben fatto a 3 mediocri
- [ ] C'è un timing logico (perché farlo adesso?)

### Step 6 — Prioritizzazione tra Big Bets

Se hai 2-3 Big Bets, ordina per:
1. **Impatto potenziale** sul revenue lever prioritario (output `mkt1_revenue_levers`)
2. **Velocità di esecuzione** (quale puoi lanciare prima?)
3. **Utilizzo degli Advantages** (quale sfrutta meglio i Marketing Advantages disponibili?)

### Step 7 — Output

Salva il documento completo in `clients/[nome]/outbound/campaigns/big-bets.md` (non in outputs/ — è un documento operativo permanente, aggiornato ogni trimestre).

Struttura del file:
```
# Big Bets — [trimestre/periodo]
Aggiornato: [data]

## Big Bet 1: [titolo]
[template compilato]

## Big Bet 2: [titolo] (se applicabile)
[template compilato]

## Priorità di esecuzione
[quale si lancia prima e perché]
```

---

## Esempi

**Big Bet efficace**: "Report sullo stato dell'outbound B2B in Italia 2026" (Fuel) distribuito via LinkedIn e cold email (Engine) a founder di startup SaaS serie A che hanno assunto un Head of Sales negli ultimi 30 giorni (Audience), per rafforzare la Perception "chi parte dalle campagne sbaglia l'ordine".

**Big Bet debole**: "Serie di contenuti LinkedIn sul GTM" — non ha Audience specifica, il Fuel è generico, non rafforza una Perception precisa.

---

## Troubleshooting

**"Non abbiamo un Fuel da produrre"**: il Fuel non deve essere un report da 50 pagine. Può essere: 5 dati originali da una survey rapida, un framework semplice in 1 slide, un caso studio di 300 parole. Il criterio è "qualcosa che il buyer trova utile", non "qualcosa di lungo".

**"Vogliamo fare tutto"**: usa il filtro "quale Big Bet, se funzionasse, cambierebbe il risultato del trimestre da solo?" — quello è il candidato primario.
