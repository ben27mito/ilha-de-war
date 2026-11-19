# Ilhas de Papel V7

Site multiplayer por turnos (Node.js + WebSocket), para publicar no Render.

## Novidades
- Ilhas com contornos orgânicos, mapa arrastável e zoom.
- Menu de ações simplificado, com atalhos para minerar, pesquisar, recrutar, fazenda, fábrica, fabricar e bombardear.
- Escolha manual dos números 10, 20, 30, 40, 50, 60.
- Mineração: 1 minério por ilha possuída quando o dado acerta.
- Pesquisas simultâneas: até uma pesquisa por ilha possuída, cada pesquisa lança o próprio dado com os mesmos números escolhidos.
- Ponte fabricável por 2 minérios após pesquisa, entre ilhas a até 225 unidades; permite colonização/ataque terrestre.
- Navios pequeno, médio e grande (2, 4, 6 minérios) com poder de 1000, 2000 e 3000, respectivamente, usado como bônus de combate (limite de 3000 por ataque).
- Consumo de alimento a cada rodada e produção de fazendas.

## Publicar no Render
No GitHub, atualize os arquivos de dentro da pasta `ilhas-multiplayer`, mantendo `package.json` junto de `server.js`. No Render: Root Directory = `ilhas-multiplayer`; Build = `npm install`; Start = `npm start`.

## Limitações desta versão
- Combate e soldados ainda são contabilizados por país, não por ilha.
- O sistema de navios é uma simplificação: o poder do navio soma ao ataque, mas a vida individual do casco ainda não é contabilizada.
- Pontes conectam apenas ilhas próximas, e o acesso pode depender do controle de uma das extremidades.
- O servidor mantém as partidas em memória; reiniciar o serviço encerra as salas.
- Ainda requer teste completo com vários navegadores antes de uma partida pública.


## Versão 8
- Mapa com ilhas arredondadas, praia, vegetação e cores de países.
- Menu de ações à direita e histórico abaixo do mapa.
- Início da partida com indicação de quais jogadores ainda precisam escolher uma ilha (mínimo 2).
- Convites de aliança e aceitação no servidor (alianças informativas; não bloqueiam ataques).
- Melhorias de apresentação da tela inicial.
- Para atualizar: mantenha a pasta ilhas-multiplayer como Root Directory no Render e substitua os arquivos no GitHub.
