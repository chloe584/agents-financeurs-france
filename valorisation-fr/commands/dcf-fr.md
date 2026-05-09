---
name: dcf-fr
description: Construit un modèle DCF avec WACC calibré France et table de football multi-méthodes.
---

# /dcf-fr

## Étapes

1. Demande inputs (CA, marge EBITDA, CAPEX, BFR, taux IS, dette nette)
2. Calcule WACC France (OAT 10 ans + MRP 6,5-7% + beta + size + CRP)
3. Projette FCF Firm sur 5-10 ans
4. Calcule valeur terminale (Gordon avec g=1,5% par défaut)
5. Actualise EV puis Equity Value
6. Construit table de sensibilité (WACC × g)
7. Compare avec multiples sectoriels FR
8. Produit xlsx avec graphiques + table de football
