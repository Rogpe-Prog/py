## Métodos \_\_str__ vs \_\_repr__

Ambos os métodos `str()` e `repr()` em Python são usados para a representação de string de um objeto,
mas existem algumas diferenças.
Por exemplo:
```python
s = 'Olá Mundo'
print (str(s))
print(repr(s))
```
```text
Olá Mundo
'Olá Mundo'
```
Você pode ver que se imprimirmos uma string usando a função `repr()`, então ela é impressa
com um par de aspas. `str()` é usada para criar uma saída para o usuário, enquanto `repr()` 
é normalmente usada para depuração e desenvolvimento. `repr()` precisa ser inequívoca, 
e `str()` &mdash; para ser legível.

Assim como `__init__`, os métodos `__repr__` e `__str__` são reservados em Python.
A instrução `print()` e a função incorporada `str()` usam o método `__str__` definido na classe do objeto
para exibir sua representação em string. A função incorporada `repr()` usa o método `__repr__` 
definida na classe do objeto.

Nossa própria classe definida deve, portanto, ter uma `__repr__` se precisarmos de informações detalhadas para depuração. 
Além disso, se pensarmos que seria útil ter uma representação de string para os usuários, devemos criar 
uma função `__str__`. Confira outra implementação da classe `Complex` no editor de código. Execute o código
para ver o que cada uma das duas instruções `print` imprime.

Para informações mais estruturadas e detalhadas, você pode se referir a [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/7139#str__-vs-__repr?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
Implemente os métodos `__str__` e `__repr__` para a classe `Cat`. O método `__str__` deve retornar uma string como esta:
`"Meu gato siamês se chama Lucy"`;  o método `__repr__` deve retornar uma string como esta:
`"Gato, raça: siamês, nome: Lucy"`. Use [f-strings](course://Strings/F-strings).



<div class="hint">Não se esqueça de usar a sintaxe <code>self.attribute</code>.</div>
<div class="hint"> Não se esqueça de escapar o caractere para imprimir o apóstrofo.</div>
