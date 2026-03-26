# Installation ATOOX — Claude Code / Cursor

> **Temps estimé : 30 secondes**

---

## Prérequis

- Claude Code installé (CLI) OU Cursor avec Claude intégré
- Node.js >= 18 (uniquement pour les scripts optionnels)

---

## Installation (3 étapes)

### Étape 1 — Décompresser le ZIP

Décompressez `atoox-claude-code.zip` dans un dossier de votre choix.

### Étape 2 — Copier les skills

**Mac / Linux :**
```bash
cp -r skills/* ~/.claude/skills/
```

**Windows (PowerShell) :**
```powershell
Copy-Item -Recurse skills\* "$env:USERPROFILE\.claude\skills\"
```

**Optionnel** — Copier aussi les agents, protocoles et commandes :
```bash
cp -r agents/* ~/.claude/agents/ 2>/dev/null
cp -r protocols/* ~/.claude/protocols/ 2>/dev/null
cp -r commands/* ~/.claude/commands/ 2>/dev/null
```

### Étape 3 — Redémarrer et tester

1. Fermez et rouvrez Claude Code (ou Cursor)
2. Tapez `/welcome` pour l'onboarding guidé
3. Ou directement `/commit` pour tester

---

## Vérification

```bash
ls ~/.claude/skills/ | wc -l
# Devrait afficher 73+ dossiers
```

---

## Commandes Principales

| Commande | Ce qu'elle fait |
|----------|----------------|
| `/atoox` | Orchestrateur principal (détecte et route automatiquement) |
| `/commit` | Commit intelligent |
| `/pr` | Pull request automatique |
| `/fix` | Corriger toutes les erreurs |
| `/atoox --full "feature"` | Pipeline complet (qualité maximale) |
| `/atoox --genesis "projet"` | Créer un projet de A à Z |
| `/welcome` | Onboarding guidé |

---

## Support

- **Site** : https://atoox.com
- **Contact** : https://atoox.com/contact

*ATOOX — Vous avez une idée. Ils sont 73 à la construire avec vous.*
