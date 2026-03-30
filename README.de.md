# tone-of-voice

🌐 [English](README.md) | [Español](README.es.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Português](README.pt.md) | [Deutsch](README.de.md)

Ein Claude Code Skill, der deine Stimme lernt — persoenlich oder als Marke, denn meistens *ist* die Stimme des Gruenders die Marke — und sie in allem durchsetzt, was du schreibst.

## Begleit-Skills

Funktioniert zusammen mit Content-Optimierungs-Skills, damit deine Stimme die Optimierung ueberlebt:
- [ai-rank](https://github.com/entpnomad/ai-rank) — Optimiert fuer LLM-Antwortmaschinen und KI-Agenten, bewahrt deine Stimme
- [seo-rank](https://github.com/entpnomad/seo-rank) — SEO-Audit und Optimierung, die deinen Markenton respektiert

Sowohl ai-rank als auch seo-rank nutzen tone-of-voice, um deine Stimme bei Content-Rewrites zu bewahren.

## Warum

Als Gruender schreibe ich den Grossteil der Kommunikation meines Unternehmens — Newsletter, Landing Pages, E-Mails, Social-Media-Posts, READMEs. Und ja, ich nutze ungeniert KI. Die Ideen sind meine. Ich diktiere den Kerngedanken mit [Whispering](https://github.com/braden-w/whispering) auf dem Mac, dann schreibt Claude den Entwurf. Aber KI ohne Leitplanken produziert Einheitsbrei. Gleiche Struktur, gleiche Formulierungen, der gleiche leblose Corporate-Ton jedes Mal. Dieser Skill behebt das. Er bringt Claude bei, wie ich klinge — mein Vokabular, meine Meinungen, meine verbotenen Phrasen — damit das Ergebnis sich wie ich liest, nicht wie eine Pressemitteilung.

## Wie es funktioniert

Beim ersten Start von `/tone-of-voice` stellt es dir 9 Fragen: wer du bist, deine Kernueberzeugung, dein Publikum, Stimmmerkmale, Vokabular-Praeferenzen, verbotene Phrasen, Kanaele und Schreibbeispiele. Die Antworten werden im Gedaechtnissystem von Claude Code gespeichert — persistent ueber Sessions hinweg.

Jedes Mal danach wendet es dein Stimmprofil auf das an, was du gerade schreibst.

## Installation

```bash
mkdir -p ~/.claude/skills/tone-of-voice
curl -sL https://raw.githubusercontent.com/entpnomad/tone-of-voice/main/SKILL.md \
  -o ~/.claude/skills/tone-of-voice/SKILL.md
```

## Nutzung

```
/tone-of-voice
```

Erster Start: interaktives Setup (~5 Minuten). Weitere Starts: Anwendungsmodus.

### Befehle

| Befehl | Was er macht |
|--------|-------------|
| `/tone-of-voice` | Wendet die Stimme auf aktuellen Content an oder startet das Setup |
| `update my tone-of-voice vocabulary` | Bearbeitet einen bestimmten Abschnitt |
| `show my tone-of-voice` | Zeigt dein vollstaendiges Stimmprofil an |

## Was es speichert

Neun Gedaechtnis-Dateien, die deine Identitaet, Ueberzeugungen, Publikum, Merkmale, Themen, Vokabular, verbotene Phrasen, Kanal-Regeln und Referenzbeispiele abdecken. Alles im Gedaechtnis-Verzeichnis von Claude Code gespeichert — die Daten gehoeren dir.

## Lizenz

MIT
