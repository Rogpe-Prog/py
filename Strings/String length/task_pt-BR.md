## Comprimento da string

O método `len()` é usado para contar quantos caracteres uma string contém.

Por exemplo:
```python
s = "Olá Mundo"
print(len(s))   # vai imprimir 9
```

Note que o resultado da operação de divisão `/` é do tipo float:
```python
a = 10/2
print(a)        # 5.0
print(type(a))  # <class 'float'>
```

Para informações mais estruturadas e detalhadas, você pode se referir a [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/5814?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
Obtenha a primeira metade da string armazenada na variável `phrase`.  
Nota: ao obter o índice, lembre-se da conversão de tipo.  

<div class='hint'>Você precisa obter um pedaço da string desde o início  
até o ponto médio.</div>

<div class='hint'>Obtenha o índice do meio dividindo o comprimento da string por 2. O 
resultado da divisão precisa ser um inteiro.</div>