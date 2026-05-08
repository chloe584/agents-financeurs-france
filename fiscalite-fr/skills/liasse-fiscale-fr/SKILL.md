---
name: liasse-fiscale-fr
description: Production et relecture de la liasse fiscale française (2065, 2050-2059, 2058-A, 2058-B, 2058-C). Déclencher dès qu'on parle de liasse fiscale, 2065, 2050, 2058, 2059, TDFC, télédéclaration, déclaration IS, réintégrations, déductions, ou bordereau. Couvre les contrôles inter-formulaires, la cohérence avec la balance, les délais (15 mai N+1), les bugs millesime Pennylane, et les mentions obligatoires.
---

# Liasse fiscale française

## Composition

| Formulaire | Contenu |
| ---------- | ------- |
| 2065 | Déclaration de résultat IS |
| 2050 | Bilan actif |
| 2051 | Bilan passif |
| 2052 | Compte de résultat (1) |
| 2053 | Compte de résultat (2) |
| 2054 | Immobilisations |
| 2055 | Amortissements |
| 2056 | Provisions |
| 2057 | Échéances créances/dettes |
| 2058-A | Résultat fiscal |
| 2058-B | Déficits, CP, provisions ND |
| 2058-C | Affectation résultat |

## Contrôles inter-formulaires

- Bilan équilibré (2050 = 2051)
- Résultat 2052/2053 = 2058-A WA = 2065 ligne 4
- Capitaux propres 2051 vs 2058-C
- Immobilisations 2054 vs 2050
- Amortissements 2055 vs 2052

## Réintégrations courantes

| Ligne | Nature | Référence |
| ----- | ------ | --------- |
| WB | Rémunérations excessives | CGI 39-1-1° |
| WC | Amortiss. véhicules | CGI 39-4 |
| WI | TVTS | CGI 1010 |
| WJ | Provisions ND | CGI 39-1-5° |
| WK | Charges fi (limite 75%/3M€) | CGI 212 bis |
| WV | CIR/CII | CGI 244 quater B/H |

## Délais

- Clôture 31/12 → dépôt au plus tard 2e jour ouvré suivant 1er mai N+1 (art. 175 CGI)
- Sanction retard : majoration 10% (art. 1728 CGI)

## Sources

- Article 53 A CGI
- BOI-IS-DECLA-10
- Article 175 CGI
