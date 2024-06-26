# HTML - Parte 1

📌 Site utilizado para estudo: [w3schools](https://www.w3schools.com/html/default.asp)

## O que é HTML? 
- Uma linguagem de marcação que descreve a estrutura de uma página web.
Exemplo:

``` html
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```
## 📚 Comandos 

| Comando | Função |
|---------| -------|
| h1, h2, h3 | Título |
| p | Parágrafo |
| br | Pula linha|
| a | Links |
| img | Imagem |
| hr  | Quebra de linha horizontal |
| pre | Define texto pré-formado |
| background-color | Mudar a cor do backgroud da página |
| color | Textos coloridos |
| font-family | Fontes nos textos |
| font-size | Tamanho do texto |
| text-align | Alinhar texto |



**Exemplos:**

-> Ex 1: Utilizando a tag <a>:
``` html
<a href="https://www.w3schools.com">This is a link</a>
```
-> Ex 2: Utilizando a tag <img> para colocar imagens:
``` html
<img src="w3schools.jpg" alt="Texto alternativo" width = "104" height = "142" <img>
<img src="imagem.jpg">
```  
* Pode-se utilizar um link externo de outro site.
* width: largura | height: altura.

## 🔎 Estrutura HTML
![a](https://pensandonaweb.com.br/content/images/2014/Aug/html-hierarchy.png)

## 🎨 Style
* Para Adicionar cores, fontes, tamanhos das fontes.
Sintaxe:
``` html
<tagname style="property:value;">
```
-> Ex 3: Mudando a cor do parágrafo:
``` html
<p style="color:red;" > Este é um parágrafo vermelho. </p>
```
-> Ex 4: Aumentando a fonte de um título: 
``` html
<h1 style="font-size:60px;">Título 1</h1>
```

### 🍄 Background Color
* Propriedade para definir cor de fundo. 

-> Ex 4.1: Mudando a cor do corpo do site:
``` html
<body style="background-color: powderblue;">
    <h1>Olá mundo! Esse é um título. </h1>
    <p>Esse é um parágrafo.</p>
    
</body>
```

-> Ex 4.2: Mudando a cor de diversos elementos:
``` html
<body style="background-color: powderblue;">
    <h1 style="background-color: blueviolet;">Olá mundo! Esse é um título. </h1>
    <p style="background-color: brown;">Esse é um parágrafo.</p>
    
</body>
```
### 🍄 Text Color
* Propriedade para definir a cor de um elemento.
* **Color**

-> Ex 4.3: Mudando a cor da fonte: 
``` html
<body style="color: powderblue;">
    <h1 style="color: blueviolet;">Olá mundo! Esse é um título. </h1>
    <p style="color: brown;">Esse é um parágrafo.</p>   
</body>
``` 

### 🍄 Fonts 
* Propriedade para definir as fontes de um texto: 
* **font-family**

-> Ex 4.3: Mudando a fonte do texto:
``` html
<h1 style="font-family: 'Courier New', Courier, monospace;">Olá1</h1>
```

### 🍄 Font-size
* Propriedade para alterar o tamanho de uma fonte:
* **font-size**

-> Ex 4.4: Mudando tamanho da fonte e mudando a cor:
``` html
<p style="font-size: 300%; color: black;">Defesa Civil</p>
``` 

### 🍄 Text Alignment
* Alinhando os elementos no centro. 
* **text-align: center**

-> Ex 4.5: Alinhando texto ao centro:
``` html
<h1 style="text-align: center;">Alinhando ao centro.</h1>
```

## 📒 Title
* Um atributo extra que permite mais informações sobre um elemento.

-> Ex 5: 
``` html
<h2 title="Eu sou um palhaço">Este é um parágrafo.</h2>
``` 

## 📕 Parágrafos
* Representado pela tag: <p> 
* Para quebra de linhas utilize: </br>
* Para quebra de linhas horizontais utilize: <hr>
* Para preservar linhas e quebra de linhas utilize: <pre>

-> Ex 6: Definindo uma quebra de linha horizontal com a tag <hr>: 

``` html
    <h1> Olá mundo </h1>
    <p> Oi Mundo </p>
    <hr>
    <h2> Olá Brasil </h2>
    <p> Eae brasil </p>
    <hr>
``` 

-> Ex 7: Fazendo um poema com a tag <pre>:
``` html
    <pre>
        Todos esses que aí estão
        Atravancando meu caminho,
        Eles passarão...
        Eu passarinho!
    </pre>

```


##  📏 HTML Formatting

## 📚 Comandos para Formatação
``` html
| Comando | Função |
|---------|---------|
| b | Negrito |
| <strong> | Texto importante |
| <i> | Itálico |
| <em> | Texto enfatizado |
| <mark> | Texto marcado |
| <small> | Texto pequeno |
| <del> | Risca texto |
| <ins> | Texto grifado abaixo |
| <sub> | Texto subscrito |
| <sup> | Texto sobrescrito |
``` 

