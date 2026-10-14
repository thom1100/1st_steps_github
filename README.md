# Kiné — système multi-agents de révision

Configuration Claude Code : l'orchestrateur (« étudiant expert en kiné ») est
décrit dans `CLAUDE.md`, les sous-agents dans `.claude/agents/` :

| Agent | Rôle |
|---|---|
| `professeur` | Explications approfondies basées sur `cours/` |
| `coach` | Fiches express quand il reste peu de temps |
| `revision` | Questionnaires d'entraînement pour les partiels + bilan |
| `anki` | Flashcards recto/verso avec répétition espacée (Leitner) |
| `schemas` | Schémas Mermaid / SVG / HTML des cours |
| `memoire` | Journal, questions récurrentes, points faibles |

## Exemples de demandes
- « C'est quoi la différence entre tendinopathie et tendinite ? » → professeur
- « J'ai 10 min avant le partiel d'anat du genou » → coach
- « Fais-moi réviser la physio respiratoire, 15 questions » → revision
- « Crée des cartes sur les vertèbres » puis « Lance le mode anki » → anki
- « Schéma des muscles de la coiffe des rotateurs » → schemas
- « Qu'est-ce que je rate le plus en ce moment ? » → memoire
