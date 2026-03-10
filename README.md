# Jean-Claude Marketplace

Marketplace de plugins pour [Claude Code](https://claude.com/claude-code), orienté consulting et exploration d'applications VPSoft.

## Présentation

Ce dépôt centralise des **skills**, **commandes** et **références documentaires** utilisables par Claude Code via le protocole MCP (Model Context Protocol). Il permet à Claude Code d'explorer, analyser et documenter des applications construites sur la plateforme low-code VPSoft.

## Plugin disponible

### vpsoft-plugin (v1.0.1)

Toolkit complet pour le consulting VPSoft :

| Domaine | Description |
|---------|-------------|
| **Modèle de données** | Exploration de 233+ entités, champs, types et relations |
| **Code dynamique** | Lecture de 38+ points d'injection (C#, JS, CSS, Razor) |
| **Audit & diagnostic** | Erreurs applicatives, historique des modifications, trail utilisateur, logs email |
| **Module formulaire** | Questionnaires, campagnes, formules, import/export Excel |
| **Permissions** | Rôles à 3 niveaux (application, module, champ) |
| **Diagrammes** | Génération de schémas Mermaid (ERD, flux, architecture) |

#### 15 outils MCP

- **Data access** : `get_all_entities`, `get_entity_fields`, `get_entity_sample_data`, `get_many_select`, `get_entities_count`, `invoke_vpsoft_function`
- **CRUD** : `create_entity`, `update_entity_patch`, `get_entity_url`
- **Audit** : `get_app_errors`, `get_audit_history`, `get_audit_trail`, `get_mail_logs`, `get_audit_versions`, `get_cascade_logs`

## Structure du dépôt

```
jean-claude-marketplace/
├── .claude-plugin/
│   └── marketplace.json          # Registre central du marketplace
├── plugins/
│   └── vpsoft-plugin/
│       ├── .mcp.json             # Configuration serveur MCP
│       ├── .claude-plugin/
│       │   └── plugin.json       # Métadonnées du plugin
│       └── skills/
│           └── consulting-vpsoft/
│               ├── SKILL.md      # 13 workflows documentés
│               ├── README.md
│               ├── claude.md
│               └── references/   # 7 fichiers de référence
│                   ├── tools-catalog.md
│                   ├── where-syntax.md
│                   ├── agl-architecture.md
│                   ├── code-injection.md
│                   ├── csharp-source.md
│                   ├── modules-menu.md
│                   └── form-module.md
├── CLAUDE.md
└── README.md
```

## Installation

1. Cloner le dépôt dans votre espace de travail Claude Code
2. Le marketplace est automatiquement détecté via `.claude-plugin/marketplace.json`
3. Le serveur MCP VPSoft doit être accessible à `https://vestax.topinambour.space/mcp`

## Auteur

**Guillaume Béal**

## Licence

Projet privé — tous droits réservés.
