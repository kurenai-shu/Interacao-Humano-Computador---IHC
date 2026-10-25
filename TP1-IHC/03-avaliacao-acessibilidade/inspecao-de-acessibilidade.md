# Avaliação de Acessibilidade
## Método utilizado
<p style="text-align: justify;">
  A Inspeção de Acessibilidade é uma técnica da área de Interação Humano-Computador e Engenharia de Acessibilidade que serve para avaliar a qualidade e a conformidade de uma interface digital em relação às necessidades de pessoas com deficiência. Na prática, o processo busca entender se o conteúdo, as estruturas semânticas e as funcionalidades do sistema respeitam as diretrizes internacionais das WCAG 2.2, permitindo que usuários que dependem de tecnologias assistivas (como leitores de tela) ou métodos alternativos de navegação (como o uso exclusivo do teclado) consigam interagir com a aplicação sem barreiras. Durante a inspeção sistemática, o método foca no mapeamento de barreiras de acessibilidade — falhas ou descumprimentos dos critérios da WCAG 2.2 identificados por avaliações manuais e ferramentas automatizadas.
</p>
<p style="text-align: justify;"> 
 Essas barreiras ocorrem devido a problemas como falta de descrições em imagens, contraste inadequado, bloqueios de navegação via teclado, ausência de foco visível ou elementos sem identificação correta. O avaliador cataloga esses achados conforme a diretriz violada e a gravidade, indicando exatamente o que deve ser corrigido na interface.
</p>

## Escopo da avaliação
Foram selecionadas as seguintes telas para inspeção:
Com base no status de acesso ao site e conhecendo a estrutura típica de grandes plataformas de comércio eletrônico (como o **AliExpress**), podemos mapear as principais **telas/páginas** e **funcionalidades** que devem ser priorizadas em uma inspeção ou auditoria de acessibilidade digital com base no modelo **WCAG 2.2** (Web Content Accessibility Guidelines).

---

### 1. Principais Telas para Inspeção no AliExpress

1. **Página Inicial (Home)**
* **O que é:** A porta de entrada do site, rica em banners dinâmicos, carrosséis de produtos, seções de ofertas relâmpago e categorias.
* **Pontos WCAG críticos:** Navegação por teclado nos carrosséis, contraste de cores em textos sobrepostos a imagens/banners promocionais, tempo limite (timeout) em ofertas relâmpago e textos alternativos (`alt`) em imagens de produtos e banners.


2. **Página de Resultados de Busca / Listagem de Produtos (PLP - Product Listing Page)**
* **O que é:** A tela onde o usuário visualiza uma grade de produtos após realizar uma busca ou filtrar por categorias (ex: preço, frete grátis, avaliação).
* **Pontos WCAG críticos:** Sinais visuais e programáticos claros de filtros ativos, foco visível ao navegar pelos produtos, ordem de leitura lógica do leitor de tela (nome do produto, preço, avaliação) e redimensionamento de texto sem perda de funcionalidade (Critério WCAG 2.2 - *Reflow*).


3. **Página de Detalhes do Produto (PDP - Product Detail Page)**
* **O que é:** A página central de compra onde o usuário escolhe variações (tamanho, cor, quantidade), visualiza galeria de imagens/vídeos e lê descrições e avaliações.
* **Pontos WCAG críticos:** Interação acessível com seletores de variação (botões de rádio ou menus suspensos), legendas e descrições em vídeos de produtos, zoom em imagens e foco que não fica preso em modais ou galerias de fotos.


4. **Fluxo de Carrinho de Compras e Checkout (Cart & Checkout)**
* **O que é:** Onde o usuário revisa os itens escolhidos, insere endereços de entrega e realiza o pagamento.
* **Pontos WCAG críticos:** Formulários acessíveis (rótulos claros, identificação de erros em tempo real e sugestões de correção conforme os novos critérios da WCAG 2.2 sobre *Entrada de Dados Errada*), gerenciamento de foco rigoroso e navegação sem barreiras em etapas complexas de pagamento.


5. **Central do Cliente / Minha Conta e Login**
* **O que é:** Área logada para rastreio de pedidos, gestão de endereços, cupons e dados pessoais.
* **Pontos WCAG críticos:** Autenticação sem barreiras cognitivas excessivas (como CAPTCHAs inacessíveis — a WCAG 2.2 exige alternativas acessíveis para testes cognitivos), mensagens de status anunciadas por leitores de tela (`aria-live`) ao atualizar o status de pedidos.



---

### 2. Principais Funcionalidades sob a Ótica da WCAG 2.2

Durante a inspeção, além das telas, as seguintes funcionalidades interativas globais do AliExpress exigem testes específicos:

* **Menu de Navegação Principal e Categorias (Mega Menu):**
* *Verificação:* O menu abre e fecha corretamente via teclado (teclas `Tab`, `Escape`, setas direcionais)? Os submenus mantêm o foco de forma previsível?


* **Busca Preditiva / Sugestões de Pesquisa:**
* *Verificação:* Quando o usuário digita na barra de pesquisa, as sugestões que aparecem dinamicamente são anunciadas para leitores de tela e podem ser selecionadas por teclado? (Critério WCAG 2.2 de *Aparência do Foco* e *Componentes de Acessibilidade Móvel*).


* **Modais, Pop-ups e Anúncios Promocionais:**
* *Verificação:* O foco do teclado é preso (trapped) dentro do modal enquanto ele está aberto? Existe um botão "Fechar" claramente acessível e focável? O pressionamento da tecla `Esc` fecha o pop-up?


* **Gestos de Toque e Dispositivos Móveis (Se testado na versão mobile/responsiva):**
* *Verificação (Novidades do WCAG 2.2):* Elementos interativos de toque (botões de adicionar ao carrinho, favoritar) possuem tamanho mínimo de alvo de clique de pelo menos 24x24 pixels? Funcionalidades complexas baseadas em gestos de arrastar (*Dragging Movements*) possuem alternativas acessíveis de clique simples?



---

Se você estiver avaliando uma tela ou fluxo específico do AliExpress (como o processo de checkout ou a busca), posso detalhar os critérios exatos da WCAG 2.2 (como os níveis A, AA e os novos critérios adicionados na versão 2.2) aplicáveis a esse cenário!
## Processo utilizado
[Explicar o processo utilizado: Detecção, coleção e discriminação]
## Resultados da inspeção
| Problema | Critério WCAG | Tela/Página | Frequência |
| --- | --- | --- | --- |
| Vídeo sem audiodescrição | 1.2.5 - Audiodescrição (pré-gravada) | Página de produto | ∞ |
| Não há linguagem de sinais em áudios pré-gravados | 1.2.6 - Linguagem de sinal (pré-gravada) | Página de produto | ∞ |
| Falta de clareza das informações relacionadas as taxas de importação de produtos estrangeiros | 1.4.3 - Contraste (mínimo) | Tela de produtos importados | ∞ |
| Falta de contraste no texto "combo de ofertas" abaixo do card dos produtos| 1.4.3 - Contraste (mínimo) | Tela principal | ∞ |
| Links que se disfarçam de itens e levam para outra tela | 3.2.5 Mudança mediante a solicitação | Tela inicial | ∞ |

### Síntese dos problemas encontrados
Explicar o que a tabela apresenta e discutir os resultados observados.

### Critérios WCAG violados
Explicar o que a tabela apresenta e discutir os resultados observados.

## Considerações sobre os resultados
Apresentar uma breve discussão sobre os principais resultados da avaliação
