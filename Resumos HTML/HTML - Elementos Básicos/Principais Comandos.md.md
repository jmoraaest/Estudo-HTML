# 💻 Comandos Básicos HTML

## ➜ Principais Comandos HTML

| Comando           | Função                      |
|-------------------|-----------------------------|
| `h1, h2, h3`      | Títulos                     |
| `p`               | Parágrafos                  |
| `br`              | Quebra de linha             |
| `a`               | Links                       |
| `img`             | Imagens                     |
| `hr`              | Linha horizontal            |
| `pre`             | Texto pré-formatado         |

### 📌 Exemplos

- **Títulos (h1, h2, h3, ...)**: Usados para definir cabeçalhos de diferentes níveis. O `h1` é o título principal e `h6` é o menos importante.
  
```html
<h1>Este é um título de nível 1</h1>
<h2>Este é um título de nível 2</h2>
<h3>Este é um título de nível 3</h3>

```

* **Parágrafos (p)**: Usados para definir blocos de texto.

``` html
<p>Este é um parágrafo.</p>

```

- **Quebra de linha (br)**: Insere uma quebra de linha dentro de um parágrafo ou texto.

```html
<p>Este é um parágrafo.<br>Esta é uma nova linha dentro do mesmo parágrafo.</p>

```

- **Links (a)**: Cria um hiperlink para outra página ou recurso.

```html
<a href="https://www.w3schools.com">Este é um link</a>

```

- **Imagens (img)**: Insere uma imagem na página.

```html
<img src="w3schools.jpg" alt="Texto alternativo" width="104" height="142">

```
    * Pode-se utilizar um link externo para a imagem.
    * `width` define a largura e `height` define a altura da imagem.

- **Linha horizontal (hr)**: Insere uma linha horizontal para separar conteúdos.

```html
<hr>

```

- **Texto pré-formatado (pre)**: Preserva espaços em branco e quebras de linha, exibindo o texto exatamente como foi digitado.

```html
<pre>
    Este texto
    será exibido
    exatamente assim.
</pre>

```
## 📚 Comandos para Formatação

| Comando | Função |
| --- | --- |
| b | Negrito |
| strong | Texto importante |
| i | Itálico |
| em | Texto enfatizado |
| mark | Texto marcado |
| small | Texto pequeno |
| del | Texto riscado |
| ins | Texto sublinhado |
| sub | Texto subscrito |
| sup | Texto sobrescrito |

## 🔎 Estrutura HTML
![a](https://pensandonaweb.com.br/content/images/2014/Aug/html-hierarchy.png)

1. **`<!DOCTYPE html>`**: Declara o tipo do documento, indicando que é um documento HTML5.
2. **`<html>`**: A tag raiz que envolve todo o conteúdo da página.
3. **`<head>`**: Contém metadados sobre o documento, como o título e links para folhas de estilo.
4. **`<title>`**: Define o título da página, que aparece na aba do navegador.
5. **`<body>`**: Contém todo o conteúdo visível da página, como textos, imagens e links.
