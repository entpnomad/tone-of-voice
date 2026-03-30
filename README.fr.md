# tone-of-voice

🌐 [English](README.md) | [Español](README.es.md) | [Français](README.fr.md) | [Italiano](README.it.md)

Un skill Claude Code qui apprend ta voix — personnelle ou de marque, parce que la plupart du temps la voix du fondateur *est* la marque — et l'applique dans tout ce que tu écris.

## Skills complémentaires

Fonctionne avec des skills d'optimisation de contenu pour que ta voix survive à l'optimisation :
- [ai-rank](https://github.com/entpnomad/ai-rank) — Optimise pour les moteurs de réponse LLM et les agents IA, en préservant ta voix
- [seo-rank](https://github.com/entpnomad/seo-rank) — Audit et optimisation SEO qui respecte le ton de ta marque

ai-rank et seo-rank consultent tous deux tone-of-voice pour préserver ta voix lors des réécritures de contenu.

## Pourquoi

En tant que fondateur, j'écris la majorité de la communication de mon entreprise — newsletters, landing pages, emails, posts sur les réseaux sociaux, READMEs. Et oui, j'utilise l'IA sans aucun complexe. Les idées sont les miennes. Je dicte la réflexion de base avec [Whispering](https://github.com/braden-w/whispering) sur Mac, puis Claude écrit le brouillon. Mais l'IA sans garde-fous produit de la bouillie. Même structure, mêmes formulations, le même ton corporate sans âme à chaque fois. Ce skill règle le problème. Il apprend à Claude comment je parle — mon vocabulaire, mes opinions, mes expressions interdites — pour que le résultat se lise comme moi, pas comme un communiqué de presse.

## Comment ça marche

La première fois que tu lances `/tone-of-voice`, il te pose 9 questions : qui tu es, ta conviction fondamentale, ton audience, tes traits de voix, tes préférences de vocabulaire, tes expressions interdites, tes canaux et des exemples d'écriture. Les réponses sont sauvegardées dans le système de mémoire de Claude Code — persistantes d'une session à l'autre.

Chaque fois après, il applique ton profil de voix à ce que tu es en train d'écrire.

## Installation

```bash
mkdir -p ~/.claude/skills/tone-of-voice
curl -sL https://raw.githubusercontent.com/entpnomad/tone-of-voice/main/SKILL.md \
  -o ~/.claude/skills/tone-of-voice/SKILL.md
```

## Utilisation

```
/tone-of-voice
```

Premier lancement : configuration interactive (~5 minutes). Lancements suivants : mode application.

### Commandes

| Commande | Ce qu'elle fait |
|----------|----------------|
| `/tone-of-voice` | Applique la voix au contenu actuel ou lance la configuration |
| `update my tone-of-voice vocabulary` | Modifie une section spécifique |
| `show my tone-of-voice` | Affiche ton profil de voix complet |

## Ce qu'il sauvegarde

Neuf fichiers mémoire couvrant ton identité, tes convictions, ton audience, tes traits, tes sujets, ton vocabulaire, tes expressions interdites, tes règles par canal et tes exemples de référence. Le tout stocké dans le répertoire mémoire de Claude Code — les données t'appartiennent.

## Licence

MIT
