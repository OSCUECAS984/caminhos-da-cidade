# Caminhos da Cidade

RPG narrativo em pixel art sobre **escolhas, empatia e sociedade**, com temas de Sociologia.
No fim de tarde, você volta a pé para casa atravessando o centro da cidade. No caminho, cinco situações pedem uma resposta, e cada uma mexe na sua barra de Empatia e no final que você vai encontrar.

Feito em HTML5 Canvas puro, num único arquivo, sem imagens nem sons externos: toda a arte é desenhada em código e toda a trilha é sintetizada com a Web Audio API.

> **Versão final de lançamento: v2.1.0.** O `index.html` da raiz é o jogo lançado. As versões anteriores continuam disponíveis em [`versoes/`](versoes/).

**▶ Jogue no navegador:** https://oscuecas984.github.io/caminhos-da-cidade/ (GitHub Pages)  
Versões anteriores online: `https://oscuecas984.github.io/caminhos-da-cidade/versoes/vX.Y.Z/`

Versão final: **v2.1.0** (lançamento) · veja o [CHANGELOG](CHANGELOG.md) e as [versões anteriores](versoes/).

---

## Como jogar

Abra `index.html` em qualquer navegador moderno (Chrome, Edge, Firefox, Safari). Funciona offline. Sem internet, as fontes do Google Fonts caem para uma fonte monoespaçada e o resto do jogo continua igual.

A música começa no primeiro clique ou toque, porque os navegadores bloqueiam som antes disso.

### Controles

| Tecla | Ação |
|---|---|
| `←` `→` ou `A` `D` | Caminhar |
| `E`, `↑` ou `W` | Olhar um ponto **?** de perto |
| `Espaço` ou `Enter` (ou clique) | Avançar o diálogo |
| `1` `2` `3` (ou clique) | Escolher a resposta |
| `Esc` ou `P` | Pausa (som e velocidade do texto) |
| `M` | Ligar ou desligar o som |

No celular aparecem botões de toque (◀ ▶ e OLHAR). O jogo fica melhor com o celular na horizontal.

### A jornada

| # | Lugar | Situação | Tema sociológico |
|---|---|---|---|
| 1 | Rua do Comércio | Fiscais recolhem as mercadorias de Seu Raimundo, vendedor ambulante | Desigualdade social e trabalho informal |
| 2 | Avenida Central | Dona Cida, de bengala, não consegue atravessar no tempo do sinal | Inclusão social e acessibilidade |
| 3 | Rua das Lojas | Um segurança acusa Caio, adolescente negro, na porta da Loja Estilo | Racismo estrutural e perfilamento racial |
| 4 | Largo Boa Vista | Seu Hélio ameaça Caramelo, um cachorro de rua | Vulnerabilidade animal e maus-tratos |
| 5 | Rua do Banco | Jorge, em situação de rua, pede algo para comer | Exclusão e invisibilidade social |

Depois de cada resposta aparece uma **Reflexão Sociológica**. Na última rua, a caminho de casa, acontece o atropelamento, e a pontuação decide o final.

Pelo caminho há também 8 pontos **?** opcionais (os *olhares*): a banca de jornal, o piso tátil, o ponto de ônibus, a vitrine, o entregador Wesley, o quadro do mercado, a marquise do banco e um gato no muro. Eles não mudam a pontuação, mas acrescentam conceitos como direito à cidade, uberização e arquitetura hostil.

### Pontuação e finais

Cada situação tem três respostas: **agir** (+10 de Empatia), **se omitir** (−2) ou **reproduzir o preconceito** (−10). A barra vai de −50 a +50.

| Final | Pontuação | Conceito |
|---|---|---|
| Céu | +11 ou mais | Agência social (Anthony Giddens) |
| Purgatório | de −10 a +10 | Modernidade líquida e invisibilidade social (Zygmunt Bauman) |
| Inferno | −11 ou menos | Violência simbólica e reprodução do preconceito (Pierre Bourdieu) |

A tela final traz a explicação sociológica, a consequência e o resumo das suas escolhas. Depois é possível recomeçar do banco da praça.

---

## Estrutura do repositório

```
index.html        o jogo lançado, v2.1.0 (arquivo único)
versoes/          cada versão publicada, jogável: versoes/vX.Y.Z/index.html
docs/             documento de game design
CHANGELOG.md      histórico de versões
```

### Detalhes técnicos

- Resolução interna de 225 px de altura e largura entre 300 e 520 px (acompanha a proporção da tela), ampliada sem suavização (`image-rendering: pixelated`).
- A cidade tem 3.640 px de largura, desenhada uma vez em camadas de dia e de noite; o céu e o horizonte se movem em paralaxe.
- Iluminação por mapa de escuridão, com luz de janelas, postes, letreiros e faróis.
- Preferências (velocidade do texto) e finais descobertos ficam salvos no navegador (`localStorage`).

---

## Créditos

- Ideia, roteiro e direção: equipe do projeto **Jogo Sociologia**.
- Código e pixel art gerados com Claude (Anthropic), a partir das especificações da equipe.
- Referências sociológicas citadas no jogo: Anthony Giddens, Zygmunt Bauman, Pierre Bourdieu, Silvio Almeida, Fernando Braga da Costa, Henri Lefebvre, Ricardo Antunes; dados do IBGE e da Rede PENSSAN; Lei Brasileira de Inclusão (13.146/2015), Lei de Crimes Ambientais (9.605/98) e Lei 14.064/2020, Lei 14.489/2022 e ABNT NBR 9050.

## Licença

Todos os direitos reservados até a equipe decidir a licença da versão pública.
