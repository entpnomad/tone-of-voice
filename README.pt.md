# tone-of-voice

🌐 [English](README.md) | [Español](README.es.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Português](README.pt.md) | [Deutsch](README.de.md)

Um skill de Claude Code que aprende a tua voz — pessoal ou de marca, porque na maioria das vezes a voz do fundador *e* a marca — e aplica-a em tudo o que escreves.

## Skills Complementares

Funciona em conjunto com skills de otimizacao de conteudo para garantir que a tua voz sobrevive a otimizacao:
- [ai-rank](https://github.com/entpnomad/ai-rank) — Otimiza para motores de resposta LLM e agentes de IA, preservando a tua voz
- [seo-rank](https://github.com/entpnomad/seo-rank) — Auditoria e otimizacao SEO que respeita o tom da tua marca

Tanto ai-rank como seo-rank consultam tone-of-voice para preservar a tua voz durante as reescritas de conteudo.

## Porquê

Como fundador, escrevo a maior parte da comunicacao da minha empresa — newsletters, landing pages, emails, posts nas redes sociais, READMEs. E sim, uso IA sem qualquer problema. As ideias sao minhas. Dito o pensamento central com [Whispering](https://github.com/braden-w/whispering) no Mac, e depois o Claude escreve o rascunho. Mas a IA sem limites produz lixo. Mesma estrutura, mesmas frases, o mesmo tom corporativo sem vida sempre. Este skill resolve isso. Ensina o Claude como eu falo — o meu vocabulario, as minhas opinioes, as minhas frases proibidas — para que o resultado se leia como eu, nao como um comunicado de imprensa.

## Como funciona

Na primeira vez que executas `/tone-of-voice`, faz-te 9 perguntas: quem es, a tua crenca central, a tua audiencia, tracos de voz, preferencias de vocabulario, frases proibidas, canais e exemplos de escrita. As respostas sao guardadas no sistema de memoria do Claude Code — persistentes entre sessoes.

Todas as vezes depois disso, aplica o teu perfil de voz ao que quer que estejas a escrever.

## Instalacao

```bash
mkdir -p ~/.claude/skills/tone-of-voice
curl -sL https://raw.githubusercontent.com/entpnomad/tone-of-voice/main/SKILL.md \
  -o ~/.claude/skills/tone-of-voice/SKILL.md
```

## Utilizacao

```
/tone-of-voice
```

Primeira execucao: configuracao interativa (~5 minutos). Execucoes seguintes: modo aplicacao.

### Comandos

| Comando | O que faz |
|---------|-----------|
| `/tone-of-voice` | Aplica a voz ao conteudo atual ou inicia a configuracao |
| `update my tone-of-voice vocabulary` | Edita uma seccao especifica |
| `show my tone-of-voice` | Mostra o teu perfil de voz completo |

## O que guarda

Nove ficheiros de memoria que cobrem a tua identidade, crencas, audiencia, tracos, topicos, vocabulario, frases proibidas, regras por canal e exemplos de referencia. Tudo armazenado no diretorio de memoria do Claude Code — os dados sao teus.

## Licenca

MIT
