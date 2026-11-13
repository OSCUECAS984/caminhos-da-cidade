# Histórico de versões

## v2.1.0 · 13/11/2026 · versão mais recente

Versão mais recente, a mesma do `index.html` da raiz. Todas as versões jogáveis estão em [versoes/](versoes/).

- **Túnel nas ruas transversais:** as duas ruas que cruzam a avenida agora descem em perspectiva e entram num túnel sob o morro, com portal de concreto, moldura listrada de amarelo e preto, placa "TÚNEL", lâmpadas no teto, muros laterais e luz da saída lá no fundo.
- **Atropelamento refeito, em quatro tempos:**
  1. Os faróis acendem no fundo do túnel e o carro (vermelho, visto de frente) se aproxima; dentro do túnel ele é quase só silhueta.
  2. Buzina, o protagonista se vira assustado, e o carro sai do túnel acelerando. A freada chega tarde, com fumaça nos pneus.
  3. Impacto: clarão curto, cacos de vidro que caem e ficam no asfalto, e o corpo é arremessado girando.
  4. O corpo quica, rola e para. Se Caramelo estiver seguindo o protagonista, ele corre até ele.

  Na v2.0.0 o acidente era um carro crescendo na tela e um clarão branco.
- **Pedestres mais vivos:** entram pelas bordas da tela ou saem pelas portas de lojas e prédios, e terminam atravessando a tela ou entrando em outra porta, sempre com transição suave. Perto de uma cena, somem aos poucos em vez de piscar. Na última rua ninguém atravessa: quem chega dá meia-volta.
- A van da fiscalização fica rente ao meio-fio, e os carros da faixa passam na frente dela.
- Carrinho de pipoca maior e com letreiro, banca com cavalete e primeira página do jornal, e árvores da praça em novas posições.

## v2.0.0 · 13/11/2026

Nova build. A história, os diálogos e os três finais continuam os mesmos da v1; mudam a arte, o som, a interface e a exploração.

- **Arte refeita:** sprites desenhados num buffer com contorno seletivo (o contorno puxa um tom escuro da cor vizinha), sombras que tendem ao roxo e luzes ao amarelo, e pontilhado (dithering) em sombras e no céu. Fonte bitmap própria, com acentos, para letreiros e placas.
- **Personagens e cidade com mais detalhe:** roupas e poses novas (Caio de moletom com capuz, Jorge sentado no chão), gato, pombos, ônibus e moto no trânsito. Fachadas texturizadas, pichações, poças, TVs acesas nas janelas e ipês amarelos e roxos nas calçadas.
- **Interface em pixel art:** molduras desenhadas, caixa de diálogo com **retrato** de quem fala e **balões de emoção** (!, coração, raiva, suor, nota) quando o humor de um personagem muda.
- **Olhares (exploração opcional):** 8 pontos **?** pela cidade. Com `E`, `↑` ou `W` (ou o botão OLHAR no celular), o protagonista para e observa:
  - a manchete da banca sobre informalidade;
  - o piso tátil que termina num poste (norma ABNT NBR 9050);
  - o preço da passagem no ponto de ônibus (*direito à cidade*, Henri Lefebvre);
  - o tênis do Caio na vitrine (*sociedade de consumo*, Bauman);
  - **Wesley**, entregador de aplicativo, personagem novo (*uberização do trabalho*, Ricardo Antunes);
  - o quadro de preços do mercado (fome no Brasil, Rede PENSSAN);
  - os pinos sob a marquise do banco (*arquitetura hostil*, Lei 14.489/2022, Lei Padre Júlio Lancellotti);
  - um gato preto no muro.

  O HUD conta **OLHARES x/8**. Os olhares não mudam a pontuação.
- **Respostas embaralhadas** a cada situação e numeradas 1, 2 e 3 (na v1 a resposta boa era sempre a primeira).
- **Pausa** com `Esc`, `P` ou o botão II: continuar, ligar ou desligar o som e escolher a velocidade do texto (Normal ou Veloz, guardada no navegador).
- **Trilha nova:** sequenciador com levada de bossa nova na cidade, tema noturno na segunda metade do caminho e temas próprios para céu, purgatório e inferno. Ambiência de zumbido urbano e chuva. Com a noite chega a chuva, e os pedestres abrem guarda-chuva.
- Caramelo ganha uma bandana quando é adotado.
- **Tela final** com estatísticas (olhares atentos e finais descobertos). O menu mostra os selos dos finais que já foram vistos (Céu, Purgatório, Inferno), guardados no navegador.
- No celular em pé, o menu pede para girar a tela para a horizontal. A imagem usa escala inteira quando isso quase não perde espaço.

## v1.1.0 · 13/11/2026

- **Sem mudanças no jogo.** O arquivo entregue como v1.1.0 é idêntico, byte a byte, ao da v1.0.0 (mesmo SHA-256: `c8984e26…2f1f`). A versão foi registrada separadamente para manter a numeração da equipe. Se havia alterações previstas para a v1.1.0, elas não estão neste arquivo.

## v1.0.0 · 13/11/2026 · primeira versão

Primeira versão do jogo enviada pela equipe.

- **RPG narrativo em pixel art:** fim de tarde, o protagonista se levanta do banco da Praça da Liberdade e volta a pé para casa, atravessando o centro da cidade. O caminho passa pela Rua do Comércio, Avenida Central, Rua das Lojas, Largo Boa Vista, Rua do Banco e Caminho de Casa, com o nome de cada trecho anunciado na tela.
- **Cinco situações**, cada uma com três respostas faladas pelo protagonista e uma **Reflexão Sociológica** no fim:
  1. Trabalho informal (desigualdade social): fiscais recolhem as mercadorias de Seu Raimundo, vendedor ambulante.
  2. Acessibilidade (inclusão social): Dona Cida, de bengala, não consegue atravessar no tempo do sinal.
  3. Perfilamento (racismo estrutural): um segurança acusa Caio, adolescente negro, na porta da Loja Estilo.
  4. Crueldade (vulnerabilidade animal): Seu Hélio ameaça Caramelo, um cachorro de rua, com a vassoura.
  5. Invisibilidade social (exclusão social): Jorge, em situação de rua, pede comida sob a marquise do banco.
- **Barra de Empatia** de −50 a +50 no HUD. Cada resposta vale +10 (agir), −2 (se omitir) ou −10 (reproduzir o preconceito). As respostas aparecem sempre na mesma ordem (A, B, C).
- **Cada escolha muda a cena:** a van vai embora com ou sem as mercadorias, Dona Cida atravessa de braço dado, o segurança solta Caio, Caramelo passa a seguir o protagonista, Jorge ganha um lanche e diz o próprio nome.
- **O dia vira noite** conforme o caminho avança: pôr do sol, luzes das janelas, letreiros em neon, postes e faróis.
- **Atropelamento** na última rua e **três finais** conforme a pontuação:
  - **Céu** (+11 ou mais): *Agência Social* (Anthony Giddens). O anjo devolve a vida ao protagonista.
  - **Purgatório** (−10 a +10): *Modernidade Líquida e Invisibilidade Social* (Zygmunt Bauman). Anjo e demônio discutem; segunda chance.
  - **Inferno** (−11 ou menos): *Violência Simbólica e Reprodução do Preconceito* (Pierre Bourdieu). O anjo aparece e concede uma segunda chance.
- **Tela final** com explicação sociológica, consequência, resumo das cinco escolhas e botão para recomeçar no banco da praça.
- Arte toda desenhada em código (HTML5 Canvas) e trilha e efeitos sintetizados (Web Audio), com tema da cidade, do céu, do purgatório e do inferno.
- Controles de teclado e botões de toque no celular.
