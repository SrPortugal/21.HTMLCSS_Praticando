<h1>Praticando HTML e CSS</h1>

O projeto do figma esta disponivel na url: https://www.figma.com/file/tFDVyNuKhrT2G03k2dCstW/Alura-Plus---Layout?node-id=1-77&t=H4SU5vNkK7URhOPu-0


Na aula 2 criamos o botao azul e o botao transparente

```HTML
<a href="www.alura.com.br" class="container__botao">Assine por 12x de R$ 120,00</a>
<a href="www.alura.com.br" class="container__botao botao_secundario">Assinar somente o Alura+</a>
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
```
