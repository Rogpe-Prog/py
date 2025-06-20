## Parâmetros padrão

Também é possível definir funções com um número variável de argumentos. Existem
três formas, que podem ser combinadas. A forma mais útil é especificar um valor padrão
para um ou mais argumentos. Isso cria uma função que pode ser chamada com menos
argumentos do que é definido. Por exemplo, confira a primeira função no editor de código.
Esta função pode ser chamada de várias maneiras:

- fornecendo apenas o argumento obrigatório `a`: `multiply_by(3)`

- fornecendo um dos argumentos opcionais: `multiply_by(3, 47)` ou `multiply_by(3, c=47)`

- ou até mesmo fornecendo todos os argumentos: `multiply_by(3, 47, 0)`

Você pode especificar qual argumento está fornecendo na chamada da função, assim como fizemos no terceiro caso
com `c=47`. Se você não especificar isso, os valores serão atribuídos de acordo com a ordem.
Não coloque espaços ao redor do símbolo `=` nas chamadas de função e nas definições.

Explore mais este tópico lendo <a href="https://docs.python.org/3/tutorial/controlflow.html#default-argument-values">esta seção</a>
da Documentação do Python.

Para obter informações mais estruturadas e detalhadas, você também pode se referir a [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/10295?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
Adicione parâmetros à função `hello()` e defina um valor padrão para o parâmetro `name`.  

<div class='hint'>Especifique qualquer valor padrão para o parâmetro <code>name</code>.</div>