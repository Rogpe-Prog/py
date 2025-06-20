## de importação

Uma forma do comando de importação traz nomes `de` um módulo diretamente. Dessa maneira, você 
pode usar o nome importado sem o prefixo `module_name`. Por exemplo:

```python
from calculator import Add

calc = Add()    # nome `Add` usado diretamente sem o prefixo `calculator`
```

Isso não introduz o nome do módulo do qual as importações são retiradas na 
tabela de símbolos local (então, em nosso exemplo, `calculator` não está definido).

Existe até uma opção de importar todos os nomes que um módulo define:
```python
from calculator import *
calc = Multiply()
```
Isso importa todos os nomes exceto aqueles que começam com um sublinhado `_`.
Na maioria dos casos, os programadores Python não usam isso, pois introduz 
um conjunto desconhecido de nomes no interpretador, possivelmente escondendo algumas coisas 
que você já definiu.

Se o nome do módulo for seguido por `as`, então o nome após `as` é vinculado 
diretamente ao módulo importado:

```python
import my_module as mm
mm.hello_world()
```
Isso está efetivamente importando o módulo da mesma maneira que `import my_module` vai 
fazer, com a única diferença de estar disponível como `mm`. Isso também pode ser usado 
ao usar `from` com efeitos semelhantes:

```python
from calculator import Subtract as Minus
```

Para informações mais estruturadas e detalhadas, você pode se referir a [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/6019#module-loading?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
Importe a classe `Calculator` do `calculator` e crie uma instância dessa classe. Lembre-se de como acessá-la corretamente nesse caso.


<div class="hint">Nota: A classe <code>Calculator</code> deve ser chamada sem um prefixo porque você a importou diretamente.</div>