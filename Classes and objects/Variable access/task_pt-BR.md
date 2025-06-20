## Acesso à variável

Você pode usar referências de atributo para acessar variáveis dentro de um objeto.
As referências de atributo usam a sintaxe padrão para todas as referências de atributos no Python: `obj.nome`. Nomes de atributos válidos são todos os nomes que estavam no espaço de nomes da classe quando o objeto da classe foi criado. Então, se a definição da classe se parecia com isso:

```python
class MyClass:
    year = 2021

    def say_hello(self):
        return 'hello world'
```
então `MyClass.year` e `MyClass.say_hello` são referências de atributo válidas que retornam um inteiro e um objeto de função, respectivamente. Atributos de classe podem ser atribuídos, então você pode alterar o valor de `MyClass.year` por atribuição.

Para informações mais estruturadas e detalhadas, você pode se referir a [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/6661#class-attribute?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
Confira nosso exemplo e imprima o valor de `variable1` de `my_object`.
Chame o método `foo` do objeto `my_object`, imprima o resultado.

<div class='hint'>Acesse <code>variable1</code> usando a sintaxe <code>object.name</code>.</div>