# Installation ATOOX — Gemini CLI / Codex / Autres Agents

> **Temps estimé : 5 minutes**
> Les skills ATOOX sont des fichiers Markdown. Tout agent IA qui lit du Markdown peut les utiliser.

---

## Principe

Les skills ATOOX sont des **instructions structurées en Markdown** avec des métadonnées YAML. Ils ne dépendent d'aucune plateforme spécifique.

Chaque fichier `SKILL.md` contient :
1. Un **frontmatter YAML** (nom, description, triggers, modes)
2. Des **instructions détaillées** que l'agent IA suit

---

## Installation Générique

### Étape 1 — Identifier le dossier d'instructions de votre agent

| Agent | Dossier d'instructions |
|-------|----------------------|
| **Gemini CLI** | Dossier de contexte configuré dans `.gemini/` |
| **Codex (OpenAI)** | System prompt ou dossier de contexte |
| **Aider** | Fichier `.aider.conf.yml` → extra_files |
| **Continue.dev** | `.continue/` directory |
| **Autre** | Consultez la doc de votre agent |

### Étape 2 — Copier les skills

Copiez les fichiers `SKILL.md` dans le dossier d'instructions de votre agent.

```bash
# Exemple pour un dossier générique
cp -r skills/ /chemin/vers/votre/agent/instructions/
```

### Étape 3 — Adapter les triggers (si nécessaire)

Les skills ATOOX utilisent des commandes slash (`/commit`, `/fix`, etc.) comme triggers.
Si votre agent ne supporte pas les slash-commands, utilisez les **mots-clés** listés dans le frontmatter YAML de chaque skill.

Exemple pour `atoox-sonar-pro` :
```yaml
triggers:
  - 'audit code'
  - 'code review'
  - 'qualité code'
  - 'dette technique'
```

→ Au lieu de taper `/atoox-sonar-pro`, tapez « audit code » ou « code review ».

### Étape 4 — Tester

Demandez à votre agent : « Audite la qualité de mon code »

Si le skill est chargé correctement, l'agent suivra les instructions du SKILL.md.

---

## Limitations Selon la Plateforme

| Fonctionnalité | Fonctionne partout | Nécessite Claude Code |
|---------------|--------------------|--------------------|
| Conseils et analyse | ✅ | — |
| Audit de code | ✅ | — |
| Spécifications | ✅ | — |
| Copywriting | ✅ | — |
| Exécution de code | — | ✅ |
| Modification de fichiers | — | ✅ |
| Commit + PR automatique | — | ✅ |
| Pipeline 39 steps | — | ✅ |

> Les skills fonctionnent en **mode conseil** sur toutes les plateformes.
> L'**exécution automatique** (écriture de code, commits, PR) nécessite Claude Code ou Cursor.

---

## Support

- **Site** : https://atoox.com
- **Contact** : https://atoox.com/contact

*ATOOX — Vous avez une idée. Ils sont 73 à la construire avec vous.*
