---
name: rapprochement-fec
description: Lance un rapprochement bancaire complet entre un FEC (export Pennylane) et un relevé bancaire (PDF Revolut, CSV CIC).
---

# /rapprochement-fec

Workflow guidé pour rapprocher un FEC avec un relevé bancaire selon le PCG.

## Étapes

1. Demande FEC (.txt) et relevé bancaire (.pdf, .csv, .xlsx)
2. Valide le format FEC (18 colonnes, tabulation)
3. Compare soldes ouverture/clôture
4. Match ligne par ligne
5. Liste les écarts par catégorie
6. Propose les écritures de régularisation PCG
7. Génère un rapport markdown + xlsx récapitulatif
