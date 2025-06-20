## Pacotes

Pacotes são uma maneira de estruturar o módulo [namespace](https://docs.python.org/3/tutorial/classes.html#python-scopes-and-namespaces) do Python usando "nomes de módulos com pontos". Por exemplo, o nome do módulo `A.B` designa um submódulo chamado `B` em um pacote chamado `A`. Assim como o uso de módulos evita que os autores de diferentes módulos tenham que se preocupar com os nomes das variáveis globais uns dos outros, o uso de nomes de módulos com pontos evita que os autores de pacotes multi-módulo como [NumPy](https://numpy.org/) ou [Pillow](https://pypi.org/project/Pillow/) tenham que se preocupar com os nomes dos módulos uns dos outros.

<div class="hint">Os arquivos <code>__init__.py</code> são necessários para fazer com que o Python trate diretórios que contêm o arquivo como pacotes. Isso impede que diretórios com um nome comum, como <code>string</code>, ocultem involuntariamente módulos válidos que aparecem mais tarde no caminho de busca do módulo. No caso mais simples, <code>__init__.py</code> pode ser apenas um arquivo vazio.</div>

Confira os pacotes `functions` e `classes` que criamos. Os usuários dos pacotes podem importar módulos individuais do pacote, por exemplo:

```python
import functions.greeting.hello
```

Isso carrega o submódulo `functions.greeting.hello`. Ele deve ser referenciado com seu nome completo:

```python
functions.greeting.hello.hello('Susan')
```
Uma maneira alternativa de importar o submódulo é:

```python
from functions.greeting import hello
```

Isso também carrega o submódulo `hello`, e o torna disponível sem seu prefixo de pacote, para que possa ser usado da seguinte maneira:

```python
hello.hello('Susan')
```

Você pode aprender mais sobre pacotes lendo <a href="https://docs.python.org/3/tutorial/modules.html#packages">esta página</a> da Documentação do Python.

Para informações mais estruturadas e detalhadas, você também pode se referir a [esta página da base de conhecimento Hyperskill](https://hyperskill.org/learn/step/6384?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
Olhe para a estrutura de arquivos nos diretórios `classes` e `functions` e seus subdiretórios.

No editor de código, importe o módulo `official` corretamente para fazer o último comando `print` funcionar.

Na segunda instrução de impressão, adicione uma chamada de função (encontre a função certa) para que ela imprima um adeus para `'Alex'`.

<div class="hint">Acesse o módulo usando uma sintaxe como <code>package.subpackage.module</code>.</div>
<div class="hint">Use uma sintaxe como <code>import module as something</code>.</div>
<div class="hint">Confira as importações: existe uma que pode ter a função certa para a segunda tarefa.
Tenha cuidado ao usá-la: o módulo já está importado com um nome específico.</div>