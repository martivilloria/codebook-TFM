# 05. Protocol de Codificació

## Introducció
Aquest protocol descriu el procés pas a pas per codificar les intervencions del corpus (sessions 59–78 de la 15a legislatura del Parlament de Catalunya).

---

## Pas 1 — Identificació de la unitat d'anàlisi

**Pregunta clau:** Aquesta intervenció parla de seguretat i/o immigració?

- ✅ **SÍ** → Continua al Pas 2
- ❌ **NO** → Descarta la intervenció

**Paraules clau per identificar intervencions rellevants:**

| Català | Castellà |
|--------|----------|
| immigració, immigrant, immigrat | inmigración, inmigrante |
| seguretat, inseguretat | seguridad, inseguridad |
| delinqüència, criminalitat | delincuencia, criminalidad |
| deportació, expulsió | deportación, expulsión |
| MENAs, menors estrangers | MENAs, menores extranjeros |
| islamisme, islamització | islamismo, islamización |
| invasió, onada | invasión, oleada |
| convivència, cohesió | convivencia, cohesión |

---

## Pas 2 — Identificació de l'actor

**Pregunta clau:** Qui fa la intervenció?

| Actor | Tipus | Codi aplicable |
|-------|-------|----------------|
| Aliança Catalana | Estímul | DR-01 a DR-05 |
| Vox | Estímul | DR-01 a DR-05 |
| PSC | Resposta | BD-01 a BD-06 |
| ERC | Resposta | BD-01 a BD-06 |
| Junts per Catalunya | Resposta | BD-01 a BD-06 |
| CUP | Resposta | BD-01 a BD-06 |
| Comuns Sumar | Resposta | BD-01 a BD-06 |
| PP | Resposta | BD-01 a BD-06 |

---

## Pas 3 — Aplicació de categories

### Si és un ESTÍMUL (AC o Vox):
Aplica les categories DR del fitxer 03. Una intervenció pot tenir múltiples categories.

**Arbre de decisió:**

```
Parla de criminalitat o delinqüència vinculada a immigrants?
→ SÍ: DR-01 (Securitització)

Usa metàfores de malaltia, plaga o invasió?
→ SÍ: DR-02 (Deshumanització)

Parla de col·lapse de serveis o "prioritat nacional"?
→ SÍ: DR-03 (Col·lapse del Benestar)

Parla d'islamisme, identitat occidental o amenaça cultural?
→ SÍ: DR-04 (Amenaça Civilitzacional)

Es presenta com a víctima de la censura o del "sistema"?
→ SÍ: DR-05 (Victimització)
```

### Si és una RESPOSTA (bloc democràtic):
Aplica les categories BD del fitxer 04.

**Arbre de decisió:**

```
Respon amb dades estadístiques sense proposar marc alternatiu?
→ SÍ: BD-01 (Dismissal amb dades)

Ataca la persona o el partit en lloc del missatge?
→ SÍ: BD-02 (Criminalització del missatger)

Proposa una causa estructural alternativa (retallades, capitalisme)?
→ SÍ: BD-03 (Reframing estructural)

Compara el discurs amb el feixisme o el racisme?
→ SÍ: BD-04 (Deslegitimació moral)

Accepta implícitament que la immigració és un problema a gestionar?
→ SÍ: BD-05 (Validació implícita del frame) ⚠️

Proposa una narrativa positiva basada en valors o contribució?
→ SÍ: BD-06 (Contra-narrativa de valors)
```

---

## Pas 4 — Registre a la fitxa de codificació

Per a cada unitat d'anàlisi, completa aquesta fitxa:

```
FITXA DE CODIFICACIÓ
====================
Número d'unitat: ___
Sessió plenària: 15p0__
Data de la sessió: ___________

--- ESTÍMUL ---
Actor: AC / Vox
Diputat/da: ___________
Fragment literal: "___________"
Pàgina: ___
Categories DR: DR-__ / DR-__ / DR-__

--- RESPOSTA 1 ---
Actor: ___________
Diputat/da: ___________
Fragment literal: "___________"
Pàgina: ___
Categories BD: BD-__ / BD-__
Categoria dominant: BD-__
Eficàcia: Alta / Mitjana / Baixa / Contraproduent
Compra el frame?: Sí / No / Parcialment

--- RESPOSTA 2 (si n'hi ha) ---
[repetir estructura]

--- OBSERVACIONS ---
___________
```

---

## Pas 5 — Càlcul de la fiabilitat intercoder

Per garantir la fiabilitat del codebook, es recomana que **dues persones** codifiquin les mateixes 10 unitats d'anàlisi de manera independent i es calculi l'**Índex Kappa de Cohen**.

| Valor Kappa | Interpretació |
|-------------|--------------|
| < 0.20 | Acord feble |
| 0.21 – 0.40 | Acord discret |
| 0.41 – 0.60 | Acord moderat |
| 0.61 – 0.80 | Acord substancial ✅ |
| > 0.80 | Acord quasi perfecte ✅✅ |

**Objectiu:** Kappa > 0.60

---

## Pas 6 — Construcció de la matriu comparativa

Un cop codificades totes les unitats d'anàlisi, els resultats s'introdueixen a la matriu comparativa (fitxer `matriu/matriu_comparativa.md`).

La matriu permet visualitzar:
- Quines categories DR usa cada actor (AC vs. Vox)
- Quines categories BD usa cada partit del bloc democràtic
- Quants partits compren el frame (BD-05)
- Evolució temporal: hi ha canvi d'estratègia al llarg de les sessions?

---

## Errors freqüents a evitar

| Error | Descripció | Solució |
|-------|-----------|---------|
| **Confondre BD-01 i BD-06** | Usar dades per desmentir (BD-01) vs. usar dades per construir narrativa positiva (BD-06) | Preguntar-se: proposa un marc alternatiu? |
| **Confondre BD-02 i BD-04** | Atacar el missatger (BD-02) vs. comparar amb el feixisme (BD-04) | BD-04 inclou sempre referència històrica o moral explícita |
| **Subestimar BD-05** | La validació del frame pot ser molt subtil | Preguntar-se: accepta implícitament que la immigració és un problema? |
| **Assignar DR quan no hi ha vinculació** | Parlar de seguretat sense vincular-ho a immigració | Revisar els criteris d'inclusió (fitxer 02) |