## Else com loops 2

Este tipo de `else` é útil apenas se houver uma condição `if` presente dentro do loop, que de alguma forma depende da variável do loop.
Vamos olhar mais uma vez para o exemplo da tarefa anterior:

```python
for n in range(2, 10):
    for x in range(2, n):
        if n % x == 0:
            print(n, 'é igual a', x, '*', n//x)
            break
    else:
        # o loop terminou sem encontrar um fator
        print(n, 'é um número primo')
```

A instrução `else` será executada apenas se `n` for um número primo, ou seja, a instrução `if` não foi executada para nenhuma iteração do loop interno `for`.

### Tarefa
Dentro da [função](course://Loops/Else com loops 2) `contains_even_number()`, escreva um loop `for` que percorreria uma lista `lst` e, se um elemento par for encontrado,
imprima `f"A lista {lst} contém um número par."` e saia do loop, se tal elemento não for encontrado, imprima `f"A lista {lst} não contém um número par."`.

<div class="hint">

Você pode usar `if i % 2 == 0:` para testar se um número dado é par.
</div>

<div class="hint">

Use a instrução `break` para sair do loop se um número par for encontrado.
</div>

<div class="hint">

Use uma cláusula `else` para imprimir `f"A lista {lst} não contém um número par."`.
</div>