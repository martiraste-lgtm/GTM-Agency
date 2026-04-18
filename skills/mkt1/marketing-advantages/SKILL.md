---
name: mkt1-marketing-advantages
description: Identifica i Marketing Advantages unici del business — le risorse, capacità o posizioni che rendono il marketing di questa azienda più efficace di quello dei competitor. Non sono vantaggi generici: sono specifici, difficili da copiare, e cambiano quali canali e tattiche funzionano. Trigger: "marketing advantages", "cosa ci rende unici nel marketing", "vantaggi competitivi marketing", "perché il nostro marketing funziona meglio", "mkt1 advantages".
license: MIT
metadata:
  author: GTM Collective (adattato da framework MKT1 — Emily Kramer / Kathleen Estreich)
  version: 1.0.0
---

## Overview

I Marketing Advantages sono la risposta alla domanda: "Cosa rende il marketing di questa azienda *slealmente* efficace rispetto ai competitor?" Non è positioning — è un inventario di asset reali che il marketing può sfruttare. Chi li identifica bene sa dove investire il tempo e il budget. Chi li ignora replica playbook generici e ottiene risultati medi.

Prerequisito: `mkt1_company_overview` completato.
Output: aggiorna `context/positioning.md` con la sezione Marketing Advantages.

---

## Instructions

### Step 1 — Inventario degli asset di marketing

Passa in rassegna queste 10 categorie di Marketing Advantages. Per ognuna, chiedi: "Ce l'abbiamo? In che misura? È difficile da copiare?"

| Categoria | Domanda diagnostica |
|-----------|---------------------|
| **Distribuzione** | Hai un canale di distribuzione unico o privilegiato? (partner, marketplace, community propria) |
| **Dati proprietari** | Hai accesso a dati che altri non hanno e che puoi usare per messaggi più rilevanti? |
| **Brand e reputazione** | Il tuo brand è già riconosciuto nel segmento? Hai founder con visibilità pubblica? |
| **Community** | Hai una community attiva di utenti, prospects o partner che amplificherà i tuoi messaggi? |
| **Ecosistema / integrazioni** | Stai dentro un ecosistema (es. Salesforce, Slack, Shopify) con access privilegiato? |
| **Effetti di rete** | Il prodotto diventa più utile con più utenti? Questo crea referral naturali? |
| **Expertise di categoria** | Hai thought leadership reale nel settore? Il founder è una voce riconosciuta? |
| **Contenuto / SEO** | Hai già asset di contenuto che portano traffico o credibilità? |
| **Velocità e agilità** | Sei più veloce dei competitor nel rispondere ai trend di mercato? |
| **Modello di pricing / accesso** | Il tuo modello (freemium, trial, open source) ti dà un vantaggio di acquisizione? |

### Step 2 — Prioritizzazione

Dai ogni advantage presente uno score su 2 dimensioni:
- **Forza** (1-3): quanto è solido e difendibile?
- **Sfruttabilità ora** (1-3): quanto è facile attivarlo con le risorse attuali?

**Score totale** = Forza × Sfruttabilità. I top 2-3 sono i Marketing Advantages prioritari.

### Step 3 — Implicazioni strategiche

Per ognuno dei 2-3 advantage prioritari, definisci:
- **Come si attiva** (quale tattica, canale o formato lo sfrutta meglio)
- **Come si mantiene** (cosa serve per non perderlo nel tempo)
- **Come si comunica** (come diventa parte del messaging e delle perceptions)

### Step 4 — Red flag

Verifica che i Marketing Advantages identificati siano reali, non desiderati:
- "Vogliamo costruire una community" ≠ "abbiamo una community" — il futuro non conta
- "Il CEO è brillante" ≠ advantage a meno che abbia già audience o visibilità misurabile
- Un advantage che tutti i competitor hanno = non è un advantage

### Step 5 — Output

Scrivi i Marketing Advantages in forma concisa:
```
Advantage 1: [Nome]
Descrizione: [cosa è concretamente]
Prova: [dato o evidenza che lo conferma]
Come si attiva: [tattica specifica]

Advantage 2: ...
```

Salva in `outputs/YYYY-MM-DD-marketing-advantages-[cliente].md`.
Aggiorna `context/positioning.md` con una sezione "Marketing Advantages".

---

## Esempi

**Advantage forte**: startup HR tech con 200 case study di clienti Fortune 500 — il content advantage è enorme (social proof + SEO).  
**Advantage debole identificato male**: "il nostro team ha esperienza nel settore" — tutti i competitor dicono lo stesso.  
**Advantage inaspettato**: il CEO è attivo su LinkedIn con 40K follower nel target ICP — è un distribution advantage sottovalutato.

---

## Troubleshooting

**"Non abbiamo nessun advantage"**: tutti i business ne hanno almeno uno. Spesso è nascosto: il founder sa cose che i competitor non sanno, c'è accesso a un segmento specifico, o il modello di pricing è più accessibile.

**Troppi advantage**: se ne emergono 6-7, stai elencando feature, non advantage. Torna al filtro "difficile da copiare in 6 mesi?" — se non passa, non è un advantage.
