# Caminhos da Cidade · Documento de Game Design

Documento do jogo na **v2.1.0** (versão final de lançamento). Atualizado em 22/11/2026.

## 1. Visão geral

Caminhos da Cidade é um RPG narrativo em pixel art sobre escolhas, empatia e sociedade, com temas de Sociologia. O jogador volta a pé para casa no fim de tarde e enfrenta cinco situações de injustiça cotidiana; cada resposta muda a barra de Empatia e, no fim, o final que ele encontra.

| Item | Descrição |
| --- | --- |
| Gênero | RPG narrativo de exploração lateral com escolhas |
| Visão | 2D lateral, com a cidade rolando horizontalmente |
| Plataforma | Navegador (desktop e celular, de preferência com o celular na horizontal) |
| Tecnologia | HTML5 Canvas puro em um único arquivo, sem imagens nem sons externos |
| Duração | Uma partida curta, de uma só caminhada (cinco situações) |
| Público | Quem se interessa por Sociologia; projeto da equipe Jogo Sociologia |
| Idioma | Português (Brasil) |

### Pilares

- **Escolha com consequência visível:** cada resposta muda a cena na hora (a van vai embora, Dona Cida atravessa, Caramelo passa a seguir o protagonista).
- **Reflexão depois da ação:** toda situação termina em uma Reflexão Sociológica com o conceito por trás do que aconteceu.
- **Sem resposta óbvia:** as três respostas são embaralhadas e numeradas a cada situação, então a boa não está sempre na mesma posição.
- **Tudo em código:** arte desenhada no Canvas e trilha sintetizada, para o jogo funcionar offline e em um único arquivo.

## 2. Premissa e narrativa

No fim de tarde, o protagonista se levanta do banco da Praça da Liberdade e volta para casa pelo centro. O caminho passa por seis trechos: Rua do Comércio, Avenida Central, Rua das Lojas, Largo Boa Vista, Rua do Banco e Caminho de Casa. O nome de cada trecho aparece na tela. Enquanto o dia vira noite (pôr do sol, luzes de janelas, neon, postes e faróis), cinco pessoas ou animais precisam de uma atitude. Na última rua, a caminho de casa, acontece o atropelamento, e a pontuação decide o final.

## 3. Loop de jogo

1. Caminhar pela cidade para a direita.
2. Chegar a uma situação e ler o diálogo.
3. Escolher entre três respostas (1, 2 ou 3).
4. Ver a cena mudar e ler a Reflexão Sociológica.
5. Repetir até a quinta situação.
6. Atropelamento, tela de final (Céu, Purgatório ou Inferno) e opção de recomeçar do banco da praça.

No caminho, o jogador pode parar para olhar os pontos **?** (opcional) e ganhar contexto extra.

## 4. Controles

| Tecla | Ação |
| --- | --- |
| `←` `→` ou `A` `D` | Caminhar |
| `E`, `↑` ou `W` | Olhar um ponto **?** de perto |
| `Espaço` ou `Enter` (ou clique) | Avançar o diálogo |
| `1` `2` `3` (ou clique) | Escolher a resposta |
| `Esc` ou `P` | Pausa (som e velocidade do texto) |
| `M` | Ligar ou desligar o som |

No celular, aparecem botões de toque (◀ ▶ e OLHAR).

## 5. A jornada

| # | Lugar | Situação | Tema sociológico |
| --- | --- | --- | --- |
| 1 | Rua do Comércio | Fiscais recolhem as mercadorias de Seu Raimundo, vendedor ambulante | Desigualdade social e trabalho informal |
| 2 | Avenida Central | Dona Cida, de bengala, não consegue atravessar no tempo do sinal | Inclusão social e acessibilidade |
| 3 | Rua das Lojas | Um segurança acusa Caio, adolescente negro, na porta da Loja Estilo | Racismo estrutural e perfilamento racial |
| 4 | Largo Boa Vista | Seu Hélio ameaça Caramelo, um cachorro de rua | Vulnerabilidade animal e maus-tratos |
| 5 | Rua do Banco | Jorge, em situação de rua, pede algo para comer | Exclusão e invisibilidade social |

Consequências visíveis das respostas: a van sai com ou sem as mercadorias; Dona Cida atravessa de braço dado; o segurança solta Caio; Caramelo passa a seguir o protagonista (e ganha uma bandana quando é adotado); Jorge recebe um lanche e diz o próprio nome.

## 6. Empatia, pontuação e finais

Cada situação tem três respostas:

| Resposta | Efeito na Empatia |
| --- | --- |
| Agir | +10 |
| Se omitir | −2 |
| Reproduzir o preconceito | −10 |

A barra vai de −50 a +50 e fica sempre visível no HUD.

| Final | Pontuação | Conceito | Autor |
| --- | --- | --- | --- |
| Céu | +11 ou mais | Agência social | Anthony Giddens |
| Purgatório | −10 a +10 | Modernidade líquida e invisibilidade social | Zygmunt Bauman |
| Inferno | −11 ou menos | Violência simbólica e reprodução do preconceito | Pierre Bourdieu |

A tela final traz a explicação sociológica, a consequência, o resumo das cinco escolhas e estatísticas (olhares atentos e finais descobertos). O menu mostra selos dos finais já vistos.

## 7. Olhares (exploração opcional)

Oito pontos **?** espalhados pela cidade. Ao olhar, o protagonista para e observa. Os olhares não mudam a pontuação; o HUD conta **OLHARES x/8**.

| Ponto | Conceito |
| --- | --- |
| Banca de jornal | Manchete sobre informalidade |
| Piso tátil que termina num poste | Acessibilidade (ABNT NBR 9050) |
| Ponto de ônibus | Direito à cidade (Henri Lefebvre) |
| Vitrine com o tênis do Caio | Sociedade de consumo (Bauman) |
| Wesley, entregador de aplicativo | Uberização do trabalho (Ricardo Antunes) |
| Quadro de preços do mercado | Fome no Brasil (Rede PENSSAN) |
| Pinos sob a marquise do banco | Arquitetura hostil (Lei 14.489/2022) |
| Gato preto no muro | Nenhum conceito citado; detalhe de ambiente |

## 8. Direção de arte

- Pixel art com contorno seletivo: o contorno puxa um tom escuro da cor vizinha. Sombras tendem ao roxo e luzes ao amarelo, com pontilhado (dithering) em sombras e no céu.
- Resolução interna de 225 px de altura e largura entre 300 e 520 px, ampliada sem suavização.
- Cidade de 3.640 px de largura, desenhada uma vez em camadas de dia e de noite, com paralaxe no céu e no horizonte.
- Iluminação por mapa de escuridão, com luz de janelas, postes, letreiros e faróis.
- Detalhes vivos: pedestres que entram por bordas e portas, trânsito (ônibus, moto, carros), pombos, gato, ipês, chuva à noite com guarda-chuvas, TVs acesas nas janelas e pichações.
- Interface em pixel art: molduras desenhadas, caixa de diálogo com **retrato** de quem fala e balões de emoção (!, coração, raiva, suor, nota). Fonte bitmap própria, com acentos.
- Túnel sob o morro nas ruas transversais, com portal de concreto, moldura listrada e placa "TÚNEL".

## 9. Áudio

Todo o áudio é sintetizado com a Web Audio API.

- Sequenciador com levada de bossa nova na cidade e tema noturno na segunda metade do caminho.
- Temas próprios para Céu, Purgatório e Inferno.
- Ambiência de zumbido urbano e chuva.
- A música começa no primeiro clique ou toque, porque os navegadores bloqueiam som antes disso.

## 10. Interface e acessibilidade

- Pausa (`Esc`, `P` ou botão II): continuar, ligar ou desligar o som e escolher a velocidade do texto (Normal ou Veloz).
- No celular em pé, o menu pede para girar a tela; a imagem usa escala inteira quando isso quase não perde espaço.
- Sem internet, as fontes do Google Fonts caem para uma fonte monoespaçada.

## 11. Persistência

Ficam salvos no navegador (`localStorage`): a velocidade do texto e os finais já descobertos.

## 12. Estrutura técnica

```
index.html        o jogo, v2.1.0 (arquivo único)
versoes/          cada versão publicada, jogável: versoes/vX.Y.Z/index.html
docs/             este documento
CHANGELOG.md      histórico de versões
```

Publicado no GitHub Pages em https://oscuecas984.github.io/caminhos-da-cidade/. O repositório tem um arquivo `.nojekyll`, que faz o Pages publicar os arquivos sem processá-los.

## 13. Histórico resumido

| Versão | Data | Destaque |
| --- | --- | --- |
| v1.0.0 | 13/11/2026 | Primeira versão: 5 situações, barra de Empatia, atropelamento e 3 finais |
| v1.1.0 | 13/11/2026 | Arquivo idêntico ao da v1.0.0, byte a byte |
| v2.0.0 | 13/11/2026 | Nova arte, retratos e emoções, 8 olhares, pausa, trilha em bossa nova, chuva |
| v2.1.0 | 13/11/2026 | Túnel nas ruas transversais, atropelamento em quatro tempos, pedestres que entram por portas (versão final) |

## 14. Referências

Anthony Giddens, Zygmunt Bauman, Pierre Bourdieu, Silvio Almeida, Fernando Braga da Costa, Henri Lefebvre e Ricardo Antunes; dados do IBGE e da Rede PENSSAN; Lei Brasileira de Inclusão (13.146/2015), Lei de Crimes Ambientais (9.605/98) e Lei 14.064/2020, Lei 14.489/2022 e ABNT NBR 9050.

## 15. Pontos em aberto

- **Licença:** hoje são "todos os direitos reservados"; a equipe ainda precisa escolher a licença da versão pública.
- **v1.1.0:** o arquivo é igual ao da v1.0.0. Se havia mudanças previstas para essa versão, elas não estão no repositório.
- **Autoria:** ideia, roteiro e direção são da equipe do projeto Jogo Sociologia; código e pixel art foram gerados com Claude (Anthropic) a partir das especificações da equipe.
