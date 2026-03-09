# Templates de Rapports — Due Diligence

## Objectif

Ce fichier fournit les structures types pour chaque livrable de la due diligence juridique. Utiliser ces templates comme base et les adapter au contexte de chaque mission.

---

## I. Rapport Red Flag (livrable principal en DD limitée)

### Structure

```
PAGE DE GARDE
- Nom du projet (code project)
- "Due Diligence Juridique — Rapport Red Flag"
- "CONFIDENTIEL — Réservé au destinataire"
- Date
- Nom du cabinet / de l'équipe

1. INTRODUCTION
   1.1 Contexte de l'opération
       - Présentation succincte de la cible (forme, activité, effectif, CA)
       - Nature de l'opération envisagée (cession de titres, apport, fusion)
       - Identification de l'acquéreur
   1.2 Périmètre de la revue
       - Domaines couverts (corporate, social, fiscal, IP, contrats, etc.)
       - Domaines exclus et raisons
       - Période de revue
   1.3 Méthodologie
       - Documents examinés (avec référence à la data room)
       - Entretiens réalisés (management, CAC, conseil)
       - Limitations (documents non reçus, langue, accès restreint)
   1.4 Disclaimer
       - "Le présent rapport a été préparé sur la base des documents
         et informations communiqués. Il ne constitue pas un audit
         exhaustif et ne saurait se substituer à une due diligence
         complète. Les conclusions sont formulées sous réserve de
         l'exhaustivité et de l'exactitude des informations reçues."

2. DÉFINITIONS
   - Cible : [Société cible]
   - Cédant : [Cédant]
   - Acquéreur : [Acquéreur]
   - Opération : [Description]
   - Date de Référence : [Date]
   - VDR : Virtual Data Room

3. SYNTHÈSE EXECUTIVE
   3.1 Principaux constats
       - Bullet points des 5-10 items les plus significatifs
   3.2 Recommandations prioritaires
       - Actions Signing (conditions préalables)
       - Actions Closing (à réaliser entre signing et closing)
       - Actions Post-Closing (à réaliser après closing)
   3.3 Évaluation globale du risque juridique

4. FICHE SOCIÉTÉ
   - Dénomination sociale
   - Forme juridique
   - Capital social
   - Siège social
   - RCS
   - SIRET / Code NAF
   - Date de création
   - Objet social
   - Exercice social
   - Dirigeants
   - Actionnariat
   - CAC
   - Convention collective (IDCC)
   - Effectif

5. TABLEAU DES RISQUES IDENTIFIÉS

   | N° | Domaine | Description du risque | Niveau | Impact estimé | Recommandation | Timing |
   |----|---------|----------------------|--------|---------------|----------------|--------|
   | 1 | Corporate | ... | Élevé | ... | ... | Signing |
   | 2 | Social | ... | Moyen | ... | ... | Closing |
   | ... | ... | ... | ... | ... | ... | ... |

   Niveaux de risque :
   - Élevé : Impact financier significatif ou risque de blocage de l'opération
   - Moyen : Impact financier modéré ou non-conformité à régulariser
   - Faible : Point d'attention, bonne pratique à mettre en place
   - Pour information : Constat sans risque immédiat

6. ANALYSE DÉTAILLÉE PAR DOMAINE

   6.1 CORPORATE
       [Analyse structurée selon references/corporate.md]
       Items numérotés : C.1, C.2, C.3...

   6.2 CONTRATS COMMERCIAUX
       [Analyse structurée selon references/contrats.md]
       Items numérotés : COM.1, COM.2...

   6.3 PROPRIÉTÉ INTELLECTUELLE
       [Analyse structurée selon references/ip.md]
       Items numérotés : PI.1, PI.2...

   6.4 FINANCEMENT
       [Analyse structurée selon references/financement.md]
       Items numérotés : FIN.1, FIN.2...

   6.5 SOCIAL
       [Analyse structurée selon references/social.md]
       Items numérotés : SOC.1, SOC.2...

   6.6 FISCAL
       [Analyse structurée selon references/fiscal.md]
       Items numérotés : FISC.1, FISC.2...

   6.7 IMMOBILIER / RÉGLEMENTAIRE / ASSURANCES
       [Analyse structurée selon references/reglementaire.md]
       Items numérotés : REG.1, REG.2...

   6.8 PROTECTION DES DONNÉES (RGPD)
       [Analyse structurée selon references/rgpd.md]
       Items numérotés : RGPD.1, RGPD.2...

7. ANNEXES
   Annexe 1 : Organigramme juridique
   Annexe 2 : Table de capitalisation
   Annexe 3 : Liste des documents examinés
   Annexe 4 : Liste des documents non reçus
```

### Format de chaque item de risque (dans l'analyse détaillée)

```
[N°] [Titre court] — [Niveau de risque]

Constat :
[Description factuelle et précise du constat, avec référence aux documents
examinés et aux dispositions légales applicables]

Risque :
[Description du risque juridique et de son impact potentiel,
avec quantification si possible]

Recommandation :
[Action corrective recommandée, avec timing (Signing/Closing/Post-Closing)]

Référence légale :
[Articles de loi, jurisprudence, doctrine applicable]
```

### Exemple d'item anonymisé

```
C.3 Conventions réglementées non approuvées — Risque Moyen

Constat :
Deux conventions réglementées entre [Cible] et [SCI du Dirigeant]
n'ont pas fait l'objet d'une approbation en assemblée générale
conformément à l'article L223-19 du Code de commerce.
Il s'agit de : (i) un contrat de bail commercial (loyer annuel :
XXX €) et (ii) une convention de mise à disposition de matériel.

Risque :
Les conventions non approuvées ne sont pas nulles mais leurs
conséquences préjudiciables peuvent être mises à la charge du
gérant (Art. L223-19 al. 4 C. com.). Risque de remise en cause
par les nouveaux associés post-acquisition.

Recommandation :
Procéder à la ratification des conventions réglementées par
l'assemblée générale des associés préalablement au Closing.
Inclure la ratification dans les conditions préalables (CP)
du SPA.

Référence légale :
Art. L223-19 et L223-20 Code de commerce
```

---

## II. Fiche Société

### Structure

```
FICHE SOCIÉTÉ — [Dénomination sociale]
Date : [Date]

IDENTITÉ
- Dénomination sociale :
- Nom commercial :
- Forme juridique :
- Capital social : [montant] € divisé en [nombre] parts/actions de [nominal] €
- Siège social :
- RCS : [ville] [numéro]
- SIRET :
- Code NAF/APE :
- N° TVA intracommunautaire :
- Date d'immatriculation :
- Durée de la société : [99 ans à compter du...]
- Exercice social : du [date] au [date]

OBJET SOCIAL
[Reproduction de l'objet social statutaire]

ACTIONNARIAT
| Associé/Actionnaire | Nombre de titres | % capital | % droits de vote |
|---------------------|------------------|-----------|------------------|
| [Nom] | [X] | [X]% | [X]% |
| ... | ... | ... | ... |
| TOTAL | [X] | 100% | 100% |

GOUVERNANCE
- Président / Gérant : [Nom], nommé le [date], pour une durée de [X]
- Directeur Général : [Nom] (le cas échéant)
- Conseil d'administration / Conseil de surveillance : [composition]

COMMISSAIRE AUX COMPTES
- Titulaire : [Cabinet], nommé le [date] pour [X] exercices
- Suppléant : [Cabinet]

CONVENTION COLLECTIVE
- IDCC : [numéro]
- Intitulé : [nom de la convention]

EFFECTIF
- CDI : [X] | CDD : [X] | Total : [X]
- Cadres : [X] | Non-cadres : [X]

CHIFFRES CLÉS (3 derniers exercices)
| | N-2 | N-1 | N |
|---|-----|-----|---|
| CA HT | | | |
| Résultat d'exploitation | | | |
| Résultat net | | | |
| Capitaux propres | | | |
| Effectif moyen | | | |

FILIALES ET PARTICIPATIONS
| Société | % détenu | Pays | Activité |
|---------|----------|------|----------|
| ... | ... | ... | ... |

ANNEXE 1 : Organigramme juridique
ANNEXE 2 : Table de capitalisation détaillée
ANNEXE 3 : Historique des modifications statutaires
```

---

## III. Synthèse Executive (Executive Summary)

### Structure (document autonome de 2-3 pages)

```
SYNTHÈSE EXECUTIVE — DUE DILIGENCE JURIDIQUE
Projet [Code Projet]
[Date]
CONFIDENTIEL

1. PRÉSENTATION DE L'OPÉRATION
   [2-3 phrases : cible, acquéreur, type d'opération, contexte]

2. PÉRIMÈTRE DE LA REVUE
   [Domaines couverts, période, limitations]

3. PRINCIPAUX CONSTATS

   Risques Élevés :
   - [Résumé item 1] → [Recommandation courte]
   - [Résumé item 2] → [Recommandation courte]

   Risques Moyens :
   - [Résumé item 3] → [Recommandation courte]
   - [Résumé item 4] → [Recommandation courte]

   Points d'attention :
   - [Résumé item 5]
   - [Résumé item 6]

4. RECOMMANDATIONS CLÉS

   Avant Signing :
   - [Action 1]
   - [Action 2]

   Entre Signing et Closing :
   - [Action 3]
   - [Action 4]

   Post-Closing :
   - [Action 5]
   - [Action 6]

5. ÉVALUATION GLOBALE
   [Paragraphe de synthèse : la cible présente un niveau de risque
   juridique [faible/modéré/significatif]. Les principaux points
   d'attention portent sur [domaines]. Sous réserve de la mise en
   œuvre des recommandations formulées, l'opération peut être
   réalisée dans des conditions satisfaisantes.]
```

---

## IV. Document de Questions-Réponses (Q&A)

### Structure

```
Q&A — DUE DILIGENCE JURIDIQUE
Projet [Code Projet]

| N° | Date | Domaine | Question | Destinataire | Réponse | Date réponse | Statut |
|----|------|---------|----------|--------------|---------|--------------|--------|
| 1 | JJ/MM | Corporate | ... | Management | ... | JJ/MM | Clos |
| 2 | JJ/MM | Social | ... | DRH | ... | | Ouvert |
| ... | ... | ... | ... | ... | ... | ... | ... |

Statuts : Ouvert | En cours | Clos | Escaladé
```

---

## V. Recommandations SPA (Share Purchase Agreement)

### Items types à inclure dans le SPA

```
DÉCLARATIONS ET GARANTIES (Representations & Warranties)
- Exactitude des informations communiquées
- Exhaustivité des litiges déclarés
- Conformité réglementaire
- Titularité des actifs PI
- Conformité RGPD
- Absence de passif non déclaré
- Validité des contrats significatifs

CONDITIONS PRÉALABLES (Conditions Precedent)
- [Issues des constats Signing du rapport]
- Obtention des waivers de changement de contrôle
- Ratification des conventions réglementées
- Information des salariés (loi Hamon)
- Consultation du CSE
- Waivers bancaires (changement de contrôle emprunts)
- Autorisations réglementaires

INDEMNISATION SPÉCIFIQUE
- Risques identifiés non provisionnés
- Litiges en cours (quantum estimé)
- Contrôles fiscaux/URSSAF (redressements potentiels)
- Régularisation PI

GARANTIE DE PASSIF
- Durée recommandée : [X] mois/années
- Plafond : [X]% du prix ou montant fixe
- Franchise / seuil de déclenchement
- Mécanisme de notification
- Séquestre ou garantie bancaire
```

---

## Conventions de nommage des livrables

| Livrable | Nom de fichier |
|----------|---------------|
| Rapport Red Flag | `[Projet] - DD Report - [Date].docx` |
| Fiche Société | `[Projet] - Fiche Société.docx` |
| Synthèse Executive | `[Projet] - Executive Summary - [Date].docx` |
| Liste de Documents | `[Projet] - Document Request List.xlsx` |
| Q&A | `[Projet] - Q&A Log.xlsx` |
| Recommandations SPA | `[Projet] - SPA Recommendations - [Date].docx` |

## Niveaux de risque — Définitions

| Niveau | Couleur | Définition |
|--------|---------|------------|
| Élevé | 🔴 | Impact financier significatif (>5% du prix), risque de blocage de l'opération, ou non-conformité grave exposant à des sanctions majeures |
| Moyen | 🟠 | Impact financier modéré (1-5% du prix), non-conformité à régulariser, ou risque de contentieux probable |
| Faible | 🟡 | Impact financier limité (<1% du prix), point d'attention ou bonne pratique à mettre en place |
| Pour information | 🔵 | Constat sans risque immédiat, élément à surveiller |

## Timing des recommandations — Définitions

| Timing | Définition |
|--------|------------|
| Signing | Condition préalable à la signature du SPA (doit être réalisé avant) |
| Closing | À réaliser entre le signing et le closing (condition de réalisation) |
| Post-Closing | À réaliser après le closing (engagement de l'acquéreur ou du cédant) |
| Ongoing | Action continue / surveillance permanente |
