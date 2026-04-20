---
name: mkt1-channel-strategy
description: Determina il miglior channel mix in base a stage aziendale, audience, GTM motion e Marketing Advantages. Usa il framework dei 6 Growth Engine e i 10 Channel Pairing per costruire una strategia multi-canale coordinata invece di copiare il playbook di altri. Trigger: "channel strategy", "quali canali usare", "dove investire nel marketing", "channel mix", "mkt1 channel", "quali canali per il GTM", "channel startup fit".
license: MIT
metadata:
  author: GTM Collective (adattato da framework MKT1 — Emily Kramer / Kathleen Estreich)
  version: 2.0.0
---

## Overview

Il problema più comune nella scelta dei canali: copiare quello che fanno gli altri o credere al mito del "singolo canale magico". La realtà: ogni startup ha una combinazione unica di prodotto, audience e GTM motion che determina quali canali funzionano. E nessun canale singolo è sufficiente — la strategia più difendibile combina canali che si rinforzano a vicenda.

Come afferma MKT1: "Approccio al growth strategy come costruire una squadra di basket — ogni canale è un giocatore che contribuisce al successo complessivo."

Prerequisiti: `mkt1_company_overview` + `mkt1_marketing_advantages`.
Output: aggiorna `_methodology/signals/signal-routing.md` e orienta la configurazione di `clients/[nome]/outbound/sequences/`.

---

## I 6 Growth Engine

Tutti i canali marketing rientrano in 6 categorie (Engine):

| Engine | Descrizione | Ideale per |
|--------|-------------|------------|
| **Inbound** | Contenuti e SEO che attirano prospect verso di te | Prodotti self-service, SMB, PLG |
| **Outbound** | Outreach diretto a prospect target (email, LinkedIn, cold call) | Enterprise, sales-led, SLG, ACV alto |
| **Product Virality** | Meccanismi di condivisione built-in nel prodotto | Prodotti con effetti di rete, B2B collaboration tools |
| **Events** | Webinar, conferenze, eventi dal vivo o virtuali | Prodotti che richiedono educazione o relazione umana |
| **Ecosystem** | Partnership, co-marketing, affiliate, integrazioni | Piattaforme, prodotti con ecosistema naturale |
| **Lifecycle** | Nurture, upsell, retention dei clienti esistenti | Tutti gli stage, spesso sottovalutato |

---

## 3 Filtri per scegliere i canali

### Filtro 1 — Product Marketing Research (Driver 1)

La ricerca sull'audience rivela naturalmente dove i prospect si trovano: comunità online, newsletter, eventi di settore, tool che usano (ecosystem). Se capisci i workflow del buyer, i canali emergono da soli.

Domanda chiave: "Dove vive online il nostro ICP? Dove cerca informazioni prima di comprare?"

### Filtro 2 — GTM Motion (Driver 2)

| GTM Motion | Engine prioritari | Logica |
|------------|-------------------|--------|
| **SLG** (Sales-Led) | Outbound, Events, Ecosystem | Il buyer vuole parlare con qualcuno |
| **PLG** (Product-Led) | Inbound, Product Virality, Lifecycle | L'acquisizione avviene attraverso il prodotto |
| **PLS** (Product-Led Sales) | PLG + Outbound selettivo su PQL | Il prodotto genera il lead, sales chiude |
| **Community-Led** | Ecosystem, Events, Inbound | Il flywheel è la community stessa |

### Filtro 3 — Marketing Advantages (Driver 3)

Ogni Marketing Advantage amplifica un Engine specifico:

| Advantage | Engine che amplifica |
|-----------|---------------------|
| Network Effects / Virality | Product Virality |
| Free Plan / Trial | Inbound + Product Virality |
| Wedge Strategy | Outbound (list specifica) + Inbound di nicchia |
| Integrations / Co-Marketing | Ecosystem |
| Channel Partnerships | Ecosystem |
| Forcing Function (trend/regolamentazioni) | Outbound (urgency hook) + Inbound |
| Community / Educational Content | Inbound + Events + Ecosystem |
| Founder Story / Market Fit | Outbound (founder-led) + Events + Inbound |
| Category Creation | Inbound (thought leadership) + Events |

---

## 10 Channel Pairing Strategici

Un singolo canale raramente è sufficiente. La strategia più difendibile combina 2 canali che si rinforzano. I 10 pairing più efficaci:

| Pairing | Approccio | Errore comune |
|---------|-----------|---------------|
| **Inbound + Outbound** | Follow up outbound su visitatori ad alta intent; ABM per account top-tier, inbound per SMB | Silos tra marketing e sales, mancanza di integrazione |
| **Inbound + Product Virality** | Contenuti attirano utenti iniziali, feature virali incoraggiano referral | Sovrainvestire in inbound senza aver validato i viral loop |
| **Inbound + Events** | Webinar come CTA leggero (alternativa al meeting 1:1) | Troppi CTA in homepage, cannibalizzazione conversioni |
| **Inbound + Ecosystem** | Co-creare contenuti con partner, amplificare reciprocamente | Partner che non mantengono gli impegni di distribuzione |
| **Outbound + Product Virality** | Raggiungere account grandi che guideranno alta virality | Outbound senza viral loop validati nel prodotto |
| **Outbound + Events** | Raggiungere account specifici via email con invito evento come CTA | Sovraccaricare lead con eventi di bassa qualità |
| **Outbound + Ecosystem** | Warm intro da partner; filtrare liste per tech stack (Clay) | Sovraccaricare i partner senza offrire valore reale |
| **Product Virality + Events** | Invitare high-sharers a eventi esclusivi; webinar su feature virali | Pressione eccessiva su clienti di valore |
| **Product Virality + Ecosystem** | Service provider come moltiplicatori (dashboard multi-cliente) | Marketing che ignora le opportunità di network effect nell'ecosystem |
| **Events + Ecosystem** | Co-ospitare eventi con partner per audience più ampio | Misallineamento su obiettivi e qualità bar con il partner |

---

## ACV e scelta del canale

Il valore medio del contratto (ACV) influenza il rapporto effort/ritorno:

| ACV annuale | Engine a ROI positivo |
|-------------|----------------------|
| < 5K/anno | Inbound, SEO, Product Virality, self-serve |
| 5-25K/anno | Outbound, LinkedIn, Inbound + sales assist |
| 25K+/anno | Outbound personalizzato, Events, Ecosystem (referral) |

---

## Traffic Light System — prioritizzazione continua

Dopo aver scelto i canali, usa il Traffic Light System per allocare il tempo:

| Semaforo | % tempo | Logica |
|----------|---------|--------|
| **Verde** | 70% | Canali dove stai già vedendo trazione — raddoppia |
| **Giallo** | 20% | Canali sperimentali da testare con attenzione |
| **Rosso** | 10% | Lascia perdere — non forzare canali che non funzionano |

Non iniziare mai con un mix 50/50 tra canali validati e nuovi esperimenti — diluisce i risultati su entrambi.

---

## Selezione finale

Dopo i filtri, hai 3-5 canali candidati. Scegli i top 2-3:

1. **Engine primario**: miglior rapporto tra probabilità di funzionare e risorse necessarie — 70% dello sforzo
2. **Engine secondario**: complementare al primario, diverso per formato — 20% dello sforzo
3. **Engine sperimentale** (opzionale): test controllato — 10% dello sforzo

---

## Output

```
Channel Mix — [cliente / periodo]

Engine primario: [nome]
Perché: [logica basata su audience + GTM motion + advantages]
Come si attiva: [tattiche specifiche, frequenza, KPI]
Traffic Light: Verde (dobbiamo scalarlo) / Giallo (stiamo testando)

Engine secondario: [nome]
Perché: [logica]
Come si attiva: [tattiche]

Channel pairing scelto: [es. Outbound + Events]
Logica pairing: [come si rinforzano]

Engine sperimentale: [nome o "nessuno per ora"]
```

Salva in `outputs/YYYY-MM-DD-channel-strategy-[cliente].md`.
Aggiorna `_methodology/signals/signal-routing.md` con i canali selezionati come output dei trigger.

---

## Principio critico

"Layering multiple channels together over time is the most defensible strategy, especially as engines and channels are changing rapidly due to AI and automation."

Non cercare il canale magico. Costruisci una combinazione che si rafforza nel tempo.

---

## Troubleshooting

**"Vogliamo fare tutto"**: applica il filtro ACV. Se è sotto 10K, non puoi permetterti Engine ad alta intensità di sales. Se è sopra 30K, l'inbound organico non converte abbastanza veloce.

**"Abbiamo sempre fatto X"**: verifica se era realmente quel canale o la rete personale del founder. Se il canale era "referral da rete diretta", non è scalabile — è un Network Effect personale che si esaurisce.

**Canali in silos**: se inbound e outbound sono gestiti da persone diverse senza coordinazione, i risultati calano. I pairing funzionano solo se i team si parlano e condividono i dati.
