
# Listas

Para começarmos uma lista utilizamos a tag `<ul>` e após a tag `<li>` para listar os itens. 

**Exemplo**

``` html
<h2>Café da manhã</h2>
    <ul>
        <li>Café</li>
        <li>Leite</li>
        <li>Pão</li>
        <li>Manteiga</li>
    </ul>

```

**Código exibido**

## Café da manhã
* Café
* Leite
* Pão
* Manteiga

Podemos listar os itens utilizando números, e para isso utilizaremos a tag `<ol>` e após a tag `<li>`.

**Exemplo**

``` html
<h2>Café da manhã</h2>
    <ol>
        <li>Café</li>
        <li>Leite</li>
        <li>Pão</li>
        <li>Manteiga</li>
    </ol>

```

**Código exibido**

## Café da manhã
    1. Café
    2. Leite
    3. Pão
    4. Manteiga

## HTML Description Lists
* Listas com descrição;
* Uma descrição para cada termo;
* `<dl>` Define a lista de descrição;
* `<dt>` Define o termo;
* `<dd>` Descreve cada termo.

**Exemplo**

``` html
<h2>Café da manhã</h2>
    <dl>
        <dt>Café</dt>
        <dd>- Uma bebida quente </dd>
        <dt>Leite</dt>
        <dd>- Uma bebida fria</dd>
    </dl>

```

**Código exibido**

Café

    - Uma bebida quente

Leite

    - Uma bebida fria

## Unordered HTML List - Choose List Item Marker
* `list-style-type` Propriedade utilizada para definir o estilo da lista.

| Valor | Descrição |
|--------|----------|
| disc | Marcador padrão |
| circle | O marcador é um círculo |
| square | O marcador é um quadrado |
| none | Sem marcadores |

**Exemplos**

``` html
<ul style="list-style-type: circle;">
        <li>Café</li>
        <li>Leite</li>
        <li>Pão</li>
    </ul>
```

## Horizontal List with CSS

``` html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>

    <style>
        ul {
            list-style-type: none;
            margin: 0;
            padding: 0;
            overflow: hidden;
            background-color: rgb(27, 2, 49);
        }

        li {
            float:left;
        }

        li a {
            color:white;
            display: block;
            text-align: center;
            padding: 16px;
            text-decoration: none;
        }

        li a:hover {
            background-color: rgb(64, 42, 83);
        }

    </style>

</head>
<body>
   <ul>

    <li> <a href="#home">Home</a></li>
    <li><a href="#contatos">Contatos</a></li>
    <li><a href="#sobre">Sobre</a></li>

   </ul>
</body>
</html>

```

