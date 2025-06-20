## Recursão

A palavra <b>recursão</b> vem do latim <i>recurrere</i>, significando retornar, reverter ou recorrer.
Na programação, recursão se refere a uma técnica de codificação na qual uma função chama a si mesma.

Na maioria dos casos, a recursão não é necessária, mas em algumas situações, a definição auto-referencial
é justificada. Percorrendo [estruturas de dados semelhantes a árvores](https://en.wikipedia.org/wiki/Tree_(data_structure)), seriam um bom exemplo.
Essas estruturas são [aninhadas](course://Data structures/Nested Lists), e se encaixam prontamente numa definição recursiva. Um algoritmo não-recursivo
para a mesma tarefa seria bastante complicado.

Aqui está um exemplo simples de uma função recursiva. Ela recebe um número como um argumento
e imprime os números do argumento especificado até chegar a zero. Na chamada recursiva,
o argumento é um a menos que o valor atual de `n`, então cada recursão se aproxima  
do caso base (que é zero).

```python
def contagem_regressiva(n):
    print(n, end=' ')
    if n == 0:
        return             # Termina a recursão
    else:
        contagem_regressiva(n - 1)   # Chamada recursiva


contagem_regressiva(4)
```
```text
4 3 2 1 0 
```

<div class="hint">Esta função não verifica a validade do seu argumento: se <code>n</code> 
for um não-inteiro ou negativo, você receberá uma exceção <a href="https://docs.python.org/3/library/exceptions.html?highlight=recursionerror#RecursionError"><code>RecursionError</code></a>, pois o caso base nunca é atingido:

```python
contagem_regressiva(-10)
```
```text
RecursionError: a profundidade máxima de recursão excedida durante a chamada de um objeto Python
```
Você pode descobrir qual é o limite de recursão do Python com uma função do módulo sys 
chamada [`getrecursionlimit()`](https://docs.python.org/3/library/sys.html#sys.getrecursionlimit), e você pode alterá-lo com [`setrecursionlimit()`](https://docs.python.org/3/library/sys.html#sys.setrecursionlimit):

```python
from sys import setrecursionlimit
setrecursionlimit(3000)
getrecursionlimit()
```
```text
3000
```
</div>

Lembre-se que a recursão não é útil em todas as situações. Para alguns problemas, uma solução recursiva, embora 
possível, será desconfortável em vez de elegante. Implementações recursivas muitas vezes consomem mais 
memória do que as não-recursivas e, em alguns casos, podem resultar em execução mais lenta.

Para obter informações mais estruturadas e detalhadas, você pode se referir a [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/7665?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
No editor de código, implemente uma função recursiva que calcule o [fatorial](https://en.wikipedia.org/wiki/Factorial) de um número inteiro positivo.
Para 1 e 0 retorna 1, para qualquer outro número calcula o produto desse número (`n`) e
o fatorial do número anterior (`n-1`).

<div class="hint">Não se esqueça da chamada da função recursiva.</div>
