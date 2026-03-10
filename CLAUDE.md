# Jean-Claude Marketplace

## Projet

Marketplace de plugins pour Claude Code, orienté consulting VPSoft. Ce dépôt contient des skills, commandes et références documentaires utilisables par Claude Code via le protocole MCP (Model Context Protocol).

## Structure

```
.claude-plugin/marketplace.json   # Registre du marketplace
plugins/
  vpsoft-plugin/                   # Plugin actif — consulting VPSoft
    .mcp.json                      # Config serveur MCP (streamable-http)
    .claude-plugin/plugin.json     # Métadonnées du plugin
    skills/consulting-vpsoft/
      SKILL.md                     # Définition principale du skill (13 workflows)
      references/                  # 7 fichiers de référence détaillés
```

## Conventions

- Les plugins sont dans `plugins/<nom-plugin>/`
- Chaque plugin contient un `.claude-plugin/plugin.json` (nom, description, version)
- Les skills sont dans `skills/<nom-skill>/SKILL.md`
- Les documents de référence sont dans `skills/<nom-skill>/references/`
- Le fichier `.mcp.json` à la racine d'un plugin configure la connexion MCP
- La documentation est rédigée en français

## Plugin actif : vpsoft-plugin (v1.0.1)

Toolkit de consulting pour explorer une application VPSoft via MCP :
- **Modèle de données** : 233+ entités, champs, relations
- **Code dynamique** : 38+ points d'injection (C#, JS, CSS, Razor)
- **Audit & diagnostic** : erreurs, historique, trail, mails, versions
- **Module formulaire** : 40+ entités (questionnaires, campagnes, formules)
- **Permissions** : 3 niveaux (application, module, champ)
- **15 outils MCP** disponibles (data access, CRUD, audit)

## Serveur MCP

URL : `https://vestax.topinambour.space/mcp` (type: streamable-http)

## Commandes utiles

```bash
# Pas de build ni de dépendances — documentation pure
git log --oneline -10   # Historique récent
```
