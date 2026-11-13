# Caminhos da Cidade

RPG narrativo em pixel art sobre **escolhas, empatia e sociedade**, com temas de Sociologia.
No fim de tarde, você volta a pé para casa atravessando o centro da cidade. No caminho, cinco situações pedem uma resposta, e cada uma mexe na sua barra de Empatia e no final que você vai encontrar.

Feito em HTML5 Canvas puro, num único arquivo, sem imagens nem sons externos: toda a arte é desenhada em código e toda a trilha é sintetizada com a Web Audio API.

Versão atual: **v1.0.0** · veja o [CHANGELOG](CHANGELOG.md).

---

## Como jogar

Abra `index.html` em qualquer navegador moderno (Chrome, Edge, Firefox, Safari). Funciona offline. Sem internet, as fontes do Google Fonts caem para uma fonte monoespaçada e o resto do jogo continua igual.

A música começa no primeiro clique ou toque, porque os navegadores bloqueiam som antes disso.

### Controles

| Tecla | Ação |
|---|---|
| `←` `→` ou `A` `D` | Caminhar |
| `Espaço` ou `Enter` (ou clique) | Avançar o diálogo |
| `1` `2` `3` (ou clique) | Escolher a resposta A, B ou C |
| `M` | Ligar ou desligar o som |

No celular aparecem botões de toque nos cantos da tela.

### A jornada

| # | Lugar | Situação | Tema sociológico |
|---|---|---|---|
| 1 | Rua do Comércio | Fiscais recolhem as mercadorias de Seu Raimundo, vendedor ambulante | Desigualdade social e trabalho informal |
| 2 | Avenida Central | Dona Cida, de bengala, não consegue atravessar no tempo do sinal | Inclusão social e acessibilidade |
| 3 | Rua das Lojas | Um segurança acusa Caio, adolescente negro, na porta da Loja Estilo | Racismo estrutural e perfilamento racial |
| 4 | Largo Boa Vista | Seu Hélio ameaça Caramelo, um cachorro de rua | Vulnerabilidade animal e maus-tratos |
| 5 | Rua do Banco | Jorge, em situação de rua, pede algo para comer | Exclusão e invisibilidade social |

Depois de cada resposta aparece uma **Reflexão Sociológica**. Na última rua, a caminho de casa, acontece o atropelamento, e a pontuação decide o final.

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
index.html        o jogo, v1.0.0 (arquivo único)
CHANGELOG.md      histórico de versões
```

### Detalhes técnicos

- Resolução interna de 225 px de altura e largura entre 300 e 520 px (acompanha a proporção da tela), ampliada sem suavização (`image-rendering: pixelated`).
- A cidade tem 3.640 px de largura, desenhada uma vez em camadas de dia e de noite; o céu e o horizonte se movem em paralaxe.
- Iluminação por mapa de escuridão, com luz de janelas, postes, letreiros e faróis.

---

## Créditos

- Ideia, roteiro e direção: equipe do projeto **Jogo Sociologia**.
- Código e pixel art gerados com Claude (Anthropic), a partir das especificações da equipe.
- Referências sociológicas citadas no jogo: Anthony Giddens, Zygmunt Bauman, Pierre Bourdieu, Silvio Almeida, Fernando Braga da Costa; dados do IBGE; Lei Brasileira de Inclusão (13.146/2015), Lei de Crimes Ambientais (9.605/98) e Lei 14.064/2020.

## Licença

Todos os direitos reservados até a equipe decidir a licença da versão pública.
