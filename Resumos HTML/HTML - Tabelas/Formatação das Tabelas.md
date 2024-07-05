# HTML Table Borders
* É possível colocar diferentes bordas e formas.


## How To Add a Border
* No CSS, utilize a propriedade `border` nos elementos `<table>`, `<th>`, e `<td>`.

**Exemplo**

``` html
<style>
    table, th, td {
        border: 1px solid black;
    }
</style>

```

## Collapsed Table Borders
* Para evitar bordas duplas, defina a propriedade `border-collapse` como `collapse`.

**Exemplo**

``` html
<style>
    table, th, td {
        border: 1px solid black;
        border-collapse: collapse;
    }
</style>

```

## Style Table Borders
* Defina uma cor de fundo para cada célula e dê à borda uma cor branca para criar a impressão de uma borda invisível.

**Exemplo**

``` html
<style>
    table, th, td {
        border: 1px solid white;
        border-collapse: collapse;
    }
    td, th {
        background-color: rgb(155, 241, 241);
    }
</style>

```

## Round Table Borders
* Utilize a propriedade `border-radius` para bordas arredondadas.

**Exemplo**

``` html
<style>
    table, th, td {
        border: 1px solid black;
        border-radius: 10px;
    }
</style>

```


* Para não arredondar as bordas de fora da tabela, remova o elemento table.

**Exemplo**

``` html
<style>
    th, td {
        border: 1px solid black;
        border-radius: 10px;
    }
</style>

```

## Dotted Table Borders
* Utilize a propriedade border-style com um dos valores abaixo:
* [Referência](https://www.w3schools.com/html/html_table_borders.asp)

|Valores |
| ------- |
|dotted   |    
|dashed   |   
|solid    | 
|double   | 
|groove   |  
|ridge    | 
|inset    | 
|outset   | 
|none     |
|hidden   |

**Exemplo**

``` html
<style>
        th, td{
            border-style:inset;
       
        }
        
    </style>

```

## Border Color
* Utilize a propriedade `border-color` para colorir uma borda:

``` html
<style>
    th, td {
        border: 1px solid;
        border-color: #d136aa;
    }
</style>
```

# HTML Table Sizes
Use o atributo `<style>` com as propriedades `width` ou `height` para especificar o tamanho de uma tabela, linha ou coluna.

**Exemplo**

``` html
<table style="width: 100%;">
    <tr>
        <th>Nome</th>
        <th>Idade</th>
        <th>Sexo</th>
    </tr>
    <tr>
        <td>Ana</td>
        <td>12</td>
        <td>F</td>
    </tr>
    <tr>
        <td>Carlos</td>
        <td>20</td>
        <td>M</td>
    </tr>
    <tr>
        <td>Clara</td>
        <td>15</td>
        <td>F</td>
    </tr>
</table>

```

## HTML Table Column Width
* Para definir o tamanho de uma coluna específica, adicione o atributo `style` em um elemento `<th> ` ou  `<td> `:

**Exemplo**

``` html
<table style="width: 100%;">
    <tr>
        <th style="width: 70%;">Nome</th>
        <th>Idade</th>
        <th>Sexo</th>
    </tr>
    <tr>
        <td>Ana</td>
        <td>12</td>
        <td>F</td>
    </tr>
    <tr>
        <td>Carlos</td>
        <td>20</td>
        <td>M</td>
    </tr>
    <tr>
        <td>Clara</td>
        <td>15</td>
        <td>F</td>
    </tr>
</table>
```

## HTML Table Row Height
* Para definir a altura de uma linha específica, adicione o atributo `style` em um elemento de linha da tabela.

**Exemplo**

``` html
 <table style="width: 100%;">
    <tr>
        <th style="width: 70%;">Nome</th>
        <th>Idade</th>
        <th>Sexo</th>
    </tr>
    <tr>
        <td style="height: 200px;">Ana</td>
        <td>12</td>
        <td>F</td>
    </tr>
    <tr>
        <td>Carlos</td>
        <td>20</td>
        <td>M</td>
    </tr>
    <tr>
        <td>Clara</td>
        <td>15</td>
        <td>F</td>
    </tr>
</table>
```

# HTML Table Headers
* Títulos nas tabelas são definidos por `<th>`.

**Exemplo de Tabela Completa**

``` html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="shortcut icon" href="/img/favicon (1).ico" type="image/x-icon">
    <style>
        table, td, th {
            border: 1px solid black;
            border-collapse: collapse;
        }
    </style>
</head>
<body>
    <h2>Cabeçalhos nas Tabelas</h2>
    <table style="width: 100%;">
        <tr>
            <th>Nome</th>
            <th>Cidade</th>
            <th>Idade</th>
        </tr>
        <tr>
            <td>Ana</td>
            <td>Saquarema</td>
            <td>18</td>
        </tr>
        <tr>
            <td>Pedro</td>
            <td>Rio de Janeiro</td>
            <td>25</td>
        </tr>
        <tr>
            <td>Carlos</td>
            <td>Rio das Ostras</td>
            <td>15</td>
        </tr>
    </table>
</body>
</html>

```

## Vertical Table Headers
* Utilize a primeira coluna como cabeçalho da tabela, definindo a primeira célula como um elemento `<th>`.

**Exemplo**

``` html
<table style="width: 100%;">
        <tr>
            <th>Nome</th>
            <td>Carlos</td>
            <td>Maria</td>
            <td>João</td>
        </tr>
        <tr>
            <th>Sexo</th>
            <td>M</td>
            <td>F</td>
            <td>M</td>
        </tr>
        <tr>
            <th>Idade</th>
            <td>12</td>
            <td>18</td>
            <td>13</td>
        </tr>
    </table>

 ```

## Align Table Headers
* Para alinhar,  utilize a propriedade `text-align`.

**Exemplo**

``` html
th {
    border: 1px solid black;
    border-collapse: collapse;
    text-align: center;
}

```

## Header for Multiple Columns
ara ter um cabeçalho com duas ou mais colunas, utilize o atributo `colspan` no elemento `<th>`.

**Exemplo**

``` html
<table style="width: 100%;">
    <tr>
        <th colspan="2">Nome e Cidade</th>
        <th>Idade</th>
    </tr>
    <tr>
        <td>Ana</td>
        <td>Saquarema</td>
        <td>18</td>
    </tr>
    <tr>
        <td>Pedro</td>
        <td>Rio de Janeiro</td>
        <td>25</td>
    </tr>
    <tr>
        <td>Carlos</td>
        <td>Rio das Ostras</td>
        <td>15</td>
    </tr>
</table>

```

## Table Caption
* Para adicionar uma legenda a uma tabela, use a tag `<caption>`.

**Exemplo**

``` html
<table style="width: 12%;">
    <caption>Dinheiro Mensal</caption>
    <tr>
        <th>Mês</th>
        <th>Renda</th>
    </tr>
    <tr>
        <td>Janeiro</td>
        <td>R$: 400</td>
    </tr>
    <tr>
        <td>Fevereiro</td>
        <td>R$: 500</td>
    </tr>
</table>

```

# HTML Table Padding & Spacing

## HTML Table - Cell Padding
* Padding: É o espaço entre as bordas e o conteúdo da célula.

**Exemplo**

``` html
th, td {
    padding: 15px;
}


```

* Para adicionar preenchimento apenas acima do conteúdo, use a propriedade `padding-top`.
E para os outros lados as propriedades `padding-bottom`, `padding-left` e `padding-right`:

**Exemplo**

``` html
th, td {
            padding-top: 10px;
            padding-left: 10px;
            padding-bottom: 40px;
        }

```

## HTML Table - Cell Spacing
* O espaçamento entre células é o espaço entre cada célula. Por padrão, o espaço é definido como 2 pixels.
* Para alterar o espaço entre as células da tabela, use a propriedade CSS border-spacing no elemento table.

**Exemplo**

``` html
table {
    border-spacing: 20px;
}


```

# HTML Table Colspan & Rowspan

## HTML Table - Colspan
* Para fazer uma célula abranger várias colunas, use o atributo `colspan`:

**Exemplo**

``` html
<table style="width: 30%;">
    <tr>
        <th colspan="2">Nome</th>
        <th>Idade</th>
    </tr>
    <tr>
        <td>Ana</td>
        <td>Toledo</td>
        <td>12</td>
    </tr>
    <tr>
        <td>Carlos</td>
        <td>Madureira</td>
        <td>10</td>
    </tr>
</table>

```

## HTML Table - Rowspan
* Para fazer uma célula abranger várias linhas, use o atributo `rowspan`.

**Exemplo**

``` html
<table style="width: 30%;">
    <tr>
        <th>Nome</th>
        <td>Carlos Henrique</td>
    </tr>
    <tr>
        <th rowspan="2">Contato(s)</th>
        <td>22233-2212</td>
    </tr>
    <tr>
        <td>2223233-2212</td>
    </tr>
</table>


```

