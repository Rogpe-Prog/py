## Definição

Funções são uma maneira conveniente de dividir seu código em blocos úteis, torná-lo mais legível e reutilizá-lo.
A palavra-chave `def` introduz uma definição de função.
Ela deve ser seguida pelo nome da função e pela lista entre parêntesis de **parâmetros formais** (que pode ser vazio).
As declarações que formam o corpo da função começam na próxima linha e devem ser recuadas.

<details>
Os parâmetros formais estão envolvidos em parênteses; são as variáveis definidas pela função, que recebem valores quando a função é chamada. A lista consiste nos nomes de todas as variáveis necessárias para o método. Cada parâmetro formal é separado por uma vírgula. Quando o método não aceita nenhum valor de entrada, ele deve ter um conjunto vazio de parênteses após o nome do método, por exemplo, <code>addition()</code>.
</details>

Funções são executadas apenas quando são chamadas. Para chamar uma função, use seu nome seguido de parênteses:

```python
def my_function():  # definição de função
  print("Olá de uma função")

my_function()  # chamada de função
```

Leia mais sobre como definir funções nesta <a href="https://docs.python.org/3/tutorial/controlflow.html#defining-functions">seção</a> da Documentação Python.

Para obter informações mais estruturadas e detalhadas, você também pode se referir a [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/5900?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
 - Chame a função `my_function` dentro do loop para repetir sua invocação 5 vezes
 - Defina uma função que possa substituir as declarações `print` duplicadas no arquivo.

<div class='hint'>Use o <code>()</code> para chamar a função <code>my_function</code>.</div>
<div class='hint'>Use a palavra-chave <code>def</code> para definir a função <code>fun</code>.</div>