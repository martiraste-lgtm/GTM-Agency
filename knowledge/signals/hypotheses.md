# Segnali — Ipotesi in Test

*Segnali che stiamo testando. Non ancora confermati. Aggiornare dopo ogni campagna.*

---

## Come leggere questo file

Ogni ipotesi ha:
- **Ipotesi**: cosa ci aspettiamo
- **Segnale**: quale trigger stiamo testando
- **Test iniziato**: data
- **Prove finora**: quante campagne hanno usato questo segnale
- **Risultati parziali**: cosa stiamo vedendo
- **Prossimo step**: quando e come confermare/confutare

---

*Nessuna ipotesi attiva ancora.*

---

## Template per nuova ipotesi

```
### H[N] — [Nome ipotesi]
**Ipotesi**: il segnale [X] porta a reply rate superiore al baseline [Y%] nel segmento [Z]
**Segnale**: [codice da signal-library.md]
**Test iniziato**: [DATA]
**Prove finora**: [N]/3 campagne
**Risultati parziali**: reply rate [X%] su [N] contatti
**Prossimo step**: [cosa fare per confermare]
**Promuovere a confirmed se**: 3 campagne con reply rate > [soglia]
```
