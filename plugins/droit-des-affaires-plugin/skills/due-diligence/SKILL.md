---
name: due-diligence
description: "Réalisation de due diligence juridique pour opérations M&A en droit français. Produit tous les livrables : rapport red flag, fiche société, synthèse executive, liste de documents, Q&A. Couvre 8 domaines (corporate, fiscal, social, IP, contrats, financement, réglementaire, RGPD). Intégré avec le MCP Légifrance pour vérification en temps réel des textes de loi, articles de code, conventions collectives et jurisprudence. Déclencher dès que l'utilisateur mentionne : due diligence, DD juridique, audit juridique, revue juridique, M&A, acquisition, cession de titres, LBO, vérification légale pré-acquisition, rapport red flag, fiche société cible."
---

# Skill Due Diligence Juridique

## Vue d'ensemble

Cette skill guide la réalisation d'une due diligence juridique complète dans le cadre d'opérations M&A (fusions-acquisitions) en droit français. Elle s'appuie sur une méthodologie éprouvée et sur l'intégration avec le MCP Légifrance pour la vérification des textes en temps réel.

## Fichiers de référence

Avant de commencer, lire les fichiers pertinents selon la mission :

| Fichier | Contenu |
|---------|---------|
| `references/corporate.md` | Forme sociale, actionnariat, gouvernance, statuts, pacte, conventions réglementées, groupe |
| `references/fiscal.md` | IS, TVA, CIR, CET, prix de transfert, contrôles, intégration fiscale |
| `references/social.md` | Effectifs, convention collective, CSE, loi Hamon, contrats de travail, durée du travail, épargne salariale |
| `references/financement.md` | Emprunts, changement de contrôle, sûretés, covenants, BPI, crédit-bail |
| `references/contrats.md` | Contrats clients/fournisseurs, distribution, sous-traitance, baux, CGV |
| `references/ip.md` | Brevets, marques, dessins, logiciels, noms de domaine, licences, litiges PI |
| `references/reglementaire.md` | Autorisations, environnement, compliance Sapin 2, immobilier, assurances |
| `references/rgpd.md` | Gouvernance RGPD, registre, DPA, transferts hors UE, sécurité, cookies, CNIL |
| `references/document-request-list.md` | Modèle de checklist de documents à demander (>100 items numérotés) |
| `references/report-templates.md` | Structures types : rapport red flag, fiche société, synthèse executive, Q&A, recommandations SPA |
| `references/legifrance-integration.md` | Table de correspondance articles / outils MCP Légifrance pour chaque domaine |

## Workflows

### Workflow 1 : DD complète (rapport red flag)

**Déclencheurs** : "faire une due diligence", "rapport red flag", "DD juridique sur [cible]"

**Étapes** :

1. **Collecte d'informations** — Demander à l'utilisateur :
   - Nom de la société cible, forme juridique, activité
   - Type d'opération (cession de titres, apport, fusion)
   - Périmètre souhaité (tous domaines ou domaines spécifiques)
   - Documents disponibles (data room, documents uploadés)
   - Délai et format de livrable souhaité

2. **Lecture des références** — Lire les fichiers de référence pour chaque domaine du périmètre. TOUJOURS commencer par `references/report-templates.md` pour la structure du livrable.

3. **Analyse par domaine** — Pour chaque domaine :
   - Suivre la checklist du fichier de référence correspondant
   - Identifier les risques (Élevé / Moyen / Faible / Pour information)
   - Vérifier les textes de loi via Légifrance (voir `references/legifrance-integration.md`)
   - Quantifier l'impact financier quand c'est possible
   - Formuler les recommandations avec timing (Signing / Closing / Post-Closing)

4. **Rédaction du rapport** — Suivre la structure de `references/report-templates.md` :
   - Page de garde avec disclaimer
   - Synthèse executive
   - Fiche société
   - Tableau des risques consolidé
   - Analyse détaillée par domaine (items numérotés)
   - Annexes

5. **Vérification** — Relire le rapport pour cohérence, vérifier les références légales, s'assurer que chaque risque a une recommandation.

6. **Livraison** — Générer le document final (DOCX de préférence).

### Workflow 2 : Fiche société

**Déclencheurs** : "fiche société", "résumé de la cible", "présentation de la société"

**Étapes** :
1. Lire `references/report-templates.md` section "Fiche Société"
2. Lire `references/corporate.md` pour les points de vérification
3. Collecter les informations (documents, Kbis, statuts)
4. Rédiger la fiche selon le template
5. Vérifier sur Légifrance si nécessaire (statuts, forme juridique)

### Workflow 3 : Liste de documents (Document Request List)

**Déclencheurs** : "liste de documents", "document request list", "checklist DD", "quels documents demander"

**Étapes** :
1. Lire `references/document-request-list.md`
2. Adapter la liste au contexte (secteur, taille, type d'opération)
3. Générer la liste personnalisée (XLSX ou DOCX avec tableau de suivi)

### Workflow 4 : Analyse d'un domaine spécifique

**Déclencheurs** : "analyser le volet social", "revue des contrats", "vérifier la PI", "audit RGPD"

**Étapes** :
1. Lire le fichier de référence du domaine concerné
2. Lire `references/legifrance-integration.md` pour les vérifications
3. Analyser les documents fournis selon la checklist
4. Identifier et grader les risques
5. Vérifier les textes via Légifrance
6. Rédiger l'analyse avec items numérotés

### Workflow 5 : Vérification légale ponctuelle

**Déclencheurs** : "vérifier l'article", "que dit la loi sur", "est-ce conforme à"

**Étapes** :
1. Lire `references/legifrance-integration.md` pour trouver l'article et l'outil MCP
2. Appeler l'outil Légifrance approprié
3. Analyser le texte dans le contexte de la DD
4. Formuler la conclusion

## Intégration Légifrance

Cette skill fonctionne en tandem avec le MCP Légifrance. Pour chaque vérification :

1. Consulter `references/legifrance-integration.md` pour l'article et le LEGITEXT
2. Utiliser `getArticleWithIdAndNumUsingPOST` pour les articles de code
3. Utiliser `searchUsingPOST` pour les lois par nom ou les recherches thématiques
4. Utiliser `displayKaliContByIdccUsingPOST` pour les conventions collectives
5. Utiliser `searchUsingPOST` fond JURI/CETAT pour la jurisprudence

**Règle** : Ne JAMAIS citer un article de loi sans avoir vérifié qu'il est toujours en vigueur via Légifrance. Les articles peuvent avoir été modifiés, renumérotés ou abrogés.

## Grille de risque

| Niveau | Critère | Action |
|--------|---------|--------|
| **Élevé** | Impact > 5% du prix, blocage possible, sanction majeure | Condition préalable au Signing ou garantie spécifique |
| **Moyen** | Impact 1-5% du prix, non-conformité à régulariser | Régularisation Closing ou indemnisation spécifique |
| **Faible** | Impact < 1% du prix, bonne pratique | Recommandation Post-Closing |
| **Info** | Pas de risque immédiat | Surveillance / mention dans le rapport |

## Conventions de rédaction

- **Objectivité** : Constats factuels, pas d'opinions non étayées
- **Précision** : Citer les articles de loi, les montants, les dates
- **Anonymisation** : Remplacer les noms réels par [Cible], [Cédant], [Acquéreur], [Sous-traitant A], etc.
- **Numérotation** : Chaque item de risque a un numéro unique (C.1, SOC.1, FISC.1, etc.)
- **Quantification** : Estimer l'impact financier chaque fois que possible
- **Recommandation** : Chaque risque identifié doit avoir une recommandation avec un timing

## Livrables possibles

1. **Rapport Red Flag** (DOCX) — Livrable principal, 20-60 pages
2. **Fiche Société** (DOCX) — 2-4 pages, annexes incluses
3. **Synthèse Executive** (DOCX) — 2-3 pages, pour le comité d'investissement
4. **Document Request List** (XLSX) — Checklist numérotée avec suivi
5. **Q&A Log** (XLSX) — Suivi des questions au management
6. **Recommandations SPA** (DOCX) — R&W, CP, indemnisation, garantie de passif
