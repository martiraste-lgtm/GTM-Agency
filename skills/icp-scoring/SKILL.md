---
name: icp-scoring
description: Qualifica e assegna tier A/B/C a una lista di account. Input: lista di aziende (CSV, testo, o URL). Output: lista scored con tier e motivazione per account. Trigger: "score questa lista", "qualifica questi account", "assegna il tier a [lista]".
license: MIT
metadata:
  author: GTM Collective (adattato da KarlRaf/gtm-starter-kit)
  version: 1.0.0
---

## Overview

Applica i criteri di `context/icp-definition.md` a una lista di account e assegna tier A/B/C con score e motivazione. Leggi `context/icp-definition.md` prima di iniziare.

---

## Instructions

### Step 1 — Input

Ricevi la lista di account. Formati accettati:
- Testo libero (nomi aziende o domini)
- CSV con colonne: company, domain, size, industry, role (se disponibili)
- Lista da LinkedIn Sales Nav

### Step 2 — Applica lo scoring

Per ogni account, applica i criteri da `context/icp-definition.md`:

**Criteri standard** (adattare se questo è un repo cliente con ICP diverso):

| Criterio | Punti |
|----------|-------|
| ARR/dimensione nel range ICP primario | +20 |
| ARR/dimensione nel range ICP secondario | +10 |
| Modello B2B con ciclo vendita medio | +15 |
| Founder ancora coinvolto nel sales | +10 |
| No team GTM strutturato | +10 |
| Segnale di urgenza attivo | +20 |
| Trazione visibile (hiring, news, funding) | +10 |
| Anti-ICP match (uno qualsiasi) | -50 |

**Soglie tier**:
- Tier A: 60+ punti
- Tier B: 35-59 punti
- Tier C: sotto 35 punti

### Step 3 — Output

Per ogni account:
```
[Nome azienda] | Tier [A/B/C] | Score: [N]
Motivazione: [perché questo tier — 1 riga]
Prossima azione: [immediata per A, settimanale per B, monitoraggio per C]
```

Salva in: `outputs/YYYY-MM-DD-scoring-[nome-lista].md`

---

## Troubleshooting

**Dati insufficienti per scorare**: assegna Tier C di default e nota "dati insufficienti — ricercare prima di procedere".
**Tutti Tier C**: problema di targeting nella lista di partenza, non nello scoring. Rivedi la fonte della lista.
