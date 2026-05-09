---
name: dcf-wacc-france
description: Modèle DCF calibré pour la France avec WACC France et prime pays. Déclencher dès qu'on parle de DCF, valorisation par actualisation des flux, WACC, CMPC, taux sans risque, OAT 10 ans, prime de risque marché France, beta sectoriel, prime de taille, valeur terminale, actualisation, free cash flow, FCF Firm, FCF Equity. Couvre la construction d'un DCF (projection 5-10 ans, FCF, WACC, valeur terminale Gordon ou multiple de sortie), les sources françaises (OAT 10 ans BdF, primes EY/PwC/Deloitte/KPMG).
---

# DCF France

## WACC France

WACC = Ke × (E/V) + Kd × (1-t) × (D/V)

## Coût des fonds propres (CAPM)

Ke = Rf + β × MRP + Size Premium + Country Risk Premium France

| Composant | Source FR | Indicatif 2026 |
| --------- | --------- | -------------- |
| Rf (OAT 10 ans) | Banque de France | ~3,2% |
| MRP | EY/PwC/Deloitte/KPMG | 6,5-7,0% |
| β | Damodaran Europe | Selon secteur |
| Size Premium | Duff & Phelps Kroll | 0-5% |
| CRP France | Damodaran | ~0,7% |

## Construction DCF

### Période explicite (5-10 ans)
FCF Firm = EBIT × (1-t) + Amortissements - CAPEX - ΔBFR

### Valeur terminale
- Gordon : VT = FCF(n+1) / (WACC - g), g = 1-2%
- Multiple de sortie : VT = EBITDA(n) × multiple sectoriel

### Equity Value
Equity Value = EV - Dette nette + Trésorerie + Actifs hors expl - Passifs hors expl

## Spécificités FR

- Taux IS : 25% (taux normal) ou 25,825% avec contribution sociale 3,3%
- CIR/CII/CIPP : réduisent le taux d'impôt effectif
- CVAE/CFE : modeliser dans EBIT

## Sources

- Banque de France (OAT 10 ans)
- Damodaran Europe (primes, betas)
- Études WACC EY, PwC, Deloitte, KPMG
- Pappers, Infogreffe (comparables FR)
