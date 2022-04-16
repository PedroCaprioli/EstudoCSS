comentario no css /* blabla */


// propriedades //

sempre fecham com (;)

. color (cor)
. font-soze (tamanho da fonte)
. background (fundo)
. margin (espaçamento fora da caixa)
. padding (preechimento dentro da caixa)
. font-weight:
    . lighter (afinar "menos negrito")
    . bold (negrito)
    . bolder (muito negrito)
. font-family: (colocar fonte)
    . normalmente é colocado no * do css
    . poder importar fontes do google forms

// seletores //

```HTML
    <div id="container" class="m-40">
        <h1>Título</h1>
        <h2>Subtitulo</h2>
    </div>
```
```CSS
    /* ID selector */
    #container {
        width: 200px;
    }

    /* Class selector */
    .m-40 {
        margin: 40px;
    }

    /* Element/Type selector + Agrupamento de seletores */
    h1, h2 {
        color: blue;
        font-size: 60px;
        background: gray;
    }
```
// regras //

. @import serve para incluir um CSS externo.
. @media são regras condicionais para vários dispositivos.
. @font-face é para colocar fontes externas.
. @keyframes serve para as animations do CSS.

// Position //

Controla onde, na página, o elemento irá ficar, alterando o fluxo normal dos elementos.

. Name: position
. Value: static | relative | absolute | fixed

//STATIC//

Por padrão os elementos são static. Isso significa que os elementos irão seguir o fluxo normal do HTML

//RELATIVE//

(top, right, bottom, left e z-index)

Lembrando que o fluxo normal dos elementos é ficar um abaixo do outro, a não ser no caso de elementos inline, que ficam um ao lado do outro.

Quando o position é relative os elementos são deslocados do seu posicionamento normal, mas sem afetar o posicionamento de outros elementos da página.

```HTML

<div class="box box1"></div>
<div class="box box2"></div>
<div class="box box3"></div>
```

```CSS

.box {
  width: 50px;
  height: 50px;
  margin-bottom: 8px;
}

.box1 {
  background-color: red;
  position: relative;
  left: 100px;
  top: 80px
}

.box2 {
  background-color: green;
}

.box3 {
  background-color: blue;
}
```
// Absolute //

Quando o position é absolute o elemento é deslocado saindo do fluxo normal. O elemento de position absolute é posicionado em relação ao seu parent element mais próximo. Se esse elemento "pai" não existir, ele será posicionando em relação ao bloco contendo a raiz do elemento.

```HTML

<div class="boxa boxa1"></div>
<div class="boxa boxa2"></div>
<div class="boxa boxa3"></div>
```

```CSS

.boxa {
  width: 50px;
  height: 50px;
  margin-bottom: 8px;
}

.boxa1 {
  background-color: red;
  position: relative;
  left: 100px;
  top: 80px
}

.boxa2 {
  background-color: green;
}

.boxa3 {
  background-color: blue;
}
```

// FIXED //

Quando aplicado o position fixed é como se criasse um elemento flutuante que fica fixo na página, independente do scrolling feito.

// element stacking //

(z-index)

É o empilhamento de elementos. Podemos usar o z-index para determinar a ordem da posição do elemento. Quanto maior o z-index, mais "acima" vai aparecer o elemento.

// flex box //

. Nos permite posicionar os elementos dentro da caixa
. Controle em uma dimensão (horizontal ou vertical)
. Alinhamento, direcionamento, ordenar e tamanhos

- Propriedades -
 . flex-direction (row,columm)
 . justify-content ()
 . align-items:

```HTML
div.parent {
	display: flex;
}
```
Flex-direction
. Qual a direção do flex: horizontal ou vertical
. row | column
Alinhamento
. justify-content
. align-items

```HTML
<div class="container">
  <div class="box blue"></div>
  <div class="box red"></div>
  <div class="box green"></div>
</div>
```

```css

.container {
    display: flex;
    justify-content: space-between;
}
.box {
  width: 50px;
  height: 50px;
  margin-bottom: 8px;
}

.blue {
  background-color: blue;
}

.red {
    background-color: red;
}

.green {
    background-color: green;
}
```
// CSS //

3 formas de adicionar CSS
    . inline CSS: Direto no elemento HTML (má 
    pratica)
    (<h1 style="color: red">olá mundo</h1>)

    . CSS Interno: Usando tags <style> no documento HTML dentro do <head>
    (<style>
        h1 {
            color:red;
        }
    </style>)

    . CSS Externo: Importando um arquivo .css no HTML

. final sempre colocar ;

//CSS Selectors//

. p (selector) (elemento que quer selecionar pra estilizar)
. {color: (property)
. red; (value)
. border: (property)
. 1px solid blue;} (values)

``` css
    p{
        color:red;
        border:1px solid blue;
    }
```



///// Selecionando elementos específicos /////
    . Usando classes: selecionar mais de um elemento
    . Usando ID: selecionar apenas um elemento

//HTML//
``` html 
    <h1 class="segundo-h1">olá mundo</h1>
```
//CSS//
``` css
    .segundo-h1 {
    color: red;
    }
```


// Atributos //
    . class="" (estilizar mais de um elemento com o mesmo estilo)
        . Inicia com (.)
```css
    .selector {
    color: royalblue;
}
```            
    . id="" (estilizar apenas um elemento)
        . Inicia com (#)
```css 
    #selector {
    color: royalblue;
}
``` 

// Cores no CSS //
    . Nome da cor (red,blue,white)
    . Hexadecimal (#000000)
    . RGB & RGBA (rgb(0,0,255) e rgba(0,0,255,0.6))

``` css
    body {
        background: red;
        color: white;
    }

    h1 {
        color: #000000
    }

    p {
        color: rgb(0,0,255)
    }

    a {
        color: rgba(0,0,255,0.6)
    }
```
// FONTES EXTERNAS //
     . https://fonts.google.com
     . colocar o <link> do site em <head> do arquivo html
     . colocar font-family no arquivo css]

// Propriedades usadas //
    . margin: auto; (colocar tudo no meio(espaçamento fora do conteudo))(top,left,right,bottom)
    . padding (top,left,right,bottom): (espaçamento dentro do conteudo)
    . border: (borda do conteudo)(top,left,right,bottom)
    . width: 60%; (com porcentagem fica mais responsivo menos usado)
    . box-sizing: border-box; (deixa mais responsivo e mais usado)

``` css
    .container {
        padding-top: 60px;
        padding-bottom: 60px;
        padding-left: 60px;
        padding-right: 60px;
        /* Mesma coisa que acima , funciona com border,margin */
        padding: 60px;
        
    }
```