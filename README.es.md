# tone-of-voice

🌐 [English](README.md) | [Español](README.es.md) | [Français](README.fr.md) | [Italiano](README.it.md)

Un skill de Claude Code que aprende tu voz — personal o de marca, porque la mayoría de las veces la voz del fundador *es* la marca — y la aplica en todo lo que escribes.

## Skills complementarios

Funciona junto con skills de optimización de contenido para que tu voz sobreviva a la optimización:
- [ai-rank](https://github.com/entpnomad/ai-rank) — Optimiza para motores de respuesta LLM y agentes de IA, preservando tu voz
- [seo-rank](https://github.com/entpnomad/seo-rank) — Auditoría y optimización SEO que respeta el tono de tu marca

Tanto ai-rank como seo-rank consultan tone-of-voice para preservar tu voz durante las reescrituras de contenido.

## Por qué

Como fundador, escribo la mayoría de la comunicación de mi empresa — newsletters, landing pages, emails, posts en redes sociales, READMEs. Y sí, uso IA sin ningún reparo. Las ideas son mías. Dicto el pensamiento central con [Whispering](https://github.com/braden-w/whispering) en Mac, y después Claude escribe el borrador. Pero la IA sin límites produce basura. Misma estructura, mismas frases, el mismo tono corporativo sin vida una y otra vez. Este skill lo soluciona. Le enseña a Claude cómo sueno — mi vocabulario, mis opiniones, mis frases prohibidas — para que el resultado se lea como yo, no como un comunicado de prensa.

## Cómo funciona

La primera vez que ejecutas `/tone-of-voice`, te hace 9 preguntas: quién eres, tu creencia central, tu audiencia, rasgos de voz, preferencias de vocabulario, frases prohibidas, canales y ejemplos de escritura. Las respuestas se guardan en el sistema de memoria de Claude Code — persistentes entre sesiones.

Cada vez después de eso, aplica tu perfil de voz a lo que sea que estés escribiendo.

## Instalación

```bash
mkdir -p ~/.claude/skills/tone-of-voice
curl -sL https://raw.githubusercontent.com/entpnomad/tone-of-voice/main/SKILL.md \
  -o ~/.claude/skills/tone-of-voice/SKILL.md
```

## Uso

```
/tone-of-voice
```

Primera ejecución: configuración interactiva (~5 minutos). Ejecuciones posteriores: modo aplicación.

### Comandos

| Comando | Qué hace |
|---------|----------|
| `/tone-of-voice` | Aplica la voz al contenido actual o inicia la configuración |
| `update my tone-of-voice vocabulary` | Edita una sección específica |
| `show my tone-of-voice` | Muestra tu perfil de voz completo |

## Qué guarda

Nueve archivos de memoria que cubren tu identidad, creencias, audiencia, rasgos, temas, vocabulario, frases prohibidas, reglas por canal y ejemplos de referencia. Todo almacenado en el directorio de memoria de Claude Code — los datos son tuyos.

## Licencia

MIT
