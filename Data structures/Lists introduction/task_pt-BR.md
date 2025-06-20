## Introdução às listas

O Python tem vários tipos de dados compostos usados para agrupar dados. 
O mais versátil é a lista, que pode ser escrita como uma série de valores 
separados por vírgulas (itens) fechados em colchetes, por exemplo, `lst = [item1, item2]`. 
As listas podem conter itens de diferentes tipos, mas geralmente todos os itens em uma lista 
são do mesmo tipo. Como strings, as listas podem ser indexadas e fatiadas (veja [Lição 3](course://Strings/String slicing)).
Todas as operações de fatiamento retornam uma nova lista contendo os elementos solicitados.

As listas também suportam operações como concatenação:

```python
squares = [1, 4, 9, 16, 25]
squares + [36, 49, 64, 81, 100]
[1, 4, 9, 16, 25, 36, 49, 64, 81, 100]
```

Você pode explorar mais detalhadamente as listas lendo <a href="https://docs.python.org/3.9/tutorial/introduction.html#lists">esta página</a>.

Para obter informações mais estruturadas e detalhadas, você também pode se referir a [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/5979?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
Use o fatiamento de lista para imprimir `[4, 9, 16]`.  

<div class='hint'>A sintaxe de fatiamento de lista se parece exatamente com a das strings: <code>lst[index1:index2]</code>.
Não se esqueça de que o elemento com o índice <code>index2</code> não está incluído!</div>