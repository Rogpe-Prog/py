## Compreensão de Listas Aninhadas

Compreensões de listas aninhadas são simplesmente compreensões de listas aninhadas dentro de outras
compreensões de listas. Isso é bastante semelhante a [loops aninhados](course://Loops/Loop aninhado).
Aqui está um programa que cria uma [lista aninhada](course://Estruturas de dados/Listas Aninhadas) usando um loop aninhado:

```python
matrix = []

for i in range(3):

    # Anexar uma sublista vazia dentro da lista
    matrix.append([])

    for j in range(0, 10, 2):
        matrix[i].append(j)

print(matrix)
```
Saída:
```text
[[0, 2, 4, 6, 8], [0, 2, 4, 6, 8], [0, 2, 4, 6, 8]]
```

O mesmo pode ser feito em apenas uma linha usando a compreensão de listas aninhadas:

```python
matrix = [[j for j in range(0, 10, 2)] for i in range(3)]
print(matrix)
```
Saída:
```text
[[0, 2, 4, 6, 8], [0, 2, 4, 6, 8], [0, 2, 4, 6, 8]]
```

Para obter informações mais estruturadas e detalhadas, você pode se referir a [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/6938#nested-list-comprehension?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa

Crie uma `matrix` $10×10$ de tal forma que cada linha (sublista) contenha **caracteres** 0–9 de
`string`. Use a compreensão de lista para completar a tarefa em uma linha de código.

<div class="hint">

Siga o exemplo na descrição da tarefa. Você simplesmente precisa usar `string` como um iterável ao invés
de um dos ranges.

</div>