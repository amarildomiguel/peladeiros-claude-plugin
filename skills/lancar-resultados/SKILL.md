---
name: lancar-resultados
description: Lança resultados de jogos de um campeonato do Peladeiros e mostra a classificação actualizada. Usar quando o utilizador diz o resultado de um jogo, quer corrigir um resultado, adiar um jogo ou ver a tabela de um campeonato que gere.
---

# Lançar resultados no Peladeiros

Responde sempre em português de Angola.

## Passos

1. **Encontrar o campeonato.** Usa `listar-campeonatos` se o utilizador não indicar qual. Se houver mais de um com nome parecido, pergunta.
2. **Encontrar o jogo.** Usa `ver-campeonato` para obter os próximos jogos e os últimos resultados, com o `id` de cada jogo. Confirma com o utilizador as duas equipas antes de lançar.
3. **Lançar o resultado.** Usa `lancar-resultado` com os golos de cada equipa. Nas variantes ou fases sem empate (por exemplo, eliminatórias) é preciso indicar o vencedor ou o resultado dos penáltis; se faltar, pergunta.
4. **Outras alterações.** A mesma ferramenta muda o estado (adiado, cancelado), a data e o campo de um jogo.
5. **Mostrar a tabela.** Depois de lançar, usa `ver-campeonato` para mostrar a classificação actualizada e, se o utilizador quiser, `texto-partilha` para preparar a mensagem do WhatsApp.

## Boas práticas

- Lança um jogo de cada vez e confirma cada resultado lido de uma fotografia ou de uma lista antes de o enviar.
- Não inventes resultados nem identificadores de jogos.
