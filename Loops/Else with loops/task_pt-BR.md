## Else com loops

Vimos que a declaração `break` sai do loop `for` ou `while` mais interno.

Python também permite que as instruções de loop tenham uma cláusula `else`. É executada quando o loop termina
por exaustão do iterável (com `for`) ou quando a condição se torna `False`
(com `while`), mas não quando o loop é terminado por uma declaração `break`. Confira
este exemplo de um loop que busca por números primos:

```python
for n in range(2, 10):
    for x in range(2, n):
        if n % x == 0:
            print(n, 'igual a', x, '*', n//x)
            break
    else:
        # loop caiu porque não encontrou um fator
        print(n, 'é um número primo')
```
```text
2 é um número primo
3 é um número primo
4 igual a 2 * 2
5 é um número primo
6 igual a 2 * 3
7 é um número primo
8 igual a 2 * 4
9 igual a 3 * 3
```
Nesse código, a cláusula `else` pertence ao loop `for`, não à
declaração `if`.

Lembre-se, um `else` após uma declaração `if` é pulado e NÃO executado se a expressão seguinte a 
`if` é `True`, enquanto no caso de loops, uma cláusula `else` é executada após o próprio loop
ser completado (a menos que houvesse um `break` em algum lugar).

Para informações mais estruturadas e detalhadas, você pode se referir a [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/6302?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
No editor de código, adicione duas linhas de código ao segundo loop para garantir que o loop imprima apenas
os números 1 e 2 e nunca imprima a frase `"for loop is done"`.

<div class="hint">Deve terminar no número 3.</div>