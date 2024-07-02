# 🖼️ HTML Images 

💡 Para adicionar imagens

``` html
<body>
    <img src="img/images.jpg" alt="txt alternativo">
</body>

```
## ➜ HTML Images Syntax

* `<img>` - Utilizado para incorporar uma imagem em uma página web;

* A tag `<img>`cria um espaço de retenção para uma imagem referenciada.

* Assim, temos dois atributos importantes:
    * **scr** - Especifica o caminho para imagem;
    * **alt** - Texto alternativo para imagem.

💡 Sytax: 

``` html
<img src="url" alt="alternatetext">

```

## ➜ Image Size - Width and Height
* É possível utilizar o `<style>` para especificar altura e largura de uma imagem. (Width - Altura, Height - Largura)


**Exemplo**

``` html
<img src="img/planeta-terra.webp" alt="Planeta Terra" style="width:440px; height: 300px;">

```

## ➜ Width and Height, or Style?
* Os atributos de altura e largura são válidos no HTML. No entanto, sugerimos usar o atributo `<style> `. 

**Exemplo**

``` html
<style>
        img{
            width: 100%;
        }
    </style>
</head>
<body>
    <img src="img/planeta-terra.webp" alt="Planeta Terra" style="width:440px; height: 300px;">
    <img src="img/planeta-terra.webp" alt="Planeta Terra" style="width:440; height: 300;">

    <p>A primeira imagem usa o atributo style para definir a largura em 128 pixels. Isso não será substituído pelo estilo na seção head:</p>

    <p> A segunda imagem usa o atributo width (definido como 128 pixels), mas o estilo na seção head o substitui e define a largura como 100%.</p>


</body>

```

## ➜ Images on Another Server/Website
* Para apontar para uma imagem em outro servidor, você deve especificar uma URL absoluta (completa) no atributo src:

**Exemplo**

``` html
<img src="https://www.infoescola.com/wp-content/uploads/2010/04/banana_600797891.jpg" alt="banana">

```
**⚠️ Cuidado com o copyright!** 

## ➜ Animated Images
* Podemos utilizar GIFS!

**Exemplo**

``` html
<img src="img/deadpool-04.gif" alt="deadpoll" style="width: 300px; height: 300px;">

```

## ➜ Image as a Link
* Use uma imagem como link, coloque a tag `<img>` dentro da tag `<a>`.

**Exemplo**

``` html
<a href="https://freemind.com.br/blog/dicas-de-prevencao-as-drogas/">
        <img src="img/59853d40760b9efab4d7edb33aa52ffd.gif" alt="bomdiaamigos" style="height: 300px; width: 300px;">
    </a>

```

## ➜ Image Floating
* Use a propriedade CSS float para deixar a imagem flutuar para a direita ou para a esquerda:

**Exemplo**

``` html
<p> <img src="img/sorriso.png" alt="sorriso" style="float:right;height:102px; width: 120px;"></p>

```

## 📚 Sintetizando os comandos utilizados

| Comando | Função |
|---------|--------|
| `<img>` | Define uma imagem |
| scr | Atribui um caminho a imagem |
| alt | Texto alternativo |
| width and height| Altura e largura |
| float | Para flutuar para a esquerda ou para a direita |


# 🌐 HTML Image Maps 

* Com mapas de imagens HTML, você pode criar áreas clicáveis ​​em uma imagem.

## Image Maps

* A tag `<map>` define um mapa de imagem;
* Mapas de imagem são imagens com áreas clicáveis;
* Para criar áreas `<area>`.

### ✔️ The Image (`<usemap>`)
* A imagem deve ser inserida utilizando a tag `<img>`, entretanto, para se diferenciar das outras,  o atributo `<usemap>` deverá ser utilizado;
* O valor `<usemap>` começa com **#** seguida pelo nome do mapa da imagem.

**Exemplo:**

``` html
<img src="/Html/img/laptop-3047422_1280.jpg" alt="fotolaptop" usemap="#workmap">

```

### ✔️ Create Image Map (`<map>`)

* O elemento `<map>` é usado para criar um mapa de imagem e está vinculado à imagem usando o atributo `name`;
* O atributo `name` deve ter o mesmo valor do atributo `<usemap>`.

**Exemplo:**

``` html
<map name="workmap"> </map>

```

### ✔️ The Areas
* Uma área clicável é definida usando um elemento `<area>`.
* Site para demarcar coordenadas: [Free Online Image Map Generator](https://www.image-map.net)
* Em caso de dúvida, utilize esse site para consulta: [HTML Image Maps](https://www.w3schools.com/html/html_images_imagemap.asp)

#### ✔️ Shape

Você pode utilizar os seguintes valores:
**rect** - Região retângular
**circle** - Região circular
**poly** - Região poligonal
**default** - Toda região

**Exemplo:**

``` html
<area shape="rect" coords="436,377,1179,718" alt="" href="computador.html">

```

## ➜ Image Map and JavaScript
* Adicionando o evento click na área.

**Exemplo**

``` html
<body>
    <h1 style="text-align: center; font-size: 40px; color: rgb(90, 20, 155);">HTML Image Maps</h1>

    <img src="/Html/img/laptop-3047422_1280.jpg" alt="fotolaptop" usemap="#workmap">]
    <map name="workmap">
        <area shape="rect" coords="436,377,1179,718" alt="" href="computador.html" onclick="clickcomp()">
    </map>

<script>
function clickcomp(){
    alert("Você clicou no computador")
}
</script>

</body>

```

# ☁️ HTML Background Images

## ➜ Background Image on a HTML element (`<background-image>`)
* Para mudarmos o plano de fundo utilizando imagens, usamos o atributo `<background-image>`

**Exemplo**

``` html
   <p style="background-image: url(img/planeta-terra.webp);">
        Em linguística, a noção de texto é ampla e ainda aberta a uma <br>
        definição mais precisa. Grosso modo, pode ser entendido como <br>
        manifestação linguística das ideias de um autor, que serão <br>
        interpretadas pelo leitor de acordo com seus conhecimentos  <br>
        linguísticos e culturais. Seu tamanho é variável.
    </p>

```

* Podemos utilizar isso no `<style>`:

**Exemplo**

``` html
<style>
        p{
            background-image: url(img/sorriso.png);
        }
    </style>
```

## ➜ Background Image on a Page
* Se você deseja que a página inteira tenha uma imagem de fundo, você deve especificar a imagem de fundo no elemento `<body>`:

**Exemplo**

``` html
  body{
            background-image: url(img/sorriso.png);
        }

```

## ➜ Background Repeat
* Se a imagem de fundo for menor que o elemento, a imagem se repetirá até chegar ao fim do elemento. 
* Para evitar que a imagem de fundo se repita, defina a propriedade `background-repeat` como `no-repeat`.

**Exemplo**

``` html
 body{
            background-image: url(img/sorriso.png);
            background-repeat: no-repeat;
        }

```

## ➜ Background Cover
* Caso queira que a imagem de fundo cubra todo o elemento, você pode definir a propriedade `<background-size>` como `cover`.
* Para garantir que todo elemento esteja coberto defina a propriedade `background-attachment` como fixa.

**Exemplo**

``` htmk
<style>
        body{
            background-image: url(img/sorriso.png);
            background-repeat: no-repeat;
            background-attachment: fixed;
            background-size: cover;
        }
</style>

```

## ➜ Background Stretch
* Se você quiser que a imagem de fundo se estique para caber em um elemento todo, você pode definir a propriedade `<background-size>` como 100% 100%.

**Exemplo**

``` html
<style>
        body{
            background-image: url(img/sorriso.png);
            background-repeat: no-repeat;
            background-attachment: fixed;
            background-size: 100% 100%;
        }
    </style>

```





