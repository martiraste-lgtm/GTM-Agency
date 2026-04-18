---
name: mkt1-marketing-strategy-setup
description: Meta-skill che orchestra l'intero processo di strategia marketing MKT1. Guida nella sequenza corretta delle 7 skill MKT1 e produce una mappa strategica completa. Trigger: "imposta la strategia marketing", "strategia MKT1", "da dove inizio con la strategia", "mkt1 setup", "costruiamo la strategia marketing".
license: MIT
metadata:
  author: GTM Collective (adattato da framework MKT1 — Emily Kramer / Kathleen Estreich)
  version: 1.0.0
---

## Overview

Questa skill non produce un output diretto — è l'orchestratore che spiega quale skill MKT1 eseguire, in quale ordine, e perché. Il framework MKT1 funziona in sequenza: ogni layer alimenta il successivo. Saltare passaggi produce output superficiali.

Usala all'inizio di ogni nuovo engagement cliente, o quando si deve riorientare la strategia.

---

## Instructions

### Step 1 — Valutazione contesto

Prima di scegliere la sequenza, chiedi:

1. **Cosa abbiamo già?** Check veloce: context/profile.md esiste e ha dati reali? context/icp-definition.md è compilato?
2. **Qual è la fase attuale?** (pre-seed / seed / serie A / growth)
3. **Qual è il trigger di questa sessione strategica?** (nuovo cliente, riorientamento, nuova fase, nuova linea di prodotto)
4. **Quanto tempo abbiamo?** (sessione 1h = si fa un layer; progetto completo = si fanno tutti)

### Step 2 — Sequenza consigliata

Esegui le skill in questo ordine. Ogni skill produce un output che diventa input della successiva.

```
1. mkt1_company_overview       ← fondamenta: stage, modello, audience, competitive
       ↓
2. mkt1_marketing_advantages   ← cosa rende QUESTO business unico nel marketing
       ↓
3. mkt1_perceptions            ← 3-4 credenze strategiche che vogliamo nel mercato
       ↓
4. mkt1_channel_strategy       ← qual è il channel mix giusto per questo contesto
       ↓
5. mkt1_revenue_levers         ← dove concentrare lo sforzo adesso (prioritizzazione)
       ↓
6. mkt1_big_bets               ← 1-3 campagne coordinate che muovono il needle
       ↓
7. mkt1_gaccs                  ← brief di allineamento per ogni big bet / campagna
```

### Step 3 — Quando usare solo un subset

Non è sempre necessario fare tutto. Regola pratica:

| Scenario | Skill minime |
|----------|--------------|
| Nuovo cliente, zero dati | 1 → 2 → 3 → 4 |
| Cliente con ICP già chiaro | 2 → 3 → 5 → 6 |
| Lancio campagna specifica | 6 → 7 |
| Review strategia esistente | 2 → 3 → 5 (verifica alignment) |
| Solo brief per team | 7 |

### Step 4 — Come collegare gli output al sistema

Ogni skill MKT1 salva il suo output in una cartella specifica del repo. Dopo ogni sessione, i file in `context/` e `content/` devono riflettere gli output aggiornati:

| Skill | Aggiorna |
|-------|----------|
| company_overview | `context/profile.md`, `context/icp-definition.md` |
| marketing_advantages | `context/positioning.md` (sezione vantaggio) |
| perceptions | `content/narrative.md`, `content/pillars.md` |
| channel_strategy | `signals/signal-routing.md`, `outbound/sequences/` |
| revenue_levers | `kpi/dashboard.md` (sezione priorità) |
| big_bets | `outbound/campaigns/big-bets.md` |
| gaccs | `outbound/campaigns/YYYY-MM-DD-gaccs-[nome].md` |

---

## Note operative

- **Non combinare più skill in una sola sessione** se si lavora in profondità — ogni skill richiede focus e dati specifici.
- **Company overview e marketing advantages** sono le skill più time-intensive. Dagli il tempo giusto.
- **Perceptions** è il layer più sottovalutato e il più differenziante. Non saltarlo.
- **GACCS** è la skill più veloce e quella usata più frequentemente (prima di ogni campagna).
