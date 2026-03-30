# tone-of-voice

🌐 [English](README.md) | [Español](README.es.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Português](README.pt.md) | [Deutsch](README.de.md)

Uno skill di Claude Code che impara la tua voce — personale o di brand, perché il più delle volte la voce del fondatore *è* il brand — e la applica in tutto quello che scrivi.

## Skill complementari

Funziona insieme a skill di ottimizzazione dei contenuti per assicurare che la tua voce sopravviva all'ottimizzazione:
- [ai-rank](https://github.com/entpnomad/ai-rank) — Ottimizza per motori di risposta LLM e agenti IA, preservando la tua voce
- [seo-rank](https://github.com/entpnomad/seo-rank) — Audit e ottimizzazione SEO che rispetta il tono del tuo brand

Sia ai-rank che seo-rank consultano tone-of-voice per preservare la tua voce durante le riscritture dei contenuti.

## Perché

Come fondatore, scrivo la maggior parte della comunicazione della mia azienda — newsletter, landing page, email, post sui social, README. E sì, uso l'IA senza alcun problema. Le idee sono mie. Detto il pensiero centrale con [Whispering](https://github.com/braden-w/whispering) su Mac, poi Claude scrive la bozza. Ma l'IA senza limiti produce spazzatura. Stessa struttura, stesse frasi, lo stesso tono corporate senza vita ogni volta. Questo skill risolve il problema. Insegna a Claude come parlo — il mio vocabolario, le mie opinioni, le mie frasi vietate — così che il risultato si legga come me, non come un comunicato stampa.

## Come funziona

La prima volta che lanci `/tone-of-voice`, ti fa 9 domande: chi sei, la tua convinzione centrale, il tuo pubblico, i tratti della tua voce, le preferenze di vocabolario, le frasi vietate, i canali e degli esempi di scrittura. Le risposte vengono salvate nel sistema di memoria di Claude Code — persistenti tra le sessioni.

Ogni volta dopo, applica il tuo profilo vocale a qualsiasi cosa tu stia scrivendo.

## Installazione

```bash
mkdir -p ~/.claude/skills/tone-of-voice
curl -sL https://raw.githubusercontent.com/entpnomad/tone-of-voice/main/SKILL.md \
  -o ~/.claude/skills/tone-of-voice/SKILL.md
```

## Uso

```
/tone-of-voice
```

Primo lancio: configurazione interattiva (~5 minuti). Lanci successivi: modalità applicazione.

### Comandi

| Comando | Cosa fa |
|---------|---------|
| `/tone-of-voice` | Applica la voce al contenuto attuale o avvia la configurazione |
| `update my tone-of-voice vocabulary` | Modifica una sezione specifica |
| `show my tone-of-voice` | Mostra il tuo profilo vocale completo |

## Cosa salva

Nove file di memoria che coprono la tua identità, convinzioni, pubblico, tratti, argomenti, vocabolario, frasi vietate, regole per canale ed esempi di riferimento. Tutto archiviato nella directory di memoria di Claude Code — i dati sono tuoi.

## Licenza

MIT
