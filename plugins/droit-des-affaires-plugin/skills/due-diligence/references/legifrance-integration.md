# Intégration Légifrance — Référence Due Diligence

## Objectif

Ce fichier centralise toutes les références Légifrance utilisées dans la due diligence, avec les appels MCP correspondants. Il sert de guide pour vérifier en temps réel les textes de loi, articles de code, conventions collectives et jurisprudence pertinents.

## Codes LEGITEXT principaux

| Code | LEGITEXT ID | Abréviation |
|------|-------------|-------------|
| Code civil | LEGITEXT000006070721 | C. civ. |
| Code de commerce | LEGITEXT000005634379 | C. com. |
| Code du travail | LEGITEXT000006072050 | C. trav. |
| Code général des impôts | LEGITEXT000006069577 | CGI |
| Code de la propriété intellectuelle | LEGITEXT000006069414 | CPI |
| Code de l'environnement | LEGITEXT000006074220 | C. env. |
| Code monétaire et financier | LEGITEXT000006072026 | CMF |
| Code de la consommation | LEGITEXT000006069565 | C. conso. |
| Code de la sécurité sociale | LEGITEXT000006073189 | CSS |
| Livre des procédures fiscales | LEGITEXT000006069583 | LPF |

---

## Vérifications par domaine

### CORPORATE

| Sujet | Article(s) | Outil MCP |
|-------|-----------|-----------|
| SARL — gérance | L223-18 à L223-22 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L223-18")` |
| SARL — conventions réglementées | L223-19, L223-20 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L223-19")` |
| SARL — décisions collectives | L223-27 à L223-34 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L223-27")` |
| SAS — président et direction | L227-6 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L227-6")` |
| SAS — conventions réglementées | L227-10, L227-11 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L227-10")` |
| SAS — décisions collectives | L227-9 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L227-9")` |
| SA — conventions réglementées | L225-38 à L225-43 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L225-38")` |
| CAC — nomination obligatoire | L823-1 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L823-1")` |
| CAC — seuils Loi PACTE | Art. 20 Loi PACTE | `searchUsingPOST` fond LODA_DATE, TITLE "plan action croissance transformation" |
| Bénéficiaire effectif | L561-2-2 CMF | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006072026", num: "L561-2-2")` |

### FISCAL

| Sujet | Article(s) | Outil MCP |
|-------|-----------|-----------|
| IS — taux normal | 219 I CGI | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069577", num: "219")` |
| IS — taux réduit PME | 219 I b CGI | Même article, al. b |
| CIR | 244 quater B CGI | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069577", num: "244 quater B")` |
| CII | 244 quater B II bis CGI | Même article |
| TVA — régime | 256 et s. CGI | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069577", num: "256")` |
| CVAE | 1586 ter CGI | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069577", num: "1586 ter")` |
| CFE | 1447 CGI | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069577", num: "1447")` |
| Prix de transfert — documentation | L13 AA LPF | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069583", num: "L13 AA")` |
| Prix de transfert — pleine concurrence | 57 CGI | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069577", num: "57")` |
| Intégration fiscale | 223 A et s. CGI | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069577", num: "223 A")` |
| Amendement Charasse | 223 B CGI | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069577", num: "223 B")` |
| Prescription fiscale | L169 LPF | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069583", num: "L169")` |

### SOCIAL

| Sujet | Article(s) | Outil MCP |
|-------|-----------|-----------|
| CSE — mise en place | L2311-2 C. trav. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006072050", num: "L2311-2")` |
| CSE — consultation | L2312-8 C. trav. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006072050", num: "L2312-8")` |
| Loi Hamon — information salariés | L23-10-1 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L23-10-1")` |
| Loi Hamon — sanctions | L23-10-6 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L23-10-6")` |
| Transfert d'entreprise | L1224-1 C. trav. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006072050", num: "L1224-1")` |
| Forfait jours | L3121-58 C. trav. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006072050", num: "L3121-58")` |
| Participation | L3322-1 C. trav. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006072050", num: "L3322-1")` |
| Intéressement | L3311-1 C. trav. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006072050", num: "L3311-1")` |
| Barème Macron | L1235-3 C. trav. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006072050", num: "L1235-3")` |
| Non-concurrence | Jurisp. Cass. soc. | `searchUsingPOST` fond JURI, "clause non-concurrence contrepartie" |
| Requalification | L8221-6 C. trav. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006072050", num: "L8221-6")` |
| Convention collective | Par IDCC | `displayKaliContByIdccUsingPOST(id: "<IDCC>")` |

### PROPRIÉTÉ INTELLECTUELLE

| Sujet | Article(s) | Outil MCP |
|-------|-----------|-----------|
| Brevets — principes | L611-1 et s. CPI | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069414", num: "L611-1")` |
| Inventions de salariés | L611-7 CPI | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069414", num: "L611-7")` |
| Déchéance brevet | L612-12 CPI | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069414", num: "L612-12")` |
| Marques | L711-1 et s. CPI | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069414", num: "L711-1")` |
| Déchéance marque non-usage | L714-5 CPI | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069414", num: "L714-5")` |
| Contrefaçon marque | L716-1 CPI | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069414", num: "L716-1")` |
| Contrefaçon brevet | L615-1 CPI | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069414", num: "L615-1")` |
| Logiciels — salariés | L113-9 CPI | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069414", num: "L113-9")` |
| Droit d'auteur | L111-1 CPI | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069414", num: "L111-1")` |
| Bases de données | L341-1 CPI | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069414", num: "L341-1")` |
| Dessins et modèles | L511-1 CPI | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069414", num: "L511-1")` |

### CONTRATS COMMERCIAUX

| Sujet | Article(s) | Outil MCP |
|-------|-----------|-----------|
| Rupture brutale | L442-1 II C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L442-1")` |
| Agent commercial | L134-1 à L134-17 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L134-1")` |
| Indemnité agent | L134-12 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L134-12")` |
| Ententes | L420-1 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L420-1")` |
| Franchise — info précontractuelle | L330-3 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L330-3")` |
| CGV B2B | L441-1 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L441-1")` |
| Clauses abusives | L212-1 C. conso. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006069565", num: "L212-1")` |
| Responsabilité produit | 1245 C. civ. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006070721", num: "1245")` |
| Concurrence déloyale | 1240 C. civ. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006070721", num: "1240")` |
| Sous-traitance | Loi 75-1334 | `searchUsingPOST` fond LODA_DATE, TITLE "sous-traitance" |

### BAUX COMMERCIAUX

| Sujet | Article(s) | Outil MCP |
|-------|-----------|-----------|
| Statut baux commerciaux | L145-1 à L145-60 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L145-1")` |
| Durée / résiliation triennale | L145-4 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L145-4")` |
| Indexation loyer | L145-38 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L145-38")` |
| Solidarité cession | L145-16-2 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L145-16-2")` |
| Droit au renouvellement | L145-8 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L145-8")` |

### FINANCEMENT

| Sujet | Article(s) | Outil MCP |
|-------|-----------|-----------|
| Nantissement fonds de commerce | L142-1 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L142-1")` |
| Nantissement parts sociales | 2355 C. civ. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006070721", num: "2355")` |
| Crédit-bail | L313-7 CMF | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006072026", num: "L313-7")` |
| Garantie autonome | 2321 C. civ. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006070721", num: "2321")` |
| Cautionnement | 2288 et s. C. civ. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006070721", num: "2288")` |

### RÉGLEMENTAIRE

| Sujet | Article(s) | Outil MCP |
|-------|-----------|-----------|
| ICPE | L511-1 C. env. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006074220", num: "L511-1")` |
| Responsabilité environnementale | L160-1 C. env. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006074220", num: "L160-1")` |
| Remise en état ICPE | L512-6-1 C. env. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006074220", num: "L512-6-1")` |
| Sites pollués | L556-1 C. env. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000006074220", num: "L556-1")` |
| Sapin 2 | Loi 2016-1691 | `searchUsingPOST` fond LODA_DATE, TITLE "transparence corruption modernisation" |
| Lanceurs d'alerte | Loi 2022-401 | `searchUsingPOST` fond LODA_DATE, TITLE "lanceurs alerte" |
| Secret des affaires | L151-1 C. com. | `getArticleWithIdAndNumUsingPOST(id: "LEGITEXT000005634379", num: "L151-1")` |

### RGPD / DONNÉES PERSONNELLES

| Sujet | Article(s) | Outil MCP |
|-------|-----------|-----------|
| Loi Informatique et Libertés | Loi 78-17 | `searchUsingPOST` fond LODA_DATE, TITLE "informatique fichiers libertés" |
| Cookies — Art. 82 LIL | Art. 82 Loi 78-17 | Via résultat de la recherche LODA ci-dessus |
| Décisions CNIL | Fond CNIL | `searchUsingPOST` fond CNIL, mots-clés pertinents |
| RGPD | Règlement UE 2016/679 | Non disponible sur Légifrance (JOUE), mais les transpositions nationales le sont |

---

## Recherches jurisprudentielles types

### Fond JURI (Cour de cassation)

```
# Rupture brutale des relations commerciales
searchUsingPOST(fond: "JURI", recherche: {
  champs: [{ typeChamp: "ALL", criteres: [{
    typeRecherche: "TOUS_LES_MOTS_DANS_UN_CHAMP",
    valeur: "rupture brutale relations commerciales établies",
    operateur: "ET"
  }], operateur: "ET" }],
  operateur: "ET", pageNumber: 1, pageSize: 10,
  sort: "DATE_DESC", typePagination: "DEFAUT"
})

# Clause de non-concurrence — contrepartie financière
searchUsingPOST(fond: "JURI", recherche: {
  champs: [{ typeChamp: "ALL", criteres: [{
    typeRecherche: "TOUS_LES_MOTS_DANS_UN_CHAMP",
    valeur: "clause non-concurrence contrepartie financière",
    operateur: "ET"
  }], operateur: "ET" }],
  operateur: "ET", pageNumber: 1, pageSize: 10,
  sort: "DATE_DESC", typePagination: "DEFAUT"
})

# Forfait jours — nullité
searchUsingPOST(fond: "JURI", recherche: {
  champs: [{ typeChamp: "ALL", criteres: [{
    typeRecherche: "TOUS_LES_MOTS_DANS_UN_CHAMP",
    valeur: "forfait jours nullité accord collectif",
    operateur: "ET"
  }], operateur: "ET" }],
  operateur: "ET", pageNumber: 1, pageSize: 10,
  sort: "DATE_DESC", typePagination: "DEFAUT"
})
```

### Fond CETAT (Conseil d'État)

```
# CIR — éligibilité des dépenses
searchUsingPOST(fond: "CETAT", recherche: {
  champs: [{ typeChamp: "ALL", criteres: [{
    typeRecherche: "TOUS_LES_MOTS_DANS_UN_CHAMP",
    valeur: "crédit impôt recherche éligibilité",
    operateur: "ET"
  }], operateur: "ET" }],
  operateur: "ET", pageNumber: 1, pageSize: 10,
  sort: "DATE_DESC", typePagination: "DEFAUT"
})
```

### Fond CNIL (Délibérations CNIL)

```
# Sanctions RGPD
searchUsingPOST(fond: "CNIL", recherche: {
  champs: [{ typeChamp: "ALL", criteres: [{
    typeRecherche: "TOUS_LES_MOTS_DANS_UN_CHAMP",
    valeur: "sanction violation données personnelles",
    operateur: "ET"
  }], operateur: "ET" }],
  operateur: "ET", pageNumber: 1, pageSize: 10,
  sort: "DATE_DECISION_DESC", typePagination: "DEFAUT"
})
```

---

## Convention collective — Navigation

```
# 1. Trouver la convention collective par IDCC
displayKaliContByIdccUsingPOST(id: "<IDCC>")

# 2. Naviguer dans les sections
displayKaliSectionUsingPOST(id: "<KALISCTA_ID>")

# 3. Consulter un article spécifique
displayKaliArticleUsingPOST(id: "<KALIARTI_ID>")

# IDCC fréquents :
# 1486 = Syntec
# 1979 = HCR
# 3248 = Métallurgie
# 2098 = Prestataires de services
# 44 = Industries chimiques
# 176 = Industrie pharmaceutique
# 2120 = Banque
```

---

## Lois par nom courant

| Nom courant | Recherche Légifrance |
|-------------|---------------------|
| Loi PACTE | `searchUsingPOST` fond LODA_DATE, TITLE "plan action croissance transformation" |
| Loi Sapin 2 | `searchUsingPOST` fond LODA_DATE, TITLE "transparence corruption modernisation" |
| Loi Hamon (cession) | Art. L23-10-1 C. com. (intégré au code) |
| Loi Informatique et Libertés | `searchUsingPOST` fond LODA_DATE, TITLE "informatique fichiers libertés" |
| Loi de sous-traitance | `searchUsingPOST` fond LODA_DATE, TITLE "sous-traitance" (Loi 75-1334) |
| Ordonnances Macron (travail) | `searchUsingPOST` fond LODA_DATE, TITLE "renforcement dialogue social" |
| Loi partage de la valeur | `searchUsingPOST` fond LODA_DATE, TITLE "partage valeur entreprise" |
| Loi Climat et Résilience | `searchUsingPOST` fond LODA_DATE, TITLE "climat résilience" |
