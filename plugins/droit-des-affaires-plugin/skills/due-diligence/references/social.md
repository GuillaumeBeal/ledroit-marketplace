# Domaine Social / Droit du Travail — Référence Due Diligence

## Objectif

Analyser la conformité de la société cible au droit du travail et identifier les risques sociaux (contentieux, non-conformité, passifs latents) susceptibles d'impacter la valorisation ou de nécessiter des actions correctives.

## Checklist d'analyse

### 1. Effectifs et organisation

**ANALYSE/VÉRIFICATION** :
- Nombre de salariés (CDI, CDD, temps plein, temps partiel)
- Ancienneté moyenne, turn-over
- Organigramme / répartition par service et qualification
- Masse salariale totale (y compris charges)
- Recours aux prestataires externes, intérimaires, freelances
- Détachement / expatriation de salariés

**POINTS DE VIGILANCE** :
- Seuils sociaux : 11 salariés (CSE), 50 salariés (CSE renforcé, participation, bilan social, obligations renforcées)
- Prestataires réguliers → risque de requalification en contrat de travail (lien de subordination, intégration, exclusivité)
- Intérimaires → vérifier le respect des motifs et durées légales

**VÉRIFICATION LEGIFRANCE** :
- Seuils CSE : Art. L2311-2 Code du travail (LEGITEXT000006072050)
- Requalification : Art. L8221-6 Code du travail (présomption de non-salariat)
- Intérim : Art. L1251-1 et s. Code du travail

### 2. Convention collective applicable

**ANALYSE/VÉRIFICATION** :
- Convention collective applicable (IDCC) et son étendue
- Accords de branche étendus applicables
- Accords d'entreprise en vigueur
- Usages et engagements unilatéraux
- Vérifier l'adéquation de la CC avec l'activité réelle (code NAF/APE)

**CONVENTIONS COLLECTIVES FRÉQUENTES** :
| IDCC | Convention |
|------|-----------|
| 1486 | Syntec (bureaux d'études, ingénierie, conseil) |
| 1979 | HCR (hôtels, cafés, restaurants) |
| 3248 | Métallurgie (nouvelle CC 2024) |
| 2098 | Prestataires de services |
| 44 | Industries chimiques |
| 176 | Industrie pharmaceutique |
| 1518 | Animation |
| 2120 | Banque |

**POINTS DE VIGILANCE** :
- Mauvaise convention collective appliquée → redressement URSSAF, rappel de salaires
- Accords d'entreprise dérogatoires → vérifier la validité (signature, dépôt, publicité)
- Usages non dénoncés → maintien automatique

**VÉRIFICATION LEGIFRANCE** :
- Convention collective : `displayKaliContByIdccUsingPOST(id: "<IDCC>")`
- Navigation : `displayKaliSectionUsingPOST` puis `displayKaliArticleUsingPOST`
- Champ d'application : Art. L2261-2 Code du travail

### 3. Représentants du personnel / CSE

**ANALYSE/VÉRIFICATION** :
- Existence d'un CSE (Comité Social et Économique)
- Date des dernières élections professionnelles
- PV de carence le cas échéant
- Composition du CSE, attributions (< 50 ou ≥ 50 salariés)
- Consultation du CSE requise pour l'opération ?
- Délégués syndicaux, sections syndicales

**POINTS DE VIGILANCE** :
- ≥ 11 salariés → obligation de mettre en place un CSE (depuis ordonnances Macron 2017)
- ≥ 50 salariés → CSE avec attributions élargies (consultation obligatoire sur marche générale, restructurations)
- Pas de CSE malgré obligation → délit d'entrave, risque pénal
- Consultation requise pour l'opération → impact sur le calendrier (délais de consultation : 1 mois minimum, 2 mois si expertise)

**VÉRIFICATION LEGIFRANCE** :
- CSE : Art. L2311-1 à L2317-2 Code du travail
- Consultation restructuration : Art. L2312-8 et L2312-39 Code du travail
- Délais consultation : Art. R2312-6 Code du travail

### 4. Loi Hamon (information des salariés)

**ANALYSE/VÉRIFICATION** :
- Entreprise < 250 salariés → obligation d'information des salariés en cas de cession de plus de 50% du capital
- S'applique aux ventes de parts/actions (pas aux apports a priori)
- Délai de 2 mois pour que les salariés formulent une offre de rachat
- Possibilité de raccourcir le délai si renonciation écrite de tous les salariés

**POINTS DE VIGILANCE** :
- Non-respect de la loi Hamon → nullité de la cession (risque majeur)
- Timing : le signing ne peut intervenir avant l'expiration du délai de 2 mois (sauf renonciation)
- En l'absence de CSE, l'information est faite directement aux salariés

**EXEMPLE ANONYMISÉ** :
> Dans le cadre de l'opération sur [Cible], il était envisagé une cession de titres + un apport. L'information des salariés au titre de la loi Hamon devait être réalisée préalablement au signing pour la partie cession, avec obtention de la renonciation expresse de tous les salariés pour écourter le délai de 2 mois.

**VÉRIFICATION LEGIFRANCE** :
- Information salariés : Art. L23-10-1 et s. Code de commerce
- Sanctions : Art. L23-10-6 Code de commerce

### 5. Contrats de travail

**ANALYSE/VÉRIFICATION** :
- Modèles de contrats utilisés (CDI, CDD, contrats spéciaux)
- Clauses essentielles : durée du travail, rémunération, lieu de travail, qualification
- Clauses de non-concurrence (existence, périmètre, durée, contrepartie financière)
- Clauses de propriété intellectuelle (cession des droits, rémunération supplémentaire)
- Clauses de mobilité, d'exclusivité
- Contrats de dirigeants (cumul mandat social / contrat de travail)
- Salariés protégés (représentants du personnel, femmes enceintes, accidentés du travail)

**POINTS DE VIGILANCE** :
- Absence de clause de non-concurrence pour postes clés → risque de départ vers un concurrent
- Clause de non-concurrence sans contrepartie financière → nulle
- Absence de clause PI → les droits sur les créations des salariés restent chez le salarié (sauf logiciel : Art. L113-9 CPI)
- Durée du travail non précisée dans le contrat → risque de rappel d'heures supplémentaires
- Absence de suivi du temps de travail → présomption en faveur du salarié

**EXEMPLE ANONYMISÉ** :
> Aucun contrat de travail de [Cible] ne comportait de clause de non-concurrence. Recommandation : conclusion d'avenants individuels pour les postes clés. Par ailleurs, la durée du travail n'était pas expressément stipulée (renvoi générique à l'horaire collectif). Risque estimé de rappel d'heures supplémentaires sur 3 ans : environ 25.000€/salarié (charges comprises).

**VÉRIFICATION LEGIFRANCE** :
- CDI : Art. L1221-2 Code du travail
- CDD : Art. L1242-1 et s. Code du travail
- Non-concurrence : jurisprudence Cass. soc. 10 juill. 2002 (contrepartie obligatoire)
- Cession PI salarié : Art. L113-9 CPI (logiciels), Art. L611-7 CPI (inventions)

### 6. Durée du travail

**ANALYSE/VÉRIFICATION** :
- Durée collective applicable (35h, 37h, 39h, forfait jours)
- Conventions de forfait jours (cadres autonomes) → accord collectif + accord individuel
- Heures supplémentaires : contingent, taux de majoration, repos compensateur
- Outil de suivi du temps de travail
- Astreintes, travail de nuit, travail le dimanche

**POINTS DE VIGILANCE** :
- Forfait jours sans accord collectif valide → nullité, rappel d'heures supplémentaires considérable
- Absence de suivi de la durée du travail → en cas de contentieux, la charge de la preuve incombe à l'employeur
- Dépassement des durées maximales → sanctions pénales

**VÉRIFICATION LEGIFRANCE** :
- Durée légale : Art. L3121-27 Code du travail (35h)
- Forfait jours : Art. L3121-58 et s. Code du travail
- Heures supplémentaires : Art. L3121-28 et s. Code du travail

### 7. Épargne salariale

**ANALYSE/VÉRIFICATION** :
- Participation (obligatoire ≥ 50 salariés pendant 5 ans consécutifs → loi PACTE : 12 mois consécutifs ou non sur 3 exercices)
- Intéressement (facultatif, durée 1 à 5 ans depuis loi partage de la valeur 2023)
- PEE, PERCO/PERECO
- Abondement employeur
- Report d'assujettissement à la participation si accord d'intéressement appliqué sans discontinuité

**POINTS DE VIGILANCE** :
- Franchissement du seuil de 50 salariés → vérifier l'obligation de participation
- Accord d'intéressement expiré → assujettissement immédiat à la participation
- Absence de participation alors qu'obligatoire → rappel + intérêts

**EXEMPLE ANONYMISÉ** :
> [Cible] avait franchi le seuil de 50 salariés en 2018. Grâce à un accord d'intéressement conclu en 2016 pour 3 ans, l'obligation de participation était repoussée à 2021. La négociation d'un accord de participation était envisagée.

**VÉRIFICATION LEGIFRANCE** :
- Participation : Art. L3322-1 et s. Code du travail
- Intéressement : Art. L3311-1 et s. Code du travail
- Seuils PACTE : Art. L3322-2 Code du travail

### 8. Litiges prud'homaux et contentieux social

**ANALYSE/VÉRIFICATION** :
- Litiges en cours (nombre, nature, montant des demandes, stade procédural)
- Litiges menacés
- Historique des litiges (3-5 ans)
- Ruptures de contrats (licenciements, ruptures conventionnelles, démissions)
- Inspections du travail, mises en demeure, PV d'infraction
- URSSAF : contrôles, redressements

**POINTS DE VIGILANCE** :
- Volume de ruptures conventionnelles élevé → vérifier l'absence de PSE déguisé
- Contentieux sériel (même type de demande par plusieurs salariés) → risque systémique
- Contrôle URSSAF → vérifier les redressements et les points récurrents

**VÉRIFICATION LEGIFRANCE** :
- Barème Macron : Art. L1235-3 Code du travail (indemnités licenciement sans cause)
- Rupture conventionnelle : Art. L1237-11 et s. Code du travail
- Contrôle URSSAF : Art. L243-7 Code de la sécurité sociale (LEGITEXT000006073189)

### 9. Risques sociaux spécifiques à l'opération

**ANALYSE/VÉRIFICATION** :
- Changement de contrôle → impact sur les contrats de travail (aucun en principe : Art. L1224-1 si transfert d'entreprise)
- Obligation de consultation du CSE
- Information des salariés (loi Hamon)
- Clauses de golden parachute / indemnités de départ
- Engagement de non-licenciement / maintien d'emploi (promesses cédant)

**VÉRIFICATION LEGIFRANCE** :
- Transfert d'entreprise : Art. L1224-1 Code du travail
- Golden parachute : Art. L225-42-1 Code de commerce (SA)
