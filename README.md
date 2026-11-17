# Peladeiros para o Claude

Plugin do [Peladeiros](https://peladeiros.ao), a plataforma angolana para organizar campeonatos de futebol de bairro: futebol 11, futebol 7, futebol 5, futsal e futebol de praia. Com este plugin, o Claude ajuda organizadores a criar campeonatos, aprovar equipas, gerar o calendário, lançar resultados e partilhar a classificação no WhatsApp, em português de Angola.

Criado por Amarildo Miguel, em co-autoria com a IAMI.

## O que inclui

- **Conector MCP** `peladeiros`, ligado a `https://peladeiros.ao/mcp`.
- **Skills:**
  - `organizar-campeonato`: da escolha da variante e do formato até ao calendário gerado.
  - `lancar-resultados`: lançar e corrigir resultados e ver a classificação.
  - `partilhar-no-whatsapp`: preparar mensagens com a tabela, os jogos e os marcadores.

## Ferramentas do servidor

| Ferramenta | O que faz | Altera dados? |
|---|---|---|
| `ver-minha-conta` | A tua conta: id do jogador, equipas e plano | Não |
| `listar-modalidades-e-formatos` | Variantes de futebol e formatos de competição | Não |
| `listar-campeonatos` | Campeonatos que geres | Não |
| `ver-campeonato` | Inscrições, classificação, jogos e resultados | Não |
| `ver-planos` | Plano actual e limites | Não |
| `ver-perfil-jogador` | Perfil de um jogador (sem id, o teu) | Não |
| `texto-partilha` | Texto e ligação wa.me para o WhatsApp | Não |
| `criar-campeonato` | Cria um campeonato em rascunho | Sim |
| `decidir-inscricao` | Aprova ou rejeita a inscrição de uma equipa | Sim |
| `gerar-calendario` | Gera os jogos do campeonato | Sim |
| `lancar-resultado` | Regista o resultado, o estado, a data ou o campo de um jogo | Sim |
| `criar-link-equipa` | Cria um link de convite para uma equipa | Sim |
| `configurar-cartao-jogador` | Cor e frase do cartão de jogador | Sim |
| `actualizar-modalidades-jogador` | Variantes de futebol do teu perfil | Sim |

## Instalação e login

1. Instala o plugin no Claude.
2. Na primeira utilização, o Claude abre o login do Peladeiros (OAuth 2.1). Entra com a tua conta e autoriza o acesso.
3. Podes revogar o acesso a qualquer momento em https://peladeiros.ao/agentes-ia.

Precisas de uma conta no Peladeiros. Organizar é grátis até 100 jogadores por campeonato.

## Dados e privacidade

- O plugin não corre código no teu computador: só liga o Claude ao servidor `https://peladeiros.ao/mcp`.
- O Claude envia a esse servidor apenas os dados de cada pedido (por exemplo, o nome do campeonato ou o resultado de um jogo), sempre em teu nome e só sobre campeonatos e perfis a que tens acesso.
- O servidor não lê as tuas conversas, a memória do Claude nem os teus ficheiros.
- Política de privacidade: https://peladeiros.ao/privacidade

## Suporte

- Documentação: https://peladeiros.ao/agentes-ia
- Contacto: amarildomgl@gmail.com

## Licença

MIT. Ver [LICENSE](LICENSE).
