
# HTML Links

## 🌐 HTML Links - Hyperlinks
* São chamados de hiperlinks;
* Você pode clicar em um documento e ir para outro;
* Um link não precisa ser necessariamente um texto, mas uma imagem também.
* É possível estilizar links no CSS.

### ➜ HTML Links - Syntax
* A tag `<a>` define um hiperlink.
  
``` html
<a href="url">link text</a>

```

* O atributo mais importante de `<a>` é o elemento `<href>` pois indica o destino do link.

### ➜ HTML Links - The target Attribute
* Por padrão, a página vinculada será exibida na janela atual do navegador. Para alterar isso, você deve especificar outro destino para o link;

* O atributo `<target>` especifica onde abrir o documento vinculado.
Seus valores são:

```
    1. _self  - Padrão, abre o documento na mesma janela em que foi clicado;
    2. _blank - Abre o documento em uma nova guia;
    3. _parent - Abre o documento (in the parent frame?);
    4. _top  - Abre o documento em todo corpo da janela.
```

**📌 Exemplo**

``` html
<a href="https://www.netflix.com/br/title/80234304" target="_blank">O gambito da rainha< a>

```

## ➜ Absolute URLs vs. Relative URLs
* Ambos os exemplos acima usam Absolute URL (um endereço da web completo) no atributo href.
*  Um link local (um link para uma página dentro do mesmo site) é especificado com um Relative URL (sem a parte “https://www”):

**📌 Exemplo**

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

## ➜ HTML Links - Use an Image as a Link
* Utilize a tag `<img>`.

**📌 Exemplo**

``` html
<h1>Image as a Link</h1>
    <p>Clique no Coringa</p>
    <a href="https://www.adorocinema.com/filmes/filme-258374/" target="_blank"><img src="/img/coringa.png" alt="HTML tutorial - Coringa" style="width: 120px; height: 120Spx;"></a>

```

## ➜ Link to an Email Address
 Utilize `<mailto>` dentro do atributo `<href>` para abrir um programa de email para o usuário.

**📌 Exemplo**

``` html
 <a href="mailto:jujumoraes123654@gmail.com">Send Email</a>

``` 

## ➜ Button as a Link
* Para usar um botão HTML como link, você deve adicionar algum código JavaScript.

**📌 Exemplo**
``` html
<body>
    <button id = "botaoclick" onclick="document.location='e4.html'">HTML tutorial</button>

    <script>
        var botao = document.getElementById("botaoclick").innerHTML = "Olá mundo!"
    </script>
</body>

```

## ➜ Link Titles
* Especifica informações extras sobre um elemento.

**📌 Exemplos**

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

# ➜ Link Colors
* Para mudar certos designs quando clicamos em um link podemos utilizar o CSS para estilizar. 

* Aqui, um link não visitado ficará verde sem sublinhado. Um link visitado ficará rosa sem sublinhado. Um link ativo ficará amarelo e sublinhado. Além disso, ao passar o mouse sobre um link (a:hover) ele ficará vermelho e sublinhado:

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
##  ➜ Link Buttons
Estilizando botões com CSS:

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
