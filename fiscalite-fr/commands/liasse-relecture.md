---
name: liasse-relecture
description: Relit une liasse fiscale française formulaire par formulaire et signale les anomalies, bugs millesime, et incohérences inter-formulaires.
---

# /liasse-relecture

## Étapes

1. Demande la liasse PDF + balance comptable
2. Vérifie complétude : 2065 + 2050-2059
3. Contrôle bilan équilibré
4. Vérifie résultat (2052/2053 = 2058-A WA = 2065 ligne 4)
5. Vérifie variation capitaux propres (2051 vs 2058-C)
6. Contrôle immobilisations (2054 vs 2050)
7. Vérifie amortissements (2055 vs 2052)
8. Contrôle réintégrations (WB, WC, WI, WJ, WK, WV)
9. Vérifie déductions (WO, WP, WT)
10. Détecte les bugs millesime Pennylane connus
11. Génère un rapport markdown des anomalies
