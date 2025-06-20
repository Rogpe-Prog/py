## Módulos integrados

Python vem com uma [biblioteca de módulos padrão](https://docs.python.org/3/library/).

Alguns módulos estão integrados ao interpretador; esses fornecem acesso a operações que não fazem parte do núcleo da linguagem, mas ainda assim estão integradas, seja para eficiência ou para fornecer acesso a primitivas do sistema operacional, como chamadas de sistema.
Um módulo em particular merece alguma atenção: `sys`, que está integrado a cada interpretador Python. As variáveis `sys.ps1` e `sys.ps2` definem as strings usadas como prompts primário e secundário se o interpretador estiver no modo interativo:

```text
>>> import sys
>>> sys.ps1
'>>> '
>>> sys.ps2
'... '
```

A variável `sys.path` é uma lista de strings que determina o caminho de busca do interpretador para módulos: veja o que ele imprime para você quando você executa o código da tarefa.

Lembre-se de que você pode usar o atalho &shortcut:CodeCompletion; após um ponto (.) para explorar os métodos disponíveis de um módulo. Você pode ler mais sobre módulos padrão <a href="https://docs.python.org/3/tutorial/modules.html#standard-modules">aqui</a>.

Para obter informações mais estruturadas e detalhadas, você também pode consultar [esta página da base de conhecimento Hyperskill](https://hyperskill.org/learn/step/6019#built-in-modules?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
Imprima a data e a hora atuais usando um módulo integrado importado `datetime`.

<div class='hint'>Use a função <code>datetime.datetime.today()</code>.</div>