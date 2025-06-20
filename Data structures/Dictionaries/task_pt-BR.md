## Dicionários

Um dicionário é semelhante a uma lista, exceto que você acessa seus valores procurando uma 
chave em vez de um índice. Uma chave pode ser de qualquer tipo imutável. Strings e números sempre podem  
ser chaves; as tuplas podem ser usadas como chaves se contiverem apenas objetos imutáveis. 
Você não pode usar listas como chaves. 

Pense em um dicionário como um conjunto de pares <code>chave: valor</code>, com a exigência 
de que as chaves sejam únicas em um dicionário. Os dicionários são delimitados 
por chaves, por exemplo, `dct = {'chave1': "valor1", 'chave2': "valor2"}`. Um par de 
chaves cria um dicionário vazio: `{}`.  

Um dicionário também pode ser criado com o construtor `dict`:
```Python
a = dict(um=1, dois=2, três=3)
b = {'um': 1, 'dois': 2, 'três': 3}
c = dict([('dois', 2), ('um', 1), ('três', 3)])
print(a == b == c)
```
```text
True
```

Você pode acessar um valor em um dicionário de maneira semelhante a como você acessaria um valor em uma lista,
mas usando uma chave em vez de um índice. Mais informações sobre essa estrutura de dados podem ser encontradas 
<a href="https://docs.python.org/3/tutorial/datastructures.html#dictionaries">aqui</a>.

Para obter informações mais estruturadas e detalhadas, você também pode se referir a [esta página da base de conhecimentos Hyperskill](https://hyperskill.org/learn/step/6481?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
Adicione o número do Jared (`"Jared"`) `570` à agenda.
Remova o número do Gerard da agenda.
Imprima o número de telefone da Jane da `agenda`.  

<div class='hint'>Use a indexação do dicionário, por exemplo, <code>dct[chave]</code></div>