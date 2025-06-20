## Método especial &#95;&#95;init&#95;&#95;

A operação de instanciação (chamar um objeto de classe) cria um objeto vazio,
mas é útil criar objetos com instâncias personalizadas para um estado inicial específico. 
Portanto, uma classe pode definir um método especial chamado `__init__()`,
assim:

```python
class MyClass:
    def __init__(self):
        self.data = []
```
`__init__` é um dos métodos reservados em Python. Se definido, o método `__init__()`
é invocado automaticamente quando uma instância da classe é criada,
e inicializa o objeto e seus atributos. Ele sempre recebe pelo menos
um argumento, `self`. Então, no nosso exemplo,
uma nova instância inicializada pode ser obtida por:

```python
x = MyClass()
```
O método `__init__()` pode receber argumentos para maior flexibilidade.
Nesse caso, argumentos fornecidos ao operador de instanciação da classe são passados
para `__init__()`. Por exemplo:
```python
class Complexo:
    def __init__(self, parte_real, parte_imag):
        self.r = parte_real
        self.i = parte_imag
        self.num = complex(self.r, self.i)

x = Complexo(3.0, -4.5)  # Instanciando um número complexo
x.num
```
```texto
(3-4.5j)
```

Para obter informações mais estruturadas e detalhadas, você pode consultar [esta página da base de conhecimento Hyperskill](https://hyperskill.org/learn/step/6669#def-__init?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
No editor de código, adicione parâmetros ao método `__init__()` da classe `Car`, para que possamos
criá-lo com uma cor e marca especificadas.

<div class='hint'>Adicione três parâmetros &mdash; <code>self</code>, <code>cor</code> e <code>marca</code>.</div>