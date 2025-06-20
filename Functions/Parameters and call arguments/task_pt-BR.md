## Parâmetros e argumentos de chamada

Os parâmetros da função são definidos dentro dos parênteses `()` após o nome da função. Um parâmetro atua como um nome de variável para um argumento passado para a função. 

Os termos parâmetro e argumento se referem à mesma coisa: informações que são passadas para uma função. No entanto, um parâmetro é a variável listada dentro dos parênteses na definição da função, enquanto um argumento é o valor que é enviado para a função quando ela é chamada.

Por padrão, a função deve ser chamada com o número correto de argumentos. Se sua função espera 2 argumentos, você tem que chamá-la com 2 argumentos:

```python
def minha_funcao(nome, sobrenome):
    print(nome + " " + sobrenome)

minha_funcao("Jon", "Snow")
```
Resultado:
```text
Jon Snow
```
No entanto, se você fornecer apenas um argumento durante a chamada:
```python
minha_funcao("Sam")
```
Será gerado um `TypeError`:
```text
TypeError                                 Traceback (most recent call last)
<ipython-input-29-40eb74e4b26a> in <module>
----> 1 my_function('Jon')

TypeError: minha_funcao() missing 1 required positional argument: 'sobrenome'
```
Para informações mais estruturadas e detalhadas, você pode consultar [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/7248?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
No editor de código, defina uma função que imprime o quadrado de um parâmetro passado.  

<div class='hint'>Adicione o parâmetro <code>x</code> dentro dos parênteses na definição da função.</div>