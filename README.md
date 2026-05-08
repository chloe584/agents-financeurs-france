# Agents Financeurs France

Marketplace de plugins Claude Code / Cowork **adaptés au contexte fiscal et comptable français** : PCG, CGI, BOFiP, ANC, Code de commerce, Code du travail.

Inspiré du marketplace officiel [`anthropics/financial-services-plugins`](https://github.com/anthropics/financial-services-plugins) (DCF, comps, LBO, GL recon en US-GAAP), ce marketplace fournit l'équivalent **France PCG** pour les sociétés françaises (SAS, SASU, SCI, SARL).

## Pourquoi un marketplace France

Les plugins finance d'Anthropic sont calibrés US-GAAP / SEC / 10-K. Pour une société française, il faut :

- Plan Comptable Général (classes 1 à 7) au lieu du Chart of Accounts US
- Liasse fiscale (2065, 2050-2059, 2058-A) au lieu du 10-K
- FEC normé (art. A.47 A-1 LPF, 18 colonnes) au lieu du General Ledger US
- Annexes ANC 2022-06 au lieu de SEC disclosures
- DSN au lieu de Form W-2
- WACC calibré OAT 10 ans + prime pays France (~5,5 %) au lieu du Treasury 10Y

Ce marketplace fournit cinq plugins qui apportent ce contexte directement à Claude.

## Plugins inclus

| Plugin | Domaine | Skills clés |
| ------ | ------- | ----------- |
| **comptabilite-pcg** | Comptabilité PCG | FEC, écritures de clôture (CCA/PCA/FNP/ICNE), annexes ANC 2022-06, rapprochement bancaire |
| **fiscalite-fr** | Fiscalité FR | Liasse 2065/2050-2059/2058-A, IS, TVA, BOFiP, TDFC |
| **tresorerie-fr** | Trésorerie | Plan 13 semaines, intragroupe (4511), convention trésorerie L.511-7 CMF, FX |
| **valorisation-fr** | Valorisation | DCF avec WACC France, multiples sectoriels FR, ANR/ANCC |
| **paie-juridique-fr** | Paie & juridique | DSN, URSSAF, Syntec/Audiovisuel, PV AGO/AGE, conventions réglementées |

## Installation

### Claude Code

```bash
claude plugin marketplace add chloe584/agents-financeurs-france
claude plugin install comptabilite-pcg@agents-financeurs-france
claude plugin install fiscalite-fr@agents-financeurs-france
claude plugin install tresorerie-fr@agents-financeurs-france
claude plugin install valorisation-fr@agents-financeurs-france
claude plugin install paie-juridique-fr@agents-financeurs-france
```

### Cowork

Ouvrir Cowork → Settings → Plugins → Add marketplace → coller l'URL :
`https://github.com/chloe584/agents-financeurs-france`

## Sources normatives

- [Plan Comptable Général (PCG)](https://www.anc.gouv.fr/) — règlement ANC 2014-03
- [BOFiP](https://bofip.impots.gouv.fr/) — doctrine fiscale
- [Code Général des Impôts](https://www.legifrance.gouv.fr/codes/texte_lc/LEGITEXT000006069577/) (CGI)
- [Code de commerce](https://www.legifrance.gouv.fr/codes/texte_lc/LEGITEXT000005634379/)
- [Code du travail](https://www.legifrance.gouv.fr/codes/texte_lc/LEGITEXT000006072050/)

## Licence

Apache-2.0 (cohérent avec le marketplace officiel Anthropic).

## Avertissement

Ces plugins assistent les workflows comptables et fiscaux mais **ne se substituent pas à un expert-comptable, un commissaire aux comptes ou un avocat fiscaliste**. Toute écriture, déclaration ou décision juridique doit être validée par un professionnel qualifié.
