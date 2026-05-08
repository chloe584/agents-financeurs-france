---
name: plan-tresorerie-13s
description: Plan de trésorerie prévisionnel 13 semaines (rolling) pour société française. Déclencher dès qu'on parle de plan trésorerie, prévisionnel cash, 13 semaines, BFR, DSO, DPO, FCF, runway, burn rate, encaissements, décaissements, ou pilotage. Couvre la construction du modèle, les KPI (BFR, DSO, DPO, FCF, runway), les scénarios (base, prudent, stress) et les alertes.
---

# Plan de trésorerie 13 semaines (FR)

## Structure

Tableau S+0 à S+12 par catégorie.

### Encaissements
- Clients par contrat
- Subventions
- Remboursement CIR/CIPP/CIJV
- Apports C/C

### Décaissements
- Salaires nets
- URSSAF (5 ou 15 du mois)
- TVA
- IS (acomptes 15/03, 15/06, 15/09, 15/12)
- Loyers
- Fournisseurs
- Emprunts

## KPI

| KPI | Formule |
| --- | ------- |
| BFR | Stocks + Créances - Dettes fournisseurs - Dettes fiscales |
| DSO | Créances clients TTC × 365 / CA TTC |
| DPO | Dettes fournisseurs TTC × 365 / Achats TTC |
| FCF | EBITDA - ΔBFR - CAPEX - IS payé |
| Runway | Trésorerie nette / Burn rate mensuel |

## Particularités FR

- Charges sociales : 5 (>=50 sal) ou 15 (<50)
- TVA : ~24 du mois M+1
- IS : 15/03, 15/06, 15/09, 15/12 + solde 15/05 N+1
- Délais B2B : 60j fin de mois (LME 2008, art. L.441-10 C.com)

## Sources

- Art. L.441-10 C. com
- Art. L.3242-1 C. trav
- Art. 1668 CGI
