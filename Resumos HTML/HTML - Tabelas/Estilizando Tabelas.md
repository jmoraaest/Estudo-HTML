# HTML Table Styling

## HTML Table - Zebra Stripes
* Adicione uma cor de fundo a cada duas linhas da tabela para obter um efeito de listras.
* Utilize `:nth-child(even)` para estilizar as linhas pares.
* Utilize `:nth-child(odd)` para estilizar as linhas ímpares.

**Exemplo:**

```html
tr:nth-child(even) {
    background-color: #D6EEEE;
}

```

## HTML Table - Vertical Zebra Stripes
* Para fazer listras verticais de zebra, estilize colunas alternadas, em vez de linhas alternadas.

**Exemplo**
``` html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
       table, th, td {
           border: 1px solid black;
           border-collapse: collapse;
       }

       th:nth-child(even), td:nth-child(even) {
           background-color: #D6EEEE;
       }
    </style>
</head>
<body>
    <table>
        <tr>
            <th>Mês</th>
            <th>Renda</th>
        </tr>
        <tr>
            <td>Janeiro</td>
            <td>R$:400</td>
        </tr>
        <tr>
            <td>Fevereiro</td>
            <td>R$: 500</td>
        </tr>
        <tr>
            <td>Março</td>
            <td>R$: 1500</td>
        </tr>
        <tr>
            <td>Abril</td>
            <td>R$: 1600</td>
        </tr>
    </table>
</body>
</html>
```

## Horizontal Dividers
* Adicione `border-bottom` na propriedade `tr` para criar divisões horizontais.

**Exemplo**

``` html
<style>
    table {
        border-collapse: collapse;
    }
    tr {
        border-bottom: 1px solid #ddd;
    }
</style>

```

## Hoverable Table
* Adicione um efeito de hover nas linhas da tabela para destacar quando o mouse passar sobre elas.

``` html
<table>
    <style>
        table {
            border-collapse: collapse;
            width: 100%;
        }

        th, td {
            padding: 8px;
            text-align: left;
            border-bottom: 1px solid #DDD;
        }

        tr:hover {
            background-color: #D6EEEE;
        }
    </style>
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

}

