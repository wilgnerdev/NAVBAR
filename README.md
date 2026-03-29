# NAVBAR
Criação de uma navbar responsiva em alusão ao meu projeto de tcc.


# ESTILIZAÇÃO INICIAL

===== HEADER ===== 
Não usar no Css, apenas o nav.

===== NAV =====
display: flex; <!-- para alinhar todos elementos um ao lado do outro. --> 

justify-content: space-around; <!-- fazer com que o espaço ao redor seja igual ao espaço entre eles -->

align-items: center; <!-- alinhar verticalmente ao centro  -->

height: 8vh; <!-- VIEWPORT-HEIGHT: unidade reponsiva que se adapta a altura da janela de visualização do usuário. obs sendo que 100vh cobre a janela inteira  -->

letter-spacing <!-- espaçamento interno das letras --> 

margin-left <!-- espaçamento a esquerda entre os elementos  -->

===== MAIN =====
background: url(../paisagem_navbar.jpg) no-repeat center center; <!-- Se refere ao seu posicionamento nos eixos X e Y -->

background-size: cover; <!-- Caso a resolução do monitor for maior que a imagem -->

# DESIGN RESPONSIVO
Abertura da media querie: @media (max-width: 999px)

===== BODY =====
overflow-x: hidden; <!-- se algo transborda, fica escondido do body, logo o sroll do nav-list não fica pra fora do body --> 

===== NAV-LIST =====
position: absolute; <!-- fica livre no site para podermos mover com position -->
width: 50vw; <!-- Ocupa metade da tela --> 

flex-direction: column; <!-- elementos em coluna (um abaixo do outro) -->

align-items: center;    <!-- Eixo muda quando coluna -->

justify-content: space-around; 
/* distribuir os elementos pelo espaço disponível  */

transform: translateX(100%);
/* Move a navegação pra fora da tela (vai ficar fora do body gerando uma horrível barra de scroll vertical, dai usamos overflow-x com o valor de hidden) */

===== MOBILE-MENU =====
display: block; 
/* layout flexbox automaticamente se ajusta */

===== NAV-LIST.ACTIVE =====
transform: translateX(0);
/* quando essa classe tiver ativa, a tag transform voltara com valor de translateX(0) (fazendo a barra voltar). obs: active é a classe que sera adicionada no js */


/*  */
/*  */
/*  */
/*  */
<!-- -->
<!-- -->
<!-- -->
<!-- -->


# APRENDIZADO

Procurando vídeos sobre no youtube, estava com um problema de responsividade, a nav-list ficava pra fora do body quando a tela tava em 999px, foi aí que usei a <meta name="viewport" content="width=device-width, initial-scale=1.0, minimum-scale=1"> e resolveu o problema para mim.