---
name: pcg-fec-rapprochement
description: Rapprochement bancaire et analyse de FEC selon le PCG français. Déclencher dès qu'on parle de FEC, rapprochement, banque, écart, lettrage, compte 5121, balance, ou export Pennylane. Couvre la validation du format FEC (18 colonnes, séparateur tabulation, art. A.47 A-1 LPF), le matching avec relevés bancaires (Revolut, CIC, BNP, Stripe), la détection d'écarts (FX, virements en transit, frais bancaires, doublons), et les écritures de régularisation PCG (476/477/666/766).
---

# Rapprochement bancaire FEC × relevés

## Format FEC normé

- 18 colonnes (art. A.47 A-1 LPF)
- Séparateur tabulation
- Encodage ISO-8859-15 ou UTF-8

## Workflow

1. Validation soldes ouverture/clôture
2. Comptage transactions débit/crédit
3. Somme arithmétique de contrôle
4. Matching ligne par ligne (date, montant, libellé)
5. Identification des écarts (FX, transit, frais, doublons)

## Écritures de régularisation

| Cas | Débit | Crédit |
| --- | ----- | ------ |
| Perte de change | 666 | 5121 |
| Gain de change | 5121 | 766 |
| Virement en transit | 5811 | 5121 |
| Frais bancaires oubliés | 627 | 5121 |

## Sources

- Article A.47 A-1 LPF
- PCG — ANC 2014-03
- BOI-CF-COM-20-30
