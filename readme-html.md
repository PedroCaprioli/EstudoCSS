// Abrir outra pagina //

``` html 
    <a href="index.html" target="_blank">
```

// colocar link em imagem //

``` html
    <a href="index.html">
        <img src="imagens/logo.png">
    </a>
```
// funcionar css //

``` html
    <link rel="stylesheet" href="arquivo de css">
    <!-- colocar em <head> -->
```
// funcionamento do <a href=""> </a> //
 . links sempre ter https:// no começo
    . https://google.com
 . emails sempre ter mailto: no começo
    . mailto:batatafrita123@gmail.com
 . telefones sempre ter tel: no começo
    . tel:+5500999999999

// conteudos do <a href=""> </a> //
``` html
    <a href="index.html">
        <img src="imagens/logo.png"> <!-- ao clicar na imagem ira para o link direcionado -->
        <p> batata </p> <!-- ao clicar em batata ira para o link direcionado -->
        <h1> batato </h1> <!-- ao clicar em batato ira para o link direcionado -->
    </a>
```

// colocar icone na aba do navegador //
``` html
    <!-- colocar em <head> -->
    <link rel="icon" href="arquivo do icon">


    <!-- Usar framework para isso: -->
    <!--- IPhone nao-retina, ipod touch e dispositivos android 2.1+: -->
    <link rel="apple-touch-icon-precomposed" href="arquivo do icon">
    <!-- iPad de primeira e segunda geração: -->
    <link rel="apple-touch-icon" sizes="48x48" href="arquivo do icon"/>

    <link rel="apple-touch-icon" sizes="72x72" href="arquivo do icon"/>

    <link rel="apple-touch-icon" sizes="96x96" href="arquivo do icon"/>

    <!-- iPhone com tela retina de alta resolução: -->
    <link rel="apple-touch-icon" sizes="144x144" href="arquivo do icon"/>

    <!-- iPad de terceira geração com tela retina de alta resolução: -->
    <link rel="apple-touch-icon" sizes="192x192" href="arquivo do icon"/>

    <link rel="apple-touch-icon" sizes="256x256" href="arquivo do icon"/>

    <link rel="apple-touch-icon" sizes="384x384" href="arquivo do icon"/>

    <link rel="apple-touch-icon" sizes="512x512" href="arquivo do icon"/>

```
// ter propriedade sobre a pagina no google //
``` html 
    <meta name="author" content="seu nome">
```
// descrição da pagina no google //
``` html 
    <meta name="description" content="descrição do site">
```