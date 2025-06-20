## Compreensão de Listas

Você pode usar um loop para construir uma lista (ou outra estrutura de dados).
Por exemplo:

```python
minha_lista = []
for i in range(5):
    minha_lista.append(i)

print(minha_lista)
```
Saída:
```text
[0, 1, 2, 3, 4]
```

Isso é legal, mas bastante volumoso. A compreensão de listas oferece uma sintaxe mais compacta quando você deseja criar uma nova lista com base nos valores de uma lista existente
ou outro iterável (tupla, string, array, range, etc.). Ele realiza a mesma tarefa e simplifica o programa. Normalmente, as compreensões de lista são escritas em uma única linha de código.

```python
minha_lista = [i for i in range(5)]
print(minha_lista)
```
Saída:
```text
[0, 1, 2, 3, 4]
```
As compreensões de lista também são mais eficientes computacionalmente do que um loop `for`.

Para obter informações mais estruturadas e detalhadas, você pode consultar [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/6315?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
No editor de código, use a compreensão de lista para construir `minha_lista_eficiente` a partir dos elementos de `minha_lista_ineficiente`
adicionando $10$ a cada um deles. Por exemplo, o primeiro elemento de `minha_lista_ineficiente` é $1 + 10 = 11$,
então o primeiro elemento de `minha_lista_eficiente` deve ser $11 + 10 = 21$, e assim por diante.

<div class="hint">

No exemplo acima, nós usamos `i para i in range(5)`. Você pode modificar `i` como quiser 
diretamente nesta expressão. Por exemplo, para subtrair `5` de cada `i`, você pode fazer 
`i - 5 for i in range(5)`.
</div>