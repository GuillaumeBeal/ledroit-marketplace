# Domaine Protection des Données / RGPD — Référence Due Diligence

## Objectif

Évaluer le niveau de conformité de la société cible à la réglementation sur la protection des données personnelles (RGPD et loi Informatique et Libertés), identifier les risques de sanctions et les actions correctives nécessaires.

## Cadre juridique

- **RGPD** : Règlement (UE) 2016/679 du 27 avril 2016
- **Loi Informatique et Libertés** : Loi n°78-17 du 6 janvier 1978 modifiée
- **ePrivacy** : Directive 2002/58/CE (cookies, communications électroniques)

**VÉRIFICATION LEGIFRANCE** :
- Loi Informatique et Libertés : `searchUsingPOST` fond LODA_DATE, typeChamp TITLE, valeur "informatique fichiers libertés"
- Décisions CNIL : `searchUsingPOST` fond CNIL, mots-clés pertinents
- Articles RGPD directement applicables (pas dans Légifrance mais dans le JOUE)

## Checklist d'analyse

### 1. Gouvernance données personnelles

**ANALYSE/VÉRIFICATION** :
- Désignation d'un DPO (Délégué à la Protection des Données) → obligatoire dans certains cas (Art. 37 RGPD)
- DPO interne ou externe ? Déclaration CNIL du DPO effectuée ?
- Politique de protection des données personnelles
- Audit de conformité RGPD réalisé ? Date ? Résultats ? Suivi des recommandations ?
- Sensibilisation/formation des collaborateurs
- Budget dédié à la conformité RGPD

**POINTS DE VIGILANCE** :
- Obligation de DPO : autorité/organisme public, suivi régulier et systématique de personnes à grande échelle, traitement à grande échelle de données sensibles
- Absence de DPO alors qu'obligatoire → non-conformité directe
- Audit réalisé mais recommandations non suivies → niveau de maturité insuffisant

### 2. Registre des activités de traitement

**ANALYSE/VÉRIFICATION** :
- Registre tenu conformément à l'Art. 30 RGPD
- Exhaustivité : tous les traitements recensés ?
- Pour chaque traitement :
  - Finalités
  - Catégories de personnes concernées
  - Catégories de données collectées
  - Destinataires
  - Durées de conservation
  - Mesures de sécurité
  - Transferts hors UE
- Base légale pour chaque traitement (consentement, contrat, intérêt légitime, obligation légale)

**POINTS DE VIGILANCE** :
- Registre incomplet ou absent → non-conformité majeure
- Traitements sans base légale identifiée → risque de sanction
- Durées de conservation non définies → risque de conservation excessive

**EXEMPLE ANONYMISÉ** :
> Le registre de [Cible] contenait une seule fiche partiellement complétée (gestion du personnel). L'ensemble des autres traitements (clients, prospects, fournisseurs, site web) n'était pas documenté. Recommandation : régulariser le registre en priorité.

### 3. Information des personnes concernées

**ANALYSE/VÉRIFICATION** :
- Politique de confidentialité du site web (Art. 13 RGPD)
  - Identité et coordonnées du responsable de traitement
  - Coordonnées du DPO
  - Finalités et bases juridiques de chaque traitement
  - Destinataires et transferts hors UE
  - Durées de conservation
  - Droits des personnes (accès, rectification, effacement, portabilité, opposition, limitation)
  - Droit d'introduire une réclamation auprès de la CNIL
  - Droit de définir des directives sur le sort des données après décès
- CGV / mentions RGPD
- Contrats de travail / livret d'accueil
- Formulaires de collecte de données (mentions d'information)

**POINTS DE VIGILANCE** :
- Politique de confidentialité incomplète → non-conformité systématique
- Absence d'information dans les contrats de travail → risque salarié
- Formulaires de collecte sans mention d'information → collecte déloyale

**EXEMPLE ANONYMISÉ** :
> La politique de confidentialité du site web de [Cible] était globalement satisfaisante mais perfectible : bases juridiques non précisées par finalité, droits de portabilité et d'opposition non mentionnés, droit post-mortem absent.

### 4. Contrats avec les sous-traitants (Art. 28 RGPD)

**ANALYSE/VÉRIFICATION** :
- Inventaire des sous-traitants traitant des données personnelles pour le compte de la cible
- DPA (Data Processing Agreement) signé avec chaque sous-traitant ?
- Clauses obligatoires Art. 28 RGPD :
  - Objet et durée du traitement
  - Nature et finalité du traitement
  - Type de données et catégories de personnes
  - Obligations et droits du responsable de traitement
  - Instruction documentée
  - Confidentialité
  - Mesures de sécurité
  - Sous-traitance ultérieure (autorisation)
  - Assistance pour les droits des personnes
  - Suppression/restitution des données en fin de contrat
  - Audits

**POINTS DE VIGILANCE** :
- Absence de DPA → non-conformité directe
- Sous-traitant hors UE sans garanties appropriées → transfert illicite
- Sous-traitant utilisant les données pour son propre compte → violation Art. 28

### 5. Transferts de données hors UE

**ANALYSE/VÉRIFICATION** :
- Transferts identifiés (sous-traitants US, filiales hors UE, cloud, SaaS)
- Garanties appropriées mises en place :
  - Décision d'adéquation de la Commission (pays reconnus)
  - Clauses Contractuelles Types (CCT/SCC) de la Commission européenne (version 2021)
  - Règles d'entreprise contraignantes (BCR)
  - Dérogations Art. 49 RGPD (consentement explicite, exécution contrat)
- TIA (Transfer Impact Assessment) réalisée pour les transferts vers les USA post-Schrems II (et pré-DPF/post-DPF)

**POINTS DE VIGILANCE** :
- EU-US Data Privacy Framework (DPF) depuis juillet 2023 → vérifier l'inscription du destinataire
- Transferts sans garantie → sanction CNIL
- Services cloud US (AWS, Google, Microsoft) → vérifier les CCT et les mesures supplémentaires

### 6. Sécurité des données

**ANALYSE/VÉRIFICATION** :
- Politique de sécurité des systèmes d'information (PSSI)
- Mesures techniques (chiffrement, pseudonymisation, contrôle d'accès, pare-feu, anti-malware)
- Mesures organisationnelles (sensibilisation, gestion des habilitations, procédure d'incident)
- Analyse d'impact relative à la protection des données (AIPD/DPIA) pour les traitements à risque
- Tests d'intrusion / audits de sécurité réalisés
- Historique des violations de données (data breaches)

**POINTS DE VIGILANCE** :
- Faille de sécurité non notifiée à la CNIL dans les 72h (Art. 33 RGPD) → sanction
- Faille de sécurité non notifiée aux personnes concernées si risque élevé (Art. 34 RGPD) → sanction
- Absence de PSSI → faiblesse structurelle
- DPIA non réalisée pour les traitements à grande échelle de données sensibles → non-conformité

**EXEMPLE ANONYMISÉ** :
> [Cible] avait fait l'objet d'une faille de sécurité susceptible d'avoir entraîné une violation de données personnelles. La faille n'avait été notifiée ni à la CNIL (Art. 33), ni aux personnes concernées (Art. 34). Risque : sanctions potentiellement importantes (jusqu'à 20 M€ ou 4% du CA mondial annuel).

### 7. Cookies et traceurs

**ANALYSE/VÉRIFICATION** :
- Bandeau cookies conforme (consentement préalable, refus aussi simple que l'acceptation)
- Politique cookies détaillée (finalités, durées, tiers)
- CMP (Consent Management Platform) utilisée
- Cookies déposés sans consentement (cookies analytics, marketing)

**VÉRIFICATION LEGIFRANCE** :
- Cookies : Art. 82 Loi Informatique et Libertés (transposition ePrivacy)
- Lignes directrices CNIL cookies : `searchUsingPOST` fond CNIL, mots-clés "cookies traceurs"

### 8. Contrôles CNIL et sanctions

**ANALYSE/VÉRIFICATION** :
- Contrôles CNIL passés ou en cours
- Correspondances avec la CNIL
- Plaintes de personnes concernées
- Sanctions prononcées

**BARÈME INDICATIF DES SANCTIONS CNIL** :
- Jusqu'à 10 M€ ou 2% du CA mondial : violations relatives aux obligations du responsable de traitement (registre, sécurité, DPIA, DPO)
- Jusqu'à 20 M€ ou 4% du CA mondial : violations relatives aux droits des personnes, transferts illicites, principes fondamentaux

## Recommandations types

| Priorité | Action |
|----------|--------|
| Haute | Compléter le registre des activités de traitement |
| Haute | Mettre à jour la politique de confidentialité |
| Haute | Signer des DPA avec tous les sous-traitants |
| Haute | Notifier les violations de données non notifiées |
| Moyenne | Mettre en conformité les contrats (clients, salariés, fournisseurs) |
| Moyenne | Mettre en place des CCT pour les transferts hors UE |
| Moyenne | Réaliser les AIPD nécessaires |
| Basse | Former les collaborateurs |
| Basse | Mettre en place une PSSI formalisée |
