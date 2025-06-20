## Declaração if

Declarações compostas em Python contêm (grupos de) outras declarações; elas afetam ou controlam a execução dessas outras declarações de alguma maneira.

Talvez o tipo de declaração mais conhecido seja a declaração `if`. A palavra-chave `if` é usada para formar uma declaração condicional que executa algum código especificado após verificar se sua expressão é `True`. Python usa recuo para definir blocos de código:

```python
if value > 1000: 
    print("É um número grande!")  # Bloco recuado
    a += 1                          # Bloco recuado
    
print("Fora do bloco!")        
```

Um bloco de código começa com recuo e termina com a primeira linha não recuada. A quantidade de recuo deve ser consistente em todo o bloco. Geralmente, quatro espaços em branco ou abas únicas são usadas para recuo.
Recuo incorreto resultará em `IndentationError`.

Se você tem apenas uma declaração para executar, você pode colocá-la na mesma linha que a declaração `if`.

```python
if a > b: print("a é maior que b")
```

Para obter informações mais estruturadas e detalhadas, você pode se referir a [esta página do banco de conhecimento Hyperskill](https://hyperskill.org/learn/step/5953?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
Imprima `"Não é uma lista vazia!"` se a lista `tasks` não estiver vazia.
Após a lista ser limpa, verifique novamente (você pode precisar de uma condição diferente!) e imprima `'Agora vazia!'` se estiver.

<div class='hint'>Use a função <code>len()</code> para verificar se <code>tasks</code> está vazia.</div>