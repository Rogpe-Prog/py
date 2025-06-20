## Chaves de dicionário keys() e valores()

Existem muitos métodos úteis em dicionários, como `keys()`, `values()` e `items()`.
O método `keys()` retorna um objeto de visualização que exibe uma lista de todas as chaves no dicionário em ordem de inserção.
`values()` retorna uma nova visualização dos valores do dicionário. Quando o método `items()` é chamado,
retorna uma nova visualização dos itens do dicionário como tuplas em uma lista (pares `(chave, valor)`).

Os objetos retornados por `dict.keys()`, `dict.values()`, e `dict.items()` fornecem uma 
visão dinâmica das entradas do dicionário, o que significa
que quando o dicionário muda, a visualização reflete essas mudanças.

Você pode explorar o resto usando &shortcut:CodeCompletion; após `nome_dict` 
seguido por um ponto.

Leia mais sobre as operações que os dicionários suportam <a href="https://docs.python.org/3/library/stdtypes.html#typesmapping">aqui</a>.

Para obter informações mais estruturadas e detalhadas, você também pode se referir a [esta página da base de conhecimento Hyperskill](https://hyperskill.org/learn/step/11096?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
Imprima todos os valores do `phone_book`.

<div class='hint'>Use o método <code>values()</code>.</div>