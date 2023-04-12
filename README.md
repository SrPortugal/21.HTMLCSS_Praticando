<h1>Praticando HTML e CSS</h1>

O projeto do figma esta disponivel na url: https://www.figma.com/file/tFDVyNuKhrT2G03k2dCstW/Alura-Plus---Layout?node-id=1-77&t=H4SU5vNkK7URhOPu-0


Na aula 2 criamos o botao azul e o botao transparente

```HTML
    <section class="container principal">
        <div>
            <h1 class="container__titulo">Com o Combo+, você pode aproveitar a Alura+ e o Alura Língua por um preço único.</h1>
            <img src="./img/Combo.png" alt="O Combo+ é a junção do alura+ e o alura lingua">
            <a href="www.alura.com.br" class="container__botao">Assine por 12x de R$ 120,00</a>
            <a href="www.alura.com.br" class="container__botao botao_secundario">Assinar somente o Alura+</a>
            <p class="container__aviso">*O preço pode variar caso a assinatura seja feita em outros planos.</p>
        </div>
    </section>
```

```CSS
.container__botao {
    text-decoration: none;
    background-color: var(--botao-azul);
    border-radius: 5px;
    padding: 1em;
    color: var(--branco-principal);
    display: block;
}
.botao_secundario {
    background-color: transparent;
    border: var(--branco-principal) 2px solid;
}
.container__aviso {
    color: var(--cinza-secundario);
    font-size: 12px;

}
```
Criamos os botoes e o texto de Obs


Aula 3

vamos ajustar as margens e o Padding

```html
<section class="container principal">
    <div class="container__caixa">
        <h1 class="container__titulo">Com o Combo+, você pode aproveitar a Alura+ e o Alura Língua por um preço único.</h1>
        <img src="./img/Combo.png" alt="O Combo+ é a junção do alura+ e o alura lingua" class="container__imagem">
        <a href="www.alura.com.br" class="container__botao">Assine por 12x de R$ 120,00</a>
        <a href="www.alura.com.br" class="container__botao botao_secundario">Assinar somente o Alura+</a>
        <p class="container__aviso">*O preço pode variar caso a assinatura seja feita em outros planos.</p>

    </div>
</section>

<section class="container secundario">
    <img src="./img/Plataformas.png" alt="Um computador e um celular com o site aberto" class="secundario__imagem">
    <!-- <div class="container__secundario"> -->
    <div class="container__descricao">
        <h2 class="descricao__titulo">Assista do seu jeito</h2>
        <p class="descricao__texto">Aproveite a tela grande da TV ou assista no tablet, laptop, celular e outros 
            aparelhos. Nossa seleção de cursos não para de crescer.</p>
    </div>
</section>

<section class="container secundario">
    <!-- <div class="container__caixa"> -->
    <div class="container__descricao">
        <p class="descricao__texto">Só o Combo+ oferece Alura+ e Alura Língua juntos para você ter acesso a cursos 
            de diversas áreas da tecnologia e aprender inglês ou espanhol, onde e como quiser.</p>
        <a href="www.alura.com.br" class="container__botao secundario__botao">Assine o Combo+</a>
    </div>
    <img src="./img/Telas.png" alt="Duas telas da pagina do curso" class="secundario__imagem">
</section>

<section class="container secundario">
    <img src="./img/Notebook.png" alt="Um notebook com um site aberto nele" class="secundario__imagem">
    <div class="container__descricao">
        <h2 class="descricao__titulo">Baixe seus cursos</h2>
        <p class="descricao__texto">Baixe e assista quando e onde quiser. Assim, seus favoritos estão 
            sempre com você, até mesmo sem internet.</p>
    </div>
</section>
```

```css
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap');
/* @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100&display=swap'); */

:root {
    --branco-principal: #ffffff;
    --cinza-secundario: #C0C0C0;
    --botao-azul: #167BF7;
    --cor-de-fundo: #00030C;
    /* --font-principal: 'Inter', sans-serif; */
    /* --font-principal: 'Roboto'; */
    --font-principal: 'Inter';
}

body {
    background-color: var(--cor-de-fundo);
    color: var(--branco-principal);
    font-family: var(--font-principal);
    font-size: 16px;
    font-weight: 400;
}
* {
    margin: 0;
    padding: 0;
}

.principal {
    background-image: url("./img/Background.png");
    background-repeat: no-repeat;
    background-size: contain;
    align-items: center;
    text-align: center;
}

.container {
    height: 100vh;
    display: grid;
    grid-template-columns: 50% 50%;

}

.container__caixa {
    margin: 0 6em;
}
.container__titulo {
    font-size: 28px;
    font-weight: 700;
}

.container__imagem {
    margin: 1em 0 2em 0;
}
.container__botao {
    text-decoration: none;
    background-color: var(--botao-azul);
    border-radius: 5px;
    padding: 1em;
    color: var(--branco-principal);
    display: block;
    margin-bottom: 1em;
}

.botao_secundario {
    background-color: transparent;
    border: var(--branco-principal) 2px solid;
}

.container__descricao {
    padding:  2em;
}
.container__aviso {
    color: var(--cinza-secundario);
    font-size: 12px;

}

.secundario__imagem {
    width: 80%
}

.secundario {
    align-items: center;
    margin: 0 10em;
}

.descricao__titulo {
    font-weight: 700;
    font-size: 48px;
    color: var(--branco-principal);
    margin-bottom: 0.1em;
}

.descricao__texto {
    color: var(--cinza-secundario);
}

.secundario__botao {
    display: inline-block;
    margin-top: 1em;
}

```

