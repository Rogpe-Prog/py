## Listas Aninhadas

Uma lista pode conter qualquer tipo de objeto, até mesmo outras listas (sublistas). Essa 
estrutura de dados é conhecida como lista aninhada.

Você pode usar listas aninhadas para organizar os dados em estruturas hierárquicas.

Uma lista aninhada pode ser criada ao escrever uma sequência separada por vírgulas de sublistas:

```python
lista_aninhada = [[1, 2, 3], [4, 5], 6]
```

Você pode acessar itens em uma lista aninhada usando índices como antes:

```python
print(lista_aninhada[1])
print(lista_aninhada[2])
```
Resultado:
```text
[4, 5]
6
```
Você pode acessar itens dentro de sublistas em uma lista aninhada usando vários índices.
Para acessar o número `1` de `lista_aninhada`, use o índice `0` duas vezes. Primeiro, você acessa o elemento `[1,2,3]` e então, o primeiro elemento dessa sublista:
```python
print(lista_aninhada[0][0])
```
Resultado:
```text
1
```
Para informações mais estruturadas e detalhadas, você pode se referir a [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/6938?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
No editor de código, use indexação para acessar e imprimir os elementos `9` e `10` da lista aninhada `minha_lista`. 

<div class="hint">Se você estiver preso, revise os exemplos na descrição da tarefa novamente.</div>