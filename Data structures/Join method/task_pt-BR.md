## O método join()

`.join()` é, de fato, um método de string, mas estamos discutindo isso agora porque ele 
exige a compreensão de objetos iteráveis, como strings, listas e tuplas.
Este [método](https://docs.python.org/3/library/stdtypes.html#str.join) fornece uma forma flexível de criar strings a partir de objetos iteráveis. 
Ele une cada elemento de um iterável (como lista, string ou tupla) por 
um separador de string (uma string na qual o método `join()` é chamado) e 
retorna uma string concatenada. Um `TypeError` será levantado se houver 
quaisquer valores não-string no iterável.

A sintaxe do método `join()` é a seguinte:

```python
string.join(iterable)
```

Exemplos:

```python
string_ = 'abcde'  # um iterável do tipo string
tuple_ = ('aa', 'bb', 'cc')  # um iterável do tipo tupla
list_ = ['Python', 'linguagem de programação']  # um iterável do tipo lista

print(' + '.join(string_))  # junta com o separador ' + '
print(' = '.join(tuple_))  # junta com o separador ' = '

sep = ' é uma '
print(sep.join(list_))  # junta com o separador ' é uma '
```
```text
a + b + c + d + e
aa = bb = cc
Python é uma linguagem de programação
```

Para obter informações mais estruturadas e detalhadas, você pode consultar [esta página da base de conhecimento Hyperskill](https://hyperskill.org/learn/step/6972#join-a-list?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
Atribua um valor à variável `joined` de forma que a instrução `print` imprima o seguinte:
```text
Eu gosto de maçãs e eu gosto de bananas e eu gosto de pêssegos e eu gosto de uvas
```

<div class="hint">Observe atentamente os exemplos e faça simplesmente o mesmo!</div>
<div class="hint"><code>frutas</code> é o seu iterável aqui, e <code>separador</code> é a string do separador.</div>