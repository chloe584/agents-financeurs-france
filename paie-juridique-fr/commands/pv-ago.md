---
name: pv-ago
description: Génère un PV d'AGO d'approbation des comptes pour une SAS, SASU, SCI ou SARL française.
---

# /pv-ago

## Étapes

1. Demande inputs (forme, dénomination, capital, siège, RCS, clôture, AGO, associés, comptes, affectation résultat, conventions, mandats)
2. Génère PV docx avec en-tête, feuille présence, lecture rapports, 7-10 résolutions, signatures
3. Génère rapport de gestion du Président
4. Génère rapport spécial conventions réglementées si applicable
5. Liste les formalités post-AGO (dépôt greffe + registre des assemblées)

## Sortie

- PV.docx
- Rapport_de_gestion.docx
- Rapport_special_conventions.docx (si applicable)
- Checklist post-AGO en markdown
