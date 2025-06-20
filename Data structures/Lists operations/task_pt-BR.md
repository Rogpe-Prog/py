## Operações com listas

Ao contrário das strings, as listas são um tipo mutável, ou seja, é possível
mudar o conteúdo delas usando `lst[indice] = novo_item`.

```python
cubes = [1, 8, 27, 65, 125]  # algo está errado aqui
4 ** 3  # o cubo de 4 é 64, não 65!
```
```text
64
```
```python
cubes[3] = 64  # substitui o valor errado
cubes
```
```text
[1, 8, 27, 64, 125]
```

Você pode adicionar novos itens no final da lista usando o método `append()` ou 
concatenação de listas. 

```python
squares = [1, 4, 9, 16, 25]
squares.append(6**2)
squares
```
```text
[1, 4, 9, 16, 25, 36]
```

Descubra sobre muitos outros métodos de lista úteis nesta <a href="https://docs.python.org/3/tutorial/datastructures.html#more-on-lists">página</a>.

Para informações mais estruturadas e detalhadas, você também pode consultar [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/6031?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
Substitua `"dino"` por `"dinossauro"` na lista `animals`.
<div class='hint'>Use a operação de indexação da lista e atribuição de valor.</div>