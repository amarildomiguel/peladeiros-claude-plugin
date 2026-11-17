---
name: organizar-campeonato
description: Organiza um campeonato de futebol no Peladeiros do início ao calendário. Usar quando o utilizador quer criar um torneio, liga ou campeonato de futebol 11, futebol 7, futebol 5, futsal ou futebol de praia, aprovar equipas inscritas ou gerar os jogos.
---

# Organizar um campeonato no Peladeiros

O Peladeiros (peladeiros.ao) é só de futebol: futebol 11, futebol 7, futebol 5, futsal e futebol de praia. Responde sempre em português de Angola.

## Passos

1. **Escolher a variante e o formato.** Usa `listar-modalidades-e-formatos` para mostrar as variantes (jogadores em campo, duração, se há empate) e os formatos: liga, eliminatória, grupos com eliminatórias, suíço, eliminatória dupla e amigáveis. Se o utilizador não disser, pergunta a variante e o formato antes de criar.
2. **Criar o campeonato.** Usa `criar-campeonato` com o nome, a variante e o formato. O campeonato nasce em rascunho e o utilizador fica como organizador. Lembra que o plano gratuito vai até 100 jogadores por campeonato; para mais, `ver-planos` mostra os contactos.
3. **Receber inscrições.** As equipas inscrevem-se pela ligação pública do campeonato. Usa `ver-campeonato` para ver as inscrições pendentes e `decidir-inscricao` para aprovar ou rejeitar cada uma, depois de o utilizador confirmar.
4. **Gerar o calendário.** Com as equipas aprovadas, usa `gerar-calendario`. Se o campeonato já tiver jogos, gerar de novo apaga-os, incluindo resultados: explica isso e só envia `"confirmar": true` depois de o utilizador concordar.
5. **Mostrar o resultado.** Termina com a ligação pública do campeonato devolvida pelas ferramentas, para o utilizador partilhar.

## Boas práticas

- Usa sempre os identificadores (`id`) devolvidos por `listar-campeonatos` e `ver-campeonato`; não os inventes.
- Antes de qualquer acção que altere dados (criar, aprovar, gerar), resume o que vai acontecer e espera pela confirmação do utilizador.
- Se uma ferramenta devolver erro de validação, mostra a mensagem ao utilizador e pede o dado em falta.
