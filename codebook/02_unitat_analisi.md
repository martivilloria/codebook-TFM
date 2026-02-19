# 02. Unitat d'Anàlisi

## Definició
La **unitat d'anàlisi** és el parell format per:
1. **L'estímul** — una intervenció de la dreta radical (AC o Vox) sobre seguretat i/o immigració
2. **La rèplica** — la resposta d'un o més partits del bloc democràtic a aquest estímul

Cada unitat d'anàlisi (UA) es registra com un parell estímul-resposta.

---

## Criteris d'inclusió
S'inclou una UA si:
- ✅ L'estímul prové d'AC o Vox
- ✅ El tema és seguretat i/o immigració
- ✅ Hi ha una rèplica explícita d'un partit del bloc democràtic
- ✅ La intervenció és en un ple del Parlament de Catalunya

## Criteris d'exclusió
S'exclou una UA si:
- ❌ La intervenció és en comissió (no en ple)
- ❌ No hi ha rèplica identificable
- ❌ El tema no és seguretat ni immigració
- ❌ La intervenció és purament procedimental

---

## Estructura de cada UA

```
UNITAT D'ANÀLISI [número]
│
├── ESTÍMUL
│   ├── Sessió: [15pXXX]
│   ├── Pàgina: [número]
│   ├── Actor: [AC / Vox]
│   ├── Diputat/da: [nom]
│   ├── Fragment literal: "[cita textual]"
│   ├── Categoria DR: [DR-01 a DR-05]
│   └── Notes analítiques: [observacions]
│
└── RÈPLICA
    ├── Actor: [PSC / ERC / Junts / CUP / Comuns]
    ├── Diputat/da: [nom]
    ├── Fragment literal: "[cita textual]"
    ├── Categoria BD: [BD-01 a BD-06]
    ├── Eficàcia estimada: [🔴 Baixa / 🟡 Mitjana / 🟢 Alta]
    └── Notes analítiques: [observacions]
```

---

## Exemple codificat

### UA-001

**ESTÍMUL**
- Sessió: 15p062
- Actor: Vox
- Diputat/da: Ignacio Garriga
- Fragment literal: *"hemos pasado de una delincuencia de baja intensidad a una zona de degradación criminal. La tolerancia con la delincuencia menor, con los okupas, con los manteros, con los ladrones del metro, ha dado paso a una delincuencia que sube peldaños"*
- Categoria DR: **DR-01** (Securitització)
- Notes: Ús d'escalada retòrica. Llista acumulativa per crear sensació de col·lapse.

**RÈPLICA**
- Actor: PSC
- Diputat/da: Núria Parlon
- Fragment literal: *"Vostè el que fa és utilitzar les dades per generar un clima social de por, d'enfrontament, de xenofòbia i dir que el Govern no fa res"*
- Categoria BD: **BD-02** (Criminalització del Missatger)
- Eficàcia estimada: 🔴 Baixa
- Notes: Ataca l'emissor però no desactiva el contingut no-en-qüestió (la pressuposició que hi ha inseguretat). Beaver & Stanley (2023): el frame queda intacte.

---

## Arbre de decisió per identificar una UA

```
Hi ha una intervenció d'AC o Vox?
        │
        ├── NO → No és UA
        │
        └── SÍ → El tema és seguretat i/o immigració?
                        │
                        ├── NO → No és UA
                        │
                        └── SÍ → Hi ha rèplica d'un partit democràtic?
                                        │
                                        ├── NO → No és UA (registrar com a "sense resposta")
                                        │
                                        └── SÍ → ✅ CODIFICAR COM A UA
```

---

## Fitxa de codificació (imprimible)

| Camp | Valor |
|------|-------|
| Número UA | |
| Sessió | |
| Pàgina | |
| Actor DR | AC / Vox |
| Diputat/da DR | |
| Fragment estímul | |
| Categoria DR | DR-01 / DR-02 / DR-03 / DR-04 / DR-05 |
| Actor BD | PSC / ERC / Junts / CUP / Comuns |
| Diputat/da BD | |
| Fragment rèplica | |
| Categoria BD | BD-01 / BD-02 / BD-03 / BD-04 / BD-05 / BD-06 |
| Eficàcia | 🔴 Baixa / 🟡 Mitjana / 🟢 Alta / 🔴 Contraproduent |
| Notes | |