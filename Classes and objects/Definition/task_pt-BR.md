## Definição

Classes fornecem um meio de agrupar dados e funcionalidades. Criar uma nova
classe cria um novo tipo de objeto, permitindo a criação de novas instâncias desse tipo.
Classes são essencialmente modelos para a criação de seus objetos.
Cada instância de classe (objeto) pode ter atributos anexados a ele para manter seu estado.
Funções de objetos são chamadas de métodos, e eles podem modificar seu estado. Métodos são
definidos pela classe do objeto.

A forma generalizada de definição de classe se parece com isso:

```
class NomeDaClasse:
    <declaração-1>
    .
    .
    .
    <declaração-N>
```
As definições de classe, como as definições de função (declarações `def`) devem ser executadas antes
que eles tenham algum efeito.

As declarações dentro de uma definição de classe geralmente serão definições de função,
mas outras declarações às vezes são úteis. As definições de função dentro de uma
classe normalmente têm uma forma peculiar de lista de argumentos - isso será explicado mais tarde.

Os objetos de classe suportam dois tipos de operações: referências de atributos e instanciação.
Referências de atributos serão discutidas nas seções seguintes. A instanciação de classe usa
notação de função. Apenas imagine que o objeto de classe é uma função sem parâmetros que
retorna uma nova instância da classe. Por exemplo:

```python
class AlgumaClasse:
    """Um exemplo simples de classe"""
    i = 12345

x = AlgumaClasse()
```

`x = AlgumaClasse()` cria uma nova instância da classe e atribui este objeto à variável local `x`.

Você pode descobrir mais sobre a sintaxe de definição de classe lendo <a href="https://docs.python.org/3/tutorial/classes.html#class-definition-syntax">esta seção</a>
da Documentação Python.

Para obter informações mais estruturadas e detalhadas, você pode também se referir a [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/6661?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
Atribua um valor à `variável` dentro de `MyClass` e crie um objeto `my_object` da classe `MyClass()`. 
Execute o código e veja o que acontece!

<div class='hint'>Atribua qualquer valor ao <code>variável</code>.</div>

<div class='hint'>Olhe o exemplo no texto para descobrir como instanciar um objeto.</div>
