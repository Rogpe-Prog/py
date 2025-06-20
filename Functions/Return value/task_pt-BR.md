## Valor de retorno

As funções podem retornar um valor ao chamador, usando a palavra-chave `return`. Você pode usar o
valor retornado para atribuí-lo a uma variável ou apenas imprimi-lo. Na verdade, até as funções
sem uma declaração `return` retornam um valor. Esse valor é 
chamado `None` (é um nome integrado). Escrever o valor `None` é normalmente suprimido pelo
interpretador, mas se você realmente quiser vê-lo, pode usar `print(some_func())`.

Para obter informações mais estruturadas e detalhadas, você pode se referir a [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/5900#execution-and-return?utm_source=jba&utm_medium=jba_courses_links).

><i>O primeiro comando do corpo da função pode opcionalmente ser uma string literal; esta string
literal é a string de documentação da função, ou docstring (mais sobre docstrings pode
ser encontrado na seção <a href="https://docs.python.org/3/tutorial/controlflow.html#tut-docstrings">Strings de Documentação</a>
na Documentação do Python). É uma boa prática incluir docstrings no código que você escreve.</i>
  
Na [sequência Fibonacci](https://en.wikipedia.org/wiki/Fibonacci_number), os dois primeiros números são `1` e `1` (às vezes, porém, eles são `0` e `1` ou `1` e `2`), e cada número subsequente
é a soma dos dois anteriores. 

### Tarefa
Escreva uma função que retorna uma lista de números
da sequência Fibonacci até `n`.  

<div class='hint'>Inicialize <code>b</code> com 1.</div>
<div class='hint'>Atualize <code>b</code> com <code>a + b</code>.</div>
<div class='hint'>Atualize <code>a</code> com <code>tmp_var</code>.</div>
