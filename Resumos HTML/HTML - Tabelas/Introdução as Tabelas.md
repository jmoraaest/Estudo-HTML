
# HTML Tables

| Comando | Função | 
|---------|--------|
| `<table>` | Define a tabela|
| `<td>`| Define uma célula |
| `<tr>` | Define uma linha|
| `<th>` | Cabeçalho |

## ➜ Define an HTML Table
* Uma tabela em HTML consiste em células de tabela dentro de linhas e colunas.

**📌 Exemplo de tabela simples**

``` html
<table>
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
        <tr>
            <td>Clara</td>
            <td>15</td>
            <td>F</td>
        </tr>
        </tr>
    </table>
    
```

## ➜ Table Cells
* Cada célula da tabela é definida por uma tag `<td>`;
* Tudo entre <td> e </td> é o conteúdo da célula da tabela.

**📌 Exemplo**

``` html
<body>
    <table>
        <tr>
            <td>Nome</td>
            <td>Idade</td>
            <td>Sexo</td>
        </tr>
    </table>
</body>

```

## ➜ Table Rows (Row - Linha)
* Cada linha da tabela começa e termina com uma tag `<tr>`;
* Significa linha da tabela (`<tr>`).

**📌 Exemplo**

``` html
<body>
    <table>
        <tr>
            <td>Clara</td>
            <td>Ana</td>
            <td>Pedro</td>
        </tr>
        <tr>
            <td>12</td>
            <td>18</td>
            <td>20</td>
        </tr>
        <tr>
            <td>F</td>
            <td>F</td>
            <td>M</td>
        </tr>
    </table>
</body>

```

## ➜ Table Headers
* Quando você precisar que certas células sejam de cabeçalho, utilize `<th>`.

**📌 Exemplo**

``` html
<tr>
            <th>Pessoa 1</th>
            <th>Pessoa 2</th>
            <th>Pessoa 3</th>
        </tr>

```
