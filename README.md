# Loader / Spinner

Este projeto é um exemplo simples de **loader animado** utilizando
**HTML e CSS puro**. Ele exibe um círculo girando (spinner) para ser
usado como indicador de carregamento em páginas web.

## Tecnologias Utilizadas

-   **HTML5** para a estrutura da página.\
-   **CSS3** para estilização e animação.

## Estrutura do Projeto

    /
    ├── index.html
    └── styles/
        └── style.css

## Como Funciona

1.  O HTML cria uma `div` com a classe `loader`.\
2.  O CSS estiliza esta `div` para parecer um círculo com borda.\
3.  A propriedade `border-right-color` cria o efeito visual da cor em um
    dos lados do círculo.\
4.  A animação `@keyframes spin` aplica rotação de **0° a 360°**,
    criando o efeito de carregamento.

## Código Principal

-   **HTML:**

``` html
<div class="loader"></div>
```

-   **CSS:**

``` css
.loader {
    height: 200px;
    width: 200px;
    border: 12px solid #e3e3e3;
    border-radius: 50%;
    border-right-color: #4070f4;
    animation: spin 1s ease infinite;
}

@keyframes spin {
    100% {
        transform: rotate(360deg);
    }
}
```

## Como Executar

1.  Baixe os arquivos ou clone o repositório.\
2.  Abra o arquivo `index.html` em qualquer navegador.

## Possíveis Melhorias

-   Permitir diferentes tamanhos e cores com variáveis CSS.\
-   Adicionar mais estilos de loaders.\
-   Tornar responsivo para diferentes layouts.
