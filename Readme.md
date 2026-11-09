#  Valorant - Sistema de Tier List e Lore

Este projeto contem informações simples sobre o universo do jogo **Valorant**, contendo páginas de história cronológica, listagem de agentes e mapas, além de uma aplicação funcional de **Tier List** com sistema de arrastar e soltar.



*   **`position: absolute` no Menu:** O cabeçalho foi fixado no topo da página de forma a iniciar fixo, mas subir e sumir da tela naturalmente à medida que o usuário rola a página para baixo.
*   **Compensação de Fluxo (`padding` e `margin`):** Como elementos absolutos saem do fluxo padrão do HTML, aplicou-se `padding-top: 90px` no conteúdo e `margin-top: 40px` no container para evitar que o topo do menu sobrepusesse a primeira seção de conteúdo.
*   **`flex-wrap: wrap` no Flexbox:** Aplicado tanto nas linhas de Rank quanto no banco de itens. Isso faz com que os ícones dos agentes fiquem lado a lado e pulem de linha automaticamente quando atingem a borda da tela.
*   **`object-fit: cover` com `overflow: hidden`:** Utilizado nas caixas dos agentes (`80px` por `80px`). A propriedade `cover` redimensiona e centraliza as imagens proporcionalmente, enquanto o `hidden` funciona como uma moldura, impedindo que partes da imagem vazem para fora do quadrado.
*   **HTML5 Drag and Drop Nativo:** Integração via JavaScript simples para permitir que os elementos com a propriedade `draggable="true"` mudem de container dinamicamente ao serem arrastados com o mouse.


##  Escolhas de Design

*   **Identidade Visual Valorant:** O site utiliza a cor vermelha vibrante oficial (`#bd3944`) como plano de fundo principal e cor de destaque do cabeçalho.
*   **Contraste e Legibilidade:** Para balancear o fundo vermelho vivo sem cansar a visão do usuário, os blocos de conteúdo e textos utilizam tonalidades de vinho extremamente escuras (`#3f1921` e `#53212b`) com textos totalmente brancos (`#ffffff`). Isso garante uma leitura confortável e um visual moderno.
*   **Fundo Temático Imersivo:** Na página de Tier List, o mapa *Ascent* foi aplicado como imagem de fundo utilizando `background-attachment: fixed`. Isso faz com que o mapa permaneça estático nas laterais decorando o site, enquanto a estrutura de ranking desliza suavemente por cima dele.
*   **Dimensão Industrial dos Itens (`80px`):** O tamanho de `80px` para os avatares dos agentes foi escolhido estrategicamente para permitir o reconhecimento imediato de cada personagem, ao mesmo tempo em que garante espaço suficiente para que vários itens fiquem enfileirados em telas de notebooks ou computadores menores.
