# Installation ATOOX — Claude.ai (Web) / Claude Desktop

> **Temps estimé : 2 minutes**
> Pas besoin de terminal. Tout se fait depuis votre navigateur.

---

## Prérequis

- Un compte Claude (claude.ai) avec un abonnement Pro, Team ou Enterprise
- L'accès à la fonctionnalité « Compétences » (Skills)

---

## Installation (3 étapes)

### Étape 1 — Ouvrir la page Compétences

Allez sur : **https://claude.ai/customize/skills**

Ou depuis Claude.ai :
1. Cliquez sur votre avatar (en haut à droite)
2. « Personnaliser Claude »
3. « Compétences » (Skills)

### Étape 2 — Téléverser les skills

1. Cliquez sur **« Ajouter des compétences »**
2. Sélectionnez les fichiers `.skill` depuis le dossier `skills/` du ZIP
3. Vous pouvez les ajouter un par un ou par lot

**Conseil** : Commencez par les 5 essentiels :
- `commit.skill`
- `create-pr.skill`
- `fix-errors.skill`
- `oneshot.skill`
- `ultrathink.skill`

Puis ajoutez ceux qui correspondent à votre métier :
- **Développeur** : `atoox-sonar-pro.skill`, `atoox-test-pro.skill`
- **Product Manager** : `atoox-spec-pro.skill`, `atoox-vision-pro.skill`
- **Marketeur** : `atoox-copy-pro.skill`, `atoox-seo-pro.skill`
- **Freelance** : `atoox.skill` (le framework complet)

### Étape 3 — Utiliser dans une conversation

Une fois les skills ajoutés, ils sont disponibles dans **toutes vos conversations**.

Tapez simplement votre demande. Si un skill correspond, Claude l'utilisera automatiquement.

Exemples :
- « Audite la qualité de mon code » → utilise atoox-sonar-pro
- « Rédige les specs de ma feature » → utilise atoox-spec-pro
- « Optimise le copy de ma landing page » → utilise atoox-copy-pro

---

## Différences avec Claude Code

| Fonctionnalité | Claude Code (CLI) | Claude.ai (Web) |
|---------------|-------------------|-----------------|
| Commandes slash (`/commit`) | ✅ | ❌ (décrivez en langage naturel) |
| Exécution de code | ✅ | ❌ (analyse uniquement) |
| Modification de fichiers | ✅ | ❌ (suggestions uniquement) |
| Analyse et conseils | ✅ | ✅ |
| Audit et review | ✅ | ✅ |
| Spécifications | ✅ | ✅ |
| Copywriting | ✅ | ✅ |

> **Note** : Sur Claude.ai (web), les skills fonctionnent en mode **conseil et analyse**.
> Ils ne peuvent pas modifier directement vos fichiers. Pour l'exécution automatique,
> utilisez Claude Code (CLI) ou Cursor.

---

## Support

- **Site** : https://atoox.com
- **Contact** : https://atoox.com/contact

*ATOOX — Vous avez une idée. Ils sont 73 à la construire avec vous.*
