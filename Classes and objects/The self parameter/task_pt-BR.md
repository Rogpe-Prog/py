## O parâmetro self

É hora de explicar o parâmetro `self` que vimos nas tarefas anteriores.
O primeiro argumento passado para um método de classe é `self`. Isso não é mais 
do que uma convenção: o nome `self` não tem nenhum significado especial para o Python. 
É aconselhável seguir a convenção, caso contrário, seu código pode ser menos legível 
para outros programadores Python.

O Python usará o parâmetro `self` para se referir ao objeto que é criado ou modificado.  
Os métodos podem chamar outros métodos usando atributos de método do argumento `self`:

```python
class Bag:
    def __init__(self):
        self.data = []

    def add(self, x):
        self.data.append(x)

    def addtwice(self, x):
        self.add(x)  # Chamando o método `add` de outro método
        self.add(x)
```
  
Para obter informações mais estruturadas e detalhadas, você pode se referir a [esta página da base de conhecimento Hyperskill](https://hyperskill.org/learn/step/6669#self?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
No editor de código, implemente o método `add` da classe `Calculator`. Ele deve 
adicionar `amount` ao campo `current`. Além disso, complete o método `get_current`.
Execute o código para ver como funciona.

<div class='hint'>Adicione <code>amount</code> à variável <code>self.current</code>.</div>
<div class="hint">Use o sinal <code>+=</code>.</div>