---
name: mkt1-marketing-strategy-setup
description: Meta-skill che orchestra l'intero processo di strategia marketing MKT1. Introduce i framework core (Fuel & Engine, 3 Strategy Driver, Wedge Strategy) e guida nella sequenza corretta delle skill MKT1. Trigger: "imposta la strategia marketing", "strategia MKT1", "da dove inizio con la strategia", "mkt1 setup", "costruiamo la strategia marketing".
license: MIT
metadata:
  author: GTM Collective (adattato da framework MKT1 — Emily Kramer / Kathleen Estreich)
  version: 2.0.0
---

## Overview

Questa skill non produce un output diretto — introduce i framework fondamentali MKT1, spiega come si collegano tra loro, e guida nella sequenza di skill da eseguire. Usala all'inizio di ogni nuovo engagement cliente, o quando si deve riorientare la strategia.

---

## I 3 Framework Core MKT1

Prima di eseguire qualsiasi skill, è fondamentale capire questi 3 concetti — sono la base di tutto il sistema.

---

### Framework 1 — Fuel & Engine

**Fuel** = il contenuto e le creatività distribuite attraverso i canali  
**Engine** = i canali e i meccanismi di targeting che distribuiscono il Fuel

**Regola critica**: Fuel e Engine devono essere allineati tra loro E con i Strategy Driver. Un grande Fuel sul canale sbagliato non funziona. Un buon Engine senza Fuel di qualità non produce risultati.

Esempi di Fuel: report di settore, case study, framework originale, webinar, template, newsletter  
Esempi di Engine: outbound email, LinkedIn, SEO/content organico, paid ads, eventi, community, partner

Il sistema MKT1 aiuta a scegliere il Fuel e l'Engine giusti in base al contesto specifico — non in astratto.

---

### Framework 2 — I 3 Strategy Driver

La strategia marketing è determinata da 3 driver interconnessi. Vanno analizzati in sequenza:

**Driver 1 — Product Marketing Strategy**
- Chi è il vostro ICP (audience prioritaria)?
- Quali segmenti sono "proven", "scaling", "testing", "non prioritari"?
- Come si posiziona il prodotto rispetto ai competitor e all'ecosistema?
- Qual è l'allineamento con la roadmap di prodotto?

**Driver 2 — GTM Motion**
- Qual è la motion principale? (SLG, PLG, PLS, hybrid)
- Il buying process dell'audience supporta self-serve o richiede sales?
- L'ACV medio indica self-serve (< ~10K/anno) o sales-led (> ~10K/anno)?
- I canali marketing sono allineati alla motion scelta?

**Driver 3 — Marketing Advantages**
- Quali dinamiche nel business, prodotto o mercato accelerano intrinsecamente la crescita?
- Quali dei 9 Marketing Advantages sono presenti e sfruttabili?
- Sono amplificati dalla strategia attuale o sottoutilizzati?

I 3 driver determinano il Fuel giusto e l'Engine giusto. Senza averli analizzati, le scelte di canale e contenuto sono congetture.

---

### Framework 3 — Wedge Strategy

La Wedge Strategy è il principio che guida il GTM nelle fasi early: **cattura prima una nicchia specifica (il wedge), poi espandi**.

Perché funziona:
- Identifica dove il prodotto offre un'esperienza 10x migliore degli alternative
- Permette di diventare esperti di quel segmento (Fuel altamente specifico)
- Evita il "marketing del pitch deck" — messaggi ampi che cercano tutti e convincono nessuno

**I 6 step della Wedge Strategy:**

1. **Trova il wedge** — identifica il segmento dove hai l'esperienza 10x (audience + use case specifico)
2. **Identifica tutti i prospect** — mappali sistematicamente nel CRM, raggiungi quanti più possibile
3. **Diventa esperto di materia** — crea Fuel specifico per quel segmento (template, framework, thought leadership)
4. **Raggiungi l'audience target** attraverso 3 canali:
   - Outbound: contenuto value-add mirato (per SLG)
   - Inbound: contenuto altamente rilevante che attrae (per PLG)
   - Ecosystem: partnership con chi ha già accesso a quell'audience
5. **Personalizza l'esperienza** — landing page, onboarding, sales enablement per il wedge
6. **Pianifica l'espansione** senza perdere il focus attuale

**Due modelli di espansione dal wedge:**
- **Land & Expand**: stessa audience, più use case
- **Vertical Expansion**: stesso use case, audience diverse

Esempi storici: Carta (founder → investitori), Toast (booking → POS completo), Stripe (developer API → fintech infrastructure)

**Attenzione**: una Wedge Strategy non significa rifiutare gli altri segmenti. Permetti crescita organica come segnale di validazione del prossimo wedge.

---

## Sequenza delle skill MKT1

Esegui in questo ordine. Ogni skill alimenta la successiva.

```
1. mkt1/company-overview         ← documenta i 3 Strategy Driver (fondamenta)
       ↓
2. mkt1/marketing-advantages     ← identifica i 9 advantage disponibili
       ↓
3. mkt1/perceptions              ← definisce le 3-4 narrative strategiche (Fuel tematico)
       ↓
4. mkt1/channel-strategy         ← determina Engine giusto per questo contesto
       ↓
5. mkt1/revenue-levers           ← prioritizza dove concentrare lo sforzo adesso
       ↓
6. mkt1/big-bets                 ← progetta 1-3 campagne Fuel + Engine coordinate
       ↓
7. mkt1/gaccs                    ← brief operativo per ogni Big Bet
```

---

## Quando usare solo un subset

| Scenario | Skill minime |
|----------|--------------|
| Nuovo cliente, zero dati | 1 → 2 → 3 → 4 |
| Cliente con ICP già chiaro | 2 → 3 → 5 → 6 |
| Lancio campagna specifica | 6 → 7 |
| Review strategia esistente | 2 → 3 → 5 (verifica alignment) |
| Solo brief per team | 7 |
| Definire il wedge iniziale | 1 → 4 (con focus Wedge Strategy) |

---

## ICP Tiering (da usare in company-overview)

Quando si analizzano i segmenti audience, usa questo schema di tiering:

| Tier | Definizione | Effort marketing |
|------|-------------|-----------------|
| **Proven** | Segmento validato — conversione confermata, best-fit | Priorità massima, scala qui |
| **Scaling** | Segmento in crescita — trazione iniziale, da consolidare | Investimento significativo |
| **Testing** | Segmento in esplorazione — ipotesi da validare | Risorse limitate, test rapidi |
| **Not a priority** | Fuori focus per ora — potenziale futuro ma non ora | Zero investimento attivo |

Ogni cambio di tier richiede buy-in cross-funzionale (marketing, sales, product).

---

## Come collegare gli output al sistema

| Skill MKT1 | Aggiorna nel repo |
|-----------|----------|
| company-overview | `context/profile.md`, `context/icp-definition.md` |
| marketing-advantages | `context/positioning.md` |
| perceptions | `content/narrative.md`, `content/pillars.md` |
| channel-strategy | `signals/signal-routing.md`, `outbound/sequences/` |
| revenue-levers | `kpi/dashboard.md` |
| big-bets | `outbound/campaigns/big-bets.md` |
| gaccs | `outbound/campaigns/YYYY-MM-DD-gaccs-[nome].md` |

---

## Note operative

- **Non combinare più skill in una sola sessione** se si lavora in profondità — ognuna richiede focus specifico
- **Company overview e marketing advantages** sono le più time-intensive. Dagli il tempo giusto.
- **Perceptions** è il layer più sottovalutato e il più differenziante. Non saltarlo.
- **GACCS** è la skill più veloce e quella usata più frequentemente (prima di ogni campagna)
- **Pianifica il prossimo wedge mentre esegui quello attuale** — non aspettare che sia esaurito
