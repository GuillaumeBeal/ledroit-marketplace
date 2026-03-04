# LeDroit Marketplace

Marketplace de skills en droit francais pour Claude Code.

Ce projet regroupe des plugins et competences permettant a Claude Code d'assister efficacement sur des problematiques de droit francais, en s'appuyant sur les sources officielles via l'API Legifrance.

## Skills et commandes disponibles

### Skill (auto-invoquee par Claude)

| Skill | Description |
|-------|-------------|
| `legifrance` | Invoquee automatiquement pour toute question de droit francais — articles, lois, decrets, jurisprudence, conventions collectives, veille |

### Commandes slash

| Commande | Description |
|----------|-------------|
| `/article` | Consulter un article de code (`/article L225-1 code de commerce`) |
| `/loi` | Trouver une loi par nom courant ou numero (`/loi Sapin 2`) |
| `/jurisprudence` | Rechercher des decisions de justice (`/jurisprudence responsabilite 2024`) |
| `/convention` | Consulter une convention collective (`/convention Syntec`) |
| `/veille` | Veille juridique par domaine et periode (`/veille droit du travail 3 mois`) |
| `/jo` | Derniers textes du Journal Officiel (`/jo`) |
| `/verifier` | Verifier une citation juridique (`/verifier art. 1382 code civil`) |

## MCP Servers

### Legifrance (DILA - API PISTE)

Connecteur vers l'API officielle Legifrance, donnant acces a l'integralite du droit francais publie :

| Fonds | Description | Outil principal |
|-------|-------------|-----------------|
| **JORF** | Journal Officiel | `displayJorfUsingPOST` |
| **CODE** | Codes en vigueur | `displayCodeUsingPOST` |
| **LODA** | Lois et decrets consolides | `displayLawDecreeUsingPOST` |
| **JURI** | Jurisprudence judiciaire | `displayJuriUsingPOST` |
| **CETAT** | Jurisprudence administrative | `displayJuriUsingPOST` |
| **CONSTIT** | Conseil constitutionnel | `displayJuriUsingPOST` |
| **KALI** | Conventions collectives | `displayKaliContUsingPOST` |
| **CNIL** | Deliberations CNIL | `displayCnilUsingPOST` |
| **CIRC** | Circulaires | `displayCirculaireUsingPOST` |
| **ACCO** | Accords d'entreprise | `displayAccoUsingPOST` |

**Fonctionnalites :**
- Recherche plein texte multi-fonds (`searchUsingPOST`)
- Consultation de codes a une date donnee (versions consolidees)
- Navigation dans les tables des matieres
- Recuperation d'articles individuels avec historique des versions
- Acces aux conventions collectives par IDCC
- Consultation des dossiers legislatifs
- Acces au Journal Officiel par date ou numero

### data.gouv.fr

Connecteur vers la plateforme open data du gouvernement francais. Permet de rechercher et interroger les jeux de donnees publics.

## Structure du projet

```
ledroit-marketplace/
├── .claude-plugin/
│   └── marketplace.json        # Registre de la marketplace
├── plugins/
│   └── legifrance-plugin/      # Plugin Legifrance (droit francais)
│       ├── .claude-plugin/plugin.json
│       ├── .mcp.json               # Serveur MCP Legifrance (streamable-http)
│       ├── skills/
│       │   └── legifrance/         # Skill auto-invoquee
│       │       ├── SKILL.md
│       │       └── references/
│       └── commands/               # Commandes slash (/article, /loi, etc.)
│           ├── article.md
│           ├── loi.md
│           ├── jurisprudence.md
│           ├── convention.md
│           ├── veille.md
│           ├── jo.md
│           └── verifier.md
├── CLAUDE.md                   # Instructions pour Claude Code
└── README.md                   # Ce fichier
```

## Configuration MCP

Pour utiliser le serveur Legifrance, ajoutez-le a votre configuration MCP Claude Code. Le serveur se connecte a l'API PISTE de la DILA (Direction de l'information legale et administrative).

Le plugin inclut un fichier `.mcp.json` pret a l'emploi. Pour l'activer dans un projet Claude Code, copiez-le a la racine de votre projet ou ajoutez la configuration dans `~/.claude/settings.json` :

```json
{
  "mcpServers": {
    "legifrance": {
      "type": "streamable-http",
      "url": "https://legifrance.stellarspace.tech/mcp"
    }
  }
}
```

## Contribuer

Pour ajouter une nouvelle command :

1. Creer un dossier dans `plugins/<nom-plugin>/`
2. Ajouter un `plugin.json` dans `.claude-plugin/`
3. Creer la command dans `commands/<nom-command>.md`
4. Enregistrer le plugin dans `.claude-plugin/marketplace.json`

## Licence

Projet open source. Les donnees juridiques sont issues de sources publiques (Legifrance / DILA).
