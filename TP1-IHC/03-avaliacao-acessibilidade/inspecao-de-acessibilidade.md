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


### 1. Telas que foram avaliadas

1. **Página Inicial (Home)**
2. **Página de Resultados de Busca / Listagem de Produtos (PLP - Product Listing Page)**
3. **Página de Detalhes do Produto (PDP - Product Detail Page)**
4. **Fluxo de Carrinho de Compras e Checkout (Cart & Checkout)**
## Processo utilizado

O processo utilizado baseou-se na detecção, coleção e discriminação de não-conformidades nas interfaces selecionadas.

* **Detecção:** Realizada por meio de inspeção manual da interface interagindo com leitor de tela (NVDA/VoiceOver) e navegação exclusiva por teclado, rastreando os 4 princípios fundamentais (Perceptível, Operável, Compreensível e Robusto).
* **Coleção:** Agrupamento das falhas sistêmicas que se repetem em componentes compartilhados, como modais promocionais e carrosséis de componentes de entrada (inputs).
* **Discriminação:** Classificação dos problemas com base no impacto real na experiência do usuário durante o fluxo de compra, priorizando gargalos que impedem a finalização de tarefas primárias (ex: adicionar ao carrinho e pagar).

## Resultados da inspeção

### Síntese dos problemas encontrados
| Problema | Critério WCAG | Tela/Página | Frequência |
| --- | --- | --- | --- |
| Vídeo sem audiodescrição | 1.2.5 - Audiodescrição (pré-gravada) | Página de produto | ∞ |
| Não há linguagem de sinais em áudios pré-gravados | 1.2.6 - Linguagem de sinal (pré-gravada) | Página de produto | ∞ |
| Falta de clareza das informações relacionadas as taxas de importação de produtos estrangeiros | 1.4.3 - Contraste (mínimo) | Tela de produtos importados | ∞ |
| Falta de contraste no texto "combo de ofertas" abaixo do card dos produtos| 1.4.3 - Contraste (mínimo) | Tela principal | ∞ |
| Links que se disfarçam de itens e levam para outra tela | 3.2.5 Mudança mediante a solicitação | Tela inicial | ∞ |
<div align="center">Tabela 1 - Tabela de síntese de problemas encontrados</div>

Nota-se ausência de recursos essenciais para conteúdos multimídia como audiodescrição e linguagem de sinais na página de produto (critérios 1.2.5 e 1.2.6), problemas graves de contraste mínimo que afetam a legibilidade de textos secundários e informações de importação (critério 1.4.3), além de links enganosos que redirecionam o usuário de forma inesperada na tela inicial (critério 3.2.5).

### Critérios WCAG violados
| Princípio | Diretriz | Critério violado | Nível | Tela/Página | Frequência |
| --- | --- | --- | --- | --- | --- |
| Perceptível | 1.2 Mídias com base em tempo | 1.2.5 Audiodescrição (pré-gravada) | AA | Página de produto | ∞ |
| Perceptível | 1.2 Mídias com base em tempo | 1.2.6 Linguagem de sinal (pré-gravada) | AAA | Página de produto | ∞ |
| Perceptível | 1.4 Discernível | 1.4.3 Contraste mínimo | AA | Tela de produtos importados | ∞ |
| Perceptível | 1.4 Discernível | 1.4.3 Contraste mínimo | AA | Página inicial | ∞ |
| Compreensível | 3.2 Previsível | 3.2.5 Mudança mediante solicitação | AAA | Página inicial | ∞ |
<div align="center"> Tabela 2 - Tabela de critérios WCAG violados</div>

Com os resultados analisados no princípio do **Perceptível**, foram identificadas falhas relacionadas a conteúdos multimídia e à legibilidade visual. Na página de produto, a ausência de audiodescrição (critério 1.2.5) e de interpretação em linguagem de sinais em vídeos pré-gravados (critério 1.2.6) impede o acesso pleno por parte de pessoas com deficiência sensorial (visual e auditiva). Ademais, problemas de contraste mínimo (critério 1.4.3) foram detectados tanto na tela de produtos importados quanto na página inicial, dificultando a distinção de elementos textuais e informativos essenciais.

No princípio do **Compreensível**, se nota uma infração ao critério de previsibilidade com a ocorrência de mudanças de contexto não solicitadas (critério 3.2.5) na página inicial, o que pode causar desorientação e problemas de navegação.

## Considerações sobre os resultados

A análise dos resultados obtidos na inspeção de acessibilidade indica que a plataforma apresenta algumas barreirasde acesso para certos perfis de usuários, violando critérios das diretrizes WCAG 2.2. 

A ausência de certos recursos de acessibilidade para conteúdos em vídeo — como audiodescrição e interpretação em LIBRAS — isola usuários com deficiências sensoriais de informações chave na decisão de compra. Além disso, os problemas recorrentes de contraste afetam a legibilidade de dados fundamentais (como taxas e ofertas), enquanto os redirecionamentos inesperados por links camuflados prejudicam a previsibilidade do sistema, criando um fluxo de navegação truncado e pouco inclusivo.
