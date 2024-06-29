
##  Introdução aos Estilos HTML - CSS

## 💭 O que é CSS?
* CSS (Cascading Style Sheets) é utilizado para estilizar páginas web, permitindo alterar cores, tamanhos, planos de fundo e muito mais.

💡 Podemos adicionar CSS de três maneiras:
1. **Inline**: Usando o atributo `<style>` dentro de um elemento HTML.
2. **Internal**: Usando um elemento `<style>` na seção `<head>`.
3. **External**: Usando um elemento `<link>` para vincular a um arquivo CSS externo.

##  ➜ Estilos Inline
Os estilos inline são aplicados diretamente aos elementos HTML usando o atributo `style`.

### 📌 Exemplo Completo de Estilo Inline

```html
<!DOCTYPE html>
<html>
<head>
    <title>Exemplo de Estilos Inline</title>
</head>
<body style="background-color:lightgrey;">

    <h1 style="color:blue; text-align:center;">Estilos Inline em HTML</h1>

    <p style="color:green; font-family:Arial, sans-serif; font-size:18px; border:1px solid black; padding:10px;">
        Este é um exemplo de parágrafo com múltiplos estilos aplicados.
    </p>

</body>
</html>

```
## ➜ Internal CSS
Define o estilo de TODOS os elementos em uma página específica.

### 📌 Exemplo Completo de Estilo Internal
```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body {
            background-color: bisque;
        }
        h2 {
            color: blueviolet;
        }
        p {
            color: brown;
        }
    </style>
</head>
<body>
    <h2>Isto é um título!</h2>
    <p>Isto é um parágrafo!</p>
</body>
</html>

```
## ➜ External CSS
É utilizado para definir o estilo de múltiplas páginas, criando um link para um arquivo CSS externo.

### 📌 Exemplo Completo de Estilo External
**HTML Exemplo:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h2>Isto é um título!</h2>
    <p>Isto é um parágrafo!</p>
</body>
</html>

```

**CSS Exemplo (style.css):**

```css
body {
    background-color: bisque;
}
h2 {
    color: blue;
}
p {
    color: chocolate;
}

```

## 🎨 Propriedades Comuns de Estilo

### ➜ Cor da Fonte (`color`)
A propriedade `color` é usada para definir a cor do texto.
[Lista de cores disponíveis](https://www.w3schools.com/colors/colors_names.asp)

**📌 Exemplo:**

```html
<p style="color:blue;">Este texto é azul.</p>

```

### ➜ Cor de Fundo (`background-color`)
A propriedade `background-color` é usada para definir a cor de fundo de um elemento.

**📌 Exemplo:**

```html
<div style="background-color:yellow;">
    <p>Este parágrafo tem um fundo amarelo.</p>
</div>

```

### ➜ Bordas (`border`)
A propriedade `border` é usada para definir bordas ao redor de um elemento.

**📌 Exemplo:**

```html
<p style="border:2px solid black;">Este parágrafo tem uma borda preta.</p>

```

## ✏️ Estilos de Texto

### ➜ Fonte (`font-family`)
A propriedade `font-family` define a família da fonte para o texto.

**📌 Exemplo:**

```html
<p style="font-family:Arial, sans-serif;">Este texto usa a fonte Arial.</p>

```

### ➜ Tamanho da Fonte (`font-size`)
A propriedade `font-size` define o tamanho do texto.

**📌 Exemplo:**

```html
<p style="font-size:20px;">Este texto tem 20 pixels de altura.</p>

```
### ➜ Alinhamento de Texto (`text-align`)
A propriedade `text-align` é usada para definir o alinhamento horizontal do texto.

**📌 Exemplo:**

```html
<h1 style="text-align:center;">Este texto está centralizado.</h1>

```

## 📌 Exemplo Completo de Estilos

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        h2 {
            color: rgb(90, 10, 10);
            font-family: Verdana, Geneva, Tahoma, sans-serif;
            font-size: 300%;
        }
        p {
            color: black;
            font-family: 'Courier New', Courier, monospace;
            font-size: 160%;
        }
    </style>
</head>
<body>
    <h2>O que é o gambito da rainha?</h2>
    <p>Uma abertura em que você sacrifica uma peça para tirar vantagem disso depois.</p>
    <p>Uma abertura em que você sacrifica uma peça para tirar vantagem disso depois.</p>
    <p>Uma abertura em que você sacrifica uma peça para tirar vantagem disso depois.</p>
</body>
</html>

```

## ➜ CSS Border
Define uma borda em volta de um elemento HTML.

**📌 Exemplo:**

```css
p {
    border: 2px solid powderblue;
}

```

## ➜ CSS Padding

Define um espaço/preenchimento entre o texto e a borda.

**📌 Exemplo:**

```css
p {
    border: 2px solid powderblue;
    padding: 20px;
}

```

## ➜ CSS Margin

Define uma margem (espaço) fora da borda.

**📌 Exemplo:**

```css
p {
    border: 2px solid powderblue;
    margin: 40px;
}

```

## ➜ Link to External CSS
* Páginas de estilo externas podem ser referenciadas com um URL completo ou com um caminho relativo à página da web atual.

**📌 Exemplo:**

``` html
<link rel="stylesheet" href="https://www.w3schools.com/html/styles.css">

```

* Páginas de estilo podem estar em pastas distintas.

**📌 Exemplo:**

``` html
<link rel="stylesheet" href="/pasta a/a.css">

```

* Pode estar localizada na pasta atual.

**📌 Exemplo:**

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

