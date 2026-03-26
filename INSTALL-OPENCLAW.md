# Installation ATOOX — OpenClaw.ai / Agents Autonomes

> **Temps estimé : 5 minutes**
> ATOOX + OpenClaw = vos 47 agents experts qui travaillent 24/7.

---

## Prérequis

- Un compte OpenClaw.ai
- Un projet configuré

---

## Installation

### Étape 1 — Décompresser le ZIP

Décompressez `atoox-openclaw.zip` dans votre projet.

### Étape 2 — Configurer l'agent OpenClaw

Dans la configuration de votre agent OpenClaw, pointez vers les fichiers ATOOX :

1. **Skills** : Ajoutez le dossier `skills/` comme source d'instructions
2. **Agents** : Chargez les définitions depuis `agents/`
3. **Protocoles** : Référencez `protocols/` pour les standards de qualité

### Étape 3 — Configurer les triggers

Dans OpenClaw, configurez les triggers pour chaque skill :
- Les triggers sont listés dans le frontmatter YAML de chaque SKILL.md
- Exemple : `atoox-sonar-pro` se déclenche sur « audit code », « code review », etc.

### Étape 4 — Tester

Lancez une tâche simple :
- « Audite la qualité du code du fichier main.ts »
- L'agent devrait charger atoox-sonar-pro et exécuter l'audit

---

## Cas d'Usage avec OpenClaw

| Scénario | Skills activés | Fréquence |
|----------|---------------|-----------|
| Audit code quotidien | sonar-pro, test-pro | Chaque commit |
| Veille concurrents | watch, market-audit | Hebdomadaire |
| Review PR automatique | sonar-pro, a11y-pro, perf-pro | Chaque PR |
| Rapport KPI | kpi-pro, dashboard | Hebdomadaire |
| Audit sécurité | sonar-pro --security, compliance | Mensuel |

---

## Support

- **Site** : https://atoox.com
- **Contact** : https://atoox.com/contact

*ATOOX — Vous avez une idée. Ils sont 73 à la construire avec vous.*
