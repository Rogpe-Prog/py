## Operadores aritméticos

Assim como em qualquer outra linguagem de programação, os operadores de adição ( `+` ), subtração ( `-` ),
multiplicação ( `*` ) e divisão ( `/` ) podem ser usados com números. Além disso, 
o Python possui os operadores de potência ( `**` ), módulo ( `%` ) e divisão de piso ( `//` ).

- O operador `*` (multiplicação) produz o produto dos argumentos. Os argumentos devem
ser ambos números, ou um argumento deve ser um número inteiro e o outro - uma sequência.
  
- Os operadores `/` (divisão) e `//` (divisão de piso) produzem o quociente de seus argumentos.
  A divisão de números inteiros produz um número flutuante, enquanto a divisão de piso de números inteiros resulta em um número inteiro.
  
- O operador `%` (módulo) produz o resto da divisão do primeiro argumento pelo segundo.

- O operador `+` (adição) produz a soma dos argumentos. Os argumentos devem ser ambos
  números ou ambos serem sequências do mesmo tipo.
  
- O operador `-` (subtração) produz a diferença de seus argumentos.

Por exemplo
```python
a = 16
b = 3
result = a // b  # o resultado será 5
result = a % b   # o resultado será 1
result = a ** 2  # o resultado será 256 (16 elevado a 2)
```

As operações aritméticas binárias têm os níveis de prioridade convencionais. Note que
algumas dessas operações também se aplicam a certos tipos não numéricos.

Você pode ler mais sobre este tópico <a href="https://docs.python.org/3/reference/expressions.html#binary-arithmetic-operations">aqui</a>.

Para informações mais estruturadas e detalhadas, você também pode se referir a [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/5865?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
 - Divida o valor armazenado em `init_number` por `2`.
 - Calcule o resto dessa divisão.
 - Multiplique o `division_result` por `2`.
 - Adicione o `division_remainder` ao `multiplication_result`.
 - Subtraia o `multiplication_result` de `init_number`.
 - Realize uma divisão piso de `init_number` por 2.
 - Eleve o `multiplication_result` à potência de 3

<div class='hint'> Primeiro, use o operador <code>/</code>. </div>
<div class='hint'> Depois, use o operador <code>%</code>. </div>

<div class='hint'> Em seguida, use o operador <code>*</code>. </div>

<div class='hint'> Depois, use o operador <code>+</code>. </div>

<div class='hint'> Depois, use o operador <code>-</code>. </div>

<div class='hint'> Por fim, use o operador <code>//</code>. </div>

<div class='hint'> Depois, use o operador <code>**</code>. </div>