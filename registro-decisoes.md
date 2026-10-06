# Registro das decisões — Seu guia sob pressão

## 1. Menu principal

**AJUSTE:** Menu do cabeçalho

**TIPO:** Intrínseco

**POR QUÊ:** O menu agora usa `flex-wrap`, permitindo que os links ocupem mais de uma linha quando o espaço diminuir, em vez de aumentar a largura da página.

**LARGURA EM QUE FALHAVA:** Em larguras pequenas, aproximadamente abaixo de 600–700px, o menu podia contribuir para o conteúdo ultrapassar a tela.

**SOLUÇÃO:** `display: flex`, `flex-wrap: wrap` e espaçamentos menores no mobile.

**O QUE FICOU DE FORA:** Não foram feitas mudanças profundas de tipografia.

**MOTIVO:** Tipografia não faz parte do foco principal desta etapa.

---

## 2. Grid dos cards

**AJUSTE:** Organização dos cards de locais

**TIPO:** Intrínseco

**POR QUÊ:** A quantidade de colunas deve acompanhar o espaço disponível, sem criar uma versão específica para cada aparelho.

**LARGURA EM QUE FALHAVA:** O problema aparecia conforme a janela diminuía e os cards precisavam competir por espaço.

**SOLUÇÃO:** `repeat(auto-fit, minmax(min(100%, 220px), 1fr))`.

**O QUE FICOU DE FORA:** Não foram alterados os textos dos locais.

**MOTIVO:** O conteúdo original deveria ser preservado.

---

## 3. Largura dos containers

**AJUSTE:** Limite de largura do conteúdo

**TIPO:** Intrínseco

**POR QUÊ:** Em telas grandes, o conteúdo não precisa ocupar toda a largura disponível.

**LARGURA EM QUE FALHAVA:** Principalmente em telas largas, nas quais o conteúdo poderia ficar muito espalhado.

**SOLUÇÃO:** Uso de `width: min(100% - 2rem, 1120px)` e `margin-inline: auto`.

**O QUE FICOU DE FORA:** Não foi criado um layout separado para 1280px.

**MOTIVO:** A proposta é que o layout se adapte também nas larguras intermediárias.

---

## 4. Mudança de composição entre mobile e desktop

**AJUSTE:** Sidebar e estrutura geral da página

**TIPO:** Deliberado

**POR QUÊ:** Em telas pequenas, a lateral ao lado do conteúdo ocupava espaço demais. Em telas maiores, a divisão em duas colunas aproveita melhor a área disponível.

**LARGURA EM QUE FALHAVA:** Aproximadamente abaixo de 760px, a composição em duas colunas ficava apertada.

**SOLUÇÃO:** Mobile começa com uma coluna. A partir de `@media (min-width: 760px)`, a página passa para duas colunas.

**O QUE FICOU DE FORA:** Não foram criados breakpoints para modelos específicos de celular.

**MOTIVO:** O breakpoint foi usado somente para uma mudança real de composição.

---

## 5. Página de detalhe

**AJUSTE:** Criação da página `detalhe.html`

**TIPO:** Deliberado

**POR QUÊ:** O projeto enviado possuía apenas a home, mas a atividade exige o fluxo card → detalhe → home.

**LARGURA EM QUE FALHAVA:** A página de detalhe ainda não existia, portanto não havia fluxo para testar.

**SOLUÇÃO:** Criação de uma página simples para o Parque Centenário, reutilizando as informações que já estavam disponíveis no projeto.

**O QUE FICOU DE FORA:** Não foram inventados endereço, coordenadas, avaliação ou informações adicionais.

**MOTIVO:** A atividade determina que informações ausentes não sejam inventadas.

---

## 6. Link do card

**AJUSTE:** Card do Parque Centenário

**TIPO:** Deliberado

**POR QUÊ:** É o local que passou a ter uma página própria.

**LARGURA EM QUE FALHAVA:** Não era um problema de largura, mas uma pendência de navegação.

**SOLUÇÃO:** O conteúdo do card foi envolvido por `<a href="detalhe.html">`, tornando o card inteiro uma área clicável.

**O QUE FICOU DE FORA:** Os outros cards não receberam links.

**MOTIVO:** Eles não possuem páginas próprias no projeto enviado.

---

## 7. Navegação da página de detalhe

**AJUSTE:** Links entre home e detalhe

**TIPO:** Deliberado

**POR QUÊ:** O usuário precisa conseguir voltar para a home e também acessar as seções da home.

**LARGURA EM QUE FALHAVA:** Não era um problema de largura; era uma pendência de navegação.

**SOLUÇÃO:** O menu da página de detalhe usa `index.html`, `index.html#locais`, `index.html#agenda` e `index.html#contato`. A página também possui âncoras internas.

**O QUE FICOU DE FORA:** Não foi usado JavaScript.

**MOTIVO:** Links HTML são suficientes para essa navegação.

---

## 8. Google Maps

**AJUSTE:** Verificação de localização

**TIPO:** Deliberado

**POR QUÊ:** A atividade pede Google Maps quando existe endereço ou coordenada disponível.

**LARGURA EM QUE FALHAVA:** Não se aplica.

**SOLUÇÃO:** O projeto enviado não contém endereço nem coordenadas do Parque Centenário. Portanto, nenhum link de mapa foi inventado.

**O QUE FICOU DE FORA:** Link do Google Maps.

**MOTIVO:** É necessário receber o endereço ou coordenadas para criar o link corretamente.

---

## 9. Tipografia e mídia

**AJUSTE:** Escopo da atividade

**TIPO:** Deliberado

**POR QUÊ:** A atividade determina foco em layout, responsividade e navegação.

**LARGURA EM QUE FALHAVA:** Não se aplica.

**SOLUÇÃO:** Foram mantidas as escolhas visuais simples do projeto e não foram adicionadas imagens ou bibliotecas externas.

**O QUE FICOU DE FORA:** Alterações profundas de tipografia e mídia.

**MOTIVO:** Esses itens ficam para a segunda parte da aula.
