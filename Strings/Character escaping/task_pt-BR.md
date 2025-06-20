## Escapando caracteres

A barra invertida é usada para escapar símbolos especiais, como aspas simples ou duplas,
por exemplo, `"It\'s me"` ou `"She said \"Hello\""`. Se você precisar realmente digitar o caractere <code>\\</code>
como parte da sua string, você também precisará escapá-lo. Por exemplo, aqui está como 
você imprime uma única barra invertida:

```python
print('\\')
```

O símbolo especial `'\n'` é usado para adicionar uma quebra de linha a uma string, enquanto `'\t'` significa tabulação.

As aspas têm significados especiais, e elas também podem ser escapadas com uma barra invertida. Se você precisar imprimir aspas dentro de uma string, use um tipo diferente de aspas: as aspas simples podem ser usadas em uma string com aspas duplas sem a necessidade de escapá-las, e vice-versa. Além disso, como nota adicional, é uma boa ideia escolher seu tipo favorito de aspas e usá-las de maneira consistente.

Você pode aprender mais sobre a fuga de caracteres nesta <a href="https://docs.python.org/3/reference/lexical_analysis.html#string-and-bytes-literals">seção</a> da Documentação Python.

Para informações mais estruturadas e detalhadas, você também pode se referir a [esta página de base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/7130?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
Imprima o seguinte texto usando uma string:
```text
The name of this ice cream is "Sweet'n'Tasty"  
```

<div class='hint'>Use a barra invertida para escapar as aspas.</div>