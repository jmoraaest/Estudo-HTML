# HTML Parte 2

## 📚 Comandos

| Comando | Função |
|---------|--------|
| blockquote | Identa os elementos |
| q | Citação curta com aspas |
| abbr | Abreviação |
| cite | Define um título para um trabalho |
| adress | Define um contato para o documento |


## 🖋 Elementos de Cotação e Citação 

### 📌HTML blockquote for Quotations
* O elemento blockquote define uma seção citada de outra fonte. Além disso identa um elemento:

-> Ex 1: **Resultado na página:**
``` markdown
Isto é uma citação do website:

    Aleister Crowley é extremamente claro ao afirmar que o Anjo da Guarda não deve ser  confundido com entidades nebulosas como o Eu Superior. 
    Diz ainda que o Anjo da Guarda é um indivíduo real, 
    com seu próprio universo, assim como os seres humanos.
    O Santo Anjo da Guarda não é uma entidade subjetiva, 
    nem consiste numa forma de "oposto da consciência" da pessoa

``` 

-> **Código:**
``` html
<body>
    <h1 style="color: rgb(150, 1, 113); text-align: center;">Elementos de citação, Cotação</h1>
    <p>- Isto é uma citação do website:</p>
    <blockquote cite="https://www.projetomayhem.com.br/sagrado-anjo-guardião">
        Aleister Crowley é extremamente claro ao afirmar que o Anjo da Guarda não deve ser confundido com entidades nebulosas como o Eu Superior. Diz ainda que o Anjo da Guarda é um indivíduo real, com seu próprio universo, assim como os seres humanos.
        O Santo Anjo da Guarda não é uma entidade subjetiva, nem consiste numa forma de "oposto da consciência" da pessoa
    </blockquote>
</body>

```
### 📌 q for Short Quotations
* Esta é uma citação curta e os navegadores geralmente colocam aspas:

-> Ex 2: **Resultado na página:**
``` html

``` markdown
Olá Júlia, Tudo bem? "O bem e o mal são relativos..."

```

-> **Código:**
``` html
<p> Olá Júlia, Tudo bem? <q>O bem e o mal são relativos... </q></p>

``` 

### 📌 abbr for Abbreviations
* Utilizamos para fazer abreviações:

-> Ex 3:
``` html
<p> Abc...<abbr title="World Health Organization">Who</abbr>was founded in 1948.</p>

```

## 💭 Comentários
* Para criar comentários curtos utilize: 

``` html 
<!-- Write your comments here -->

```

* Para comentários longos utilize:

``` html
<!--
<p>Look at this cool image:</p>
<img border="0" src="pic_trulli.jpg" alt="Trulli">
-->

```

## 🌈 HTML Colors


### ⭐Funcionalidades básicas

[Lista de cores disponíveis](https://www.w3schools.com/colors/colors_names.asp)

| Comando | Função |
| ------ | ------- |
| color | Para mudar a cor da fonte |
| background-color | Para mudar a cor de fundo |
| border | Para colocar bordas coloridas |

