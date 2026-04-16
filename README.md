# GTM Collective Brain

Sistema operativo Claude Code per GTM Engineering + Outbound with Signals.

**Isolato da**: `claude-brain` personale e `System-content-flywheel`. Zero dipendenze esterne.

---

## Setup su nuova macchina

```bash
git clone [URL repo privato] gtm-collective-brain
cd gtm-collective-brain
```

Apri Claude Code con working directory `gtm-collective-brain/` e di': **"Leggi CLAUDE.md"**.

---

## Setup per nuovo cliente

```bash
git clone [URL questo repo] client-[nome]
cd client-[nome]
rm -rf .git && git init
git remote add origin [URL nuovo repo privato cliente]
```

Poi: `Read skills/setup/SKILL.md and set up this repo for [dominio-cliente.com]`

---

## Struttura

```
CLAUDE.md          → hub centrale, leggerlo sempre
context/           → chi siamo / chi è il cliente
signals/           → signal library con scoring e routing
outbound/          → campagne, sequenze, account research
content/           → pillars narrativi e LinkedIn
kpi/               → dashboard metriche e benchmark
knowledge/         → BRAIN: pattern accumulati nel tempo
playbooks/         → guide situazionali
workflows/         → processi documentati per gli umani
skills/            → skill Claude eseguibili
outputs/           → risultati datati delle skill
```

---

## Skills principali

| Comando | Quando |
|---------|--------|
| `Read skills/setup/SKILL.md and set up this repo for [domain]` | Nuovo cliente |
| `Read skills/account-research/SKILL.md and research [company]` | Prima dell'outreach |
| `Read skills/signal-to-sequence/SKILL.md` | Segnale rilevato → campagna |
| `Read skills/preventivo/SKILL.md` | Generare un preventivo |
| `Read skills/weekly-update/SKILL.md` | Ogni lunedì |
| `Read skills/brain-update/SKILL.md` | Dopo ogni campagna |

---

## Non committare mai

- Liste contatti (dati personali)
- API keys o credenziali
- Pricing e condizioni commerciali

---

## Manutenzione

| Frequenza | Azione |
|-----------|--------|
| Ogni lunedì | `weekly-update` |
| Dopo ogni campagna | `brain-update` |
| Dopo win/loss | Aggiorna `knowledge/deals/` |
| Trimestrale | Revisione `CLAUDE.md` → promuovi pattern confermati |
