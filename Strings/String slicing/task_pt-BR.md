## Fatiamento

O fatiamento é usado para extrair vários caracteres (uma substring) de uma string.
Sua sintaxe é semelhante à da indexação, mas em vez de usar apenas um índice, você usa
dois índices (números) separados por dois pontos, por exemplo, `str[ind1:ind2]`. Estes dois
índices correspondem ao início e ao fim da substring. Note que o símbolo
com o índice `ind1` será incluído, enquanto o símbolo com o índice `ind2` – não será.

Aqui está uma visualização de como o fatiamento funciona no Python:

```text
+---+---+---+---+---+---+
| P | y | t | h | o | n |
+---+---+---+---+---+---+
0   1   2   3   4   5   6
-6  -5  -4  -3  -2  -1
```

##### Exemplo
<pre><code>
str[inicio:fim] # itens de início a fim-1
str[inicio:]    # itens de início até o resto do array
str[:fim]       # itens do início até fim-1
str[:]          # uma cópia de todo o array
</code></pre>

Para informações mais estruturadas e detalhadas, você pode se referir a [esta página da base de conhecimento Hyperskill](https://hyperskill.org/learn/step/6177?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
Use o fatiamento para obter `"Python"` da variável `monty_python`.  

<div class='hint'>Você pode deixar um dos índices vazio.</div>