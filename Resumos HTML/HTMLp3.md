# HTML - CSS

# 💭 O que é CSS?
* Em inglês é denominado como: Cascading Style Sheets (CSS). Sendo este utilizado para estilização de páginas. Podemos alterar cores, tamanhos, planos de fundo, etc.
* Podemos adicionar três documentos ao CSS: 

    1. **Inline**: Usando o atributo `<style>` dentro de um elemento HTML;
    2. **Internal**: Usando um elemento `<style>` na seção `<head>`;
    3. **External**: Usando um elemento `<link>` para vincular a um arquivo.


### 📌 Inline CSS
* O inline é utilizado para aplicar um estilo a um único elemento HTML.

➤ Observe o exemplo:

``` html
<h1 style="color:blue;">Olá mundo!</h1>

```

### 📌 Internal CSS
* Define o modelo de texto de TODOS os elementos nesta página.

➤ Observe o exemplo: 

``` html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body{
            background-color: bisque;
        }
        h2{
            color:blueviolet
        }
        p{
            color: brown;
        }
    </style>
</head>
<body>
    <h2>Isto é um título! </h2>
    <p>Isto é um parágrafo!</p>
</body>
</html>
```

### 📌 External CSS
* É utilizado para definir o estilo de muitas páginas. Sendo assim, é criado um link externo.

➤ Observe o exemplo: 

**HTML**
``` html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h2>Isto é um título! </h2>
    <p>Isto é um parágrafo!</p>
</body>
</html>

```

**CSS**
``` css
body{
    background-color: bisque;
}
h2{
    color: blue;
}
p{
    color: chocolate;
}
```

## 🎀 CSS Colors, Fonts and Sizes

Aqui apresentaremos algumas propriedades usadas no CSS:

* A propriedade CSS `<color>` define a cor do texto a ser utilizada.
    [Lista de cores disponíveis](https://www.w3schools.com/colors/colors_names.asp)

* A propriedade CSS `<font-family>` define a fonte a ser usada.

* A propriedade CSS `<font-size>` define o tamanho do texto a ser usado.

➤  Observe o exemplo: 

``` html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        h2{
            color: rgb(90, 10, 10);
            font-family: Verdana, Geneva, Tahoma, sans-serif;
            font-size: 300%;
        }
        p{
            color: black;
            font-family: 'Courier New', Courier, monospace;
            font-size: 160%;
        }

    </style>
</head>
<body>
    <h2> O que é o gambito da rainha?</h2>
    <p>uma abertura em que você sacrifica uma peça para tirar vantagem disso depois. </p>
    <p>uma abertura em que você sacrifica uma peça para tirar vantagem disso depois. </p>
    <p>uma abertura em que você sacrifica uma peça para tirar vantagem disso depois. </p>
</body>
</html>

```

### 📌 CSS Border
* Define uma borda em volta de um elemento HTML.

➤ Observe o exemplo:

``` html
p{
    border: 2px solid powderblue;
}

```

### 📌 CSS Padding
* Define um espaço/preenchimento entre o texto e a borda.

➤ Observe o exemplo: 

``` html
        p{
            border: 2px solid powderblue;
            padding: 20px;
        }

```

### 📌 CSS Margin
A propriedade CSS margin define uma margem (espaço) fora da borda.

➤ Observe o exemplo:

``` html
 p{
            border: 2px solid powderblue;
            margin: 40px;
        }

```

## 📎 Link to External CSS
* Páginas de estilo externas podem ser referenciadas com um URL completo ou com um caminho relativo à página da web atual.

➤ Observe o exemplo: 

``` html
<link rel="stylesheet" href="https://www.w3schools.com/html/styles.css">

```

* Páginas de estilo podem estar em pastas distintas.

➤ Observe o exemplo:

``` html
<link rel="stylesheet" href="/pasta a/a.css">

```

* Pode estar localizada na pasta atual.

➤ Observe o exemplo: 

``` html
<link rel="stylesheet" href="style.css">

```

## 📚 Sintetizando os comandos utilizados

| Comando | Função |
| --------| -------|
| `<style>`| HTML - Elemento utilizado para atribuir CSS interno |
| `<link>` | HTML - Elemento para atribuir CSS externo |
| `<head>` | HTML - Para armazenar os elementos `<style>` e `<link>` |
| `<color>` | CSS = Colorir elementos |
| `<font-family>` | CSS - Colocar fontes nos textos |
| `<font-size>`| CSS - Alterar tamanho da fonte |
| `<border>` | CSS - Propriedade para colocar espaços dentro da bordas |
| `<padding>` | CSS - Propriedade para colocar espaços entre as bordas |
| `<margin>`| CSS - Propriedade para espaços fora da borda |

# HTML Links 

* Os links permitem que o usuário vá de uma página para outra.

##  🌐 HTML Links - Hyperlinks
* São chamados de hiperlinks;
* Você pode clicar em um documento e ir para outro documento;
* Um link não precisa ser necessariamente um texto, mas uma imagem também.
* É possível estilizar links no CSS.

### 📌 HTML Links - Syntax
* A tag `<a>` define um hiperlink.

Sintaxe:

``` html
<a href="url">link text</a>

```

➤ O atributo mais importante de `<a>` é o elemento `<href>` pois indica o destino do link.

### 📌 HTML Links - The target Attribute
* Por padrão, a página vinculada será exibida na janela atual do navegador. Para alterar isso, você deve especificar outro destino para o link;

➤ O atributo `<target>` especifica onde abrir o documento vinculado.
Seus valores são:

```
    1. _self  - Padrão, abre o documento na mesma janela em que foi clicado;
    2. _blank - Abre o documento em uma nova guia;
    3. _parent - Abre o documento (in the parent frame?);
    4. _top  - Abre o documento em todo corpo da janela.
```

Exemplo:

``` html
<a href="https://www.netflix.com/br/title/80234304" target="_blank">O gambito da rainha< a>

```

## ✉️ Absolute URLs vs. Relative URLs
➤ Ambos os exemplos acima usam Absolute URL (um endereço da web completo) no atributo href.
➤ Um link local (um link para uma página dentro do mesmo site) é especificado com um Relative URL (sem a parte “https://www”):

Exemplos:

``` html
<body>

    <h1>Absolute URL</h1>
    <p><a href="https://www.letras.mus.br/tv-girl/lovers-rock/traducao.html">Lovers-rock</a></p>
    <p><a href="https://www.letras.mus.br/cigarettes-after-sex/apocalypse/">Apocalypse</a></p>

    <h1>Relative Links</h1>
    <p><a href="e2.html">HTML 1</a></p>
    <p><a href="e4.html">HTML 2</a></p>


</body>

```

## 📁 HTML Links - Use an Image as a Link
* Utilize a tag `<img>`.

Exemplo:

``` html
<h1>Image as a Link</h1>
    <p>Clique no Coringa</p>
    <a href="https://www.adorocinema.com/filmes/filme-258374/" target="_blank"><img src="/img/coringa.png" alt="HTML tutorial - Coringa" style="width: 120px; height: 120Spx;"></a>

```

## 📧 Link to an Email Address
➤ Utilize `<mailto>` dentro do atributo `<href>` para abrir um programa de email para o usuário.

Exemplo:

``` html
 <a href="mailto:jujumoraes123654@gmail.com">Send Email</a>

``` 

## 💡 Button as a Link
* Para usar um botão HTML como link, você deve adicionar algum código JavaScript.

``` html
<body>
    <button id = "botaoclick" onclick="document.location='e4.html'">HTML tutorial</button>

    <script>
        var botao = document.getElementById("botaoclick").innerHTML = "Olá mundo!"
    </script>
</body>

```

## 💡 Link Titles
* Especifica informações extras sobre um elemento.

Exemplo: 

``` html 
<a href="https://www.w3schools.com/html/default.asp">HTML tutorial</a>

```

## 📚 Sintetizando os comandos utilizados

| Comando | Função |
|---------|--------|
|`<a>` | Definindo um link |
|`<href>` | Definindo um endereço |
|`<target>`| Atributo para definir onde o site será aberto |
| `<img>` dentro de `<a>` | Inserindo imagem em um link |
| `<mailto>` | Para abrir um programa de email |

# Link Colors
* Para mudar certos designs quando clicamos em um link podemos utilizar o CSS para estilizar. 

➤ Aqui, um link não visitado ficará verde sem sublinhado. Um link visitado ficará rosa sem sublinhado. Um link ativo ficará amarelo e sublinhado. Além disso, ao passar o mouse sobre um link (a:hover) ele ficará vermelho e sublinhado:

``` html
<style>
        a:link{
            color: green;
            background-color: transparent;
            text-decoration: none; /*Tirando o sublinhado */
        }
        a:visited{
            color: pink;
            background-color: transparent;
            text-decoration: none;
        }
        a:hover{
            color: red;
            background-color: transparent;
            text-decoration: underline;
        }
        a:active{
            color: yellow;
            background-color: transparent;
            text-decoration: underline;
        }
    </style>

```
## 📁 Link Buttons
➤ Estilizando botões com CSS:

``` html
<style>
        a:link, a:visited{
            background-color: rgb(75, 16, 131);
            color: white;
            padding: 15px;
            text-align: center;
            text-decoration: none;
            display: inline-block;

        }
        a:hover, a:active{
            background-color: rgb(46, 4, 85);
        }

    </style>

```

