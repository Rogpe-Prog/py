## Tuplas

Tuplas representam outro tipo padrão de sequência de dados.
Elas são quase idênticas às listas. A única diferença significativa entre tuplas e 
listas é que as tuplas são imutáveis: você não pode adicionar, substituir ou excluir elementos em 
uma tupla. As tuplas são construídas por elementos separados por vírgulas e contidos em parênteses, por 
exemplo: 

```python
(a, b, c)
```
 
Uma situação especial é a construção de tuplas contendo 0 ou 1 itens. 
Tuplas vazias são construídas por um par vazio de parênteses; 
uma tupla com um item é construída seguindo um valor com uma vírgula. Por exemplo:

```python
vazio = ()
singleton = 'olá',    # <-- note a vírgula no final
len(vazio)
```
```text
0
```
```python
len(singleton)
```
```text
1
```
```python
singleton
```
```text
('olá',)
```

A declaração `t = 12345, 54321, 'olá!'` é um exemplo de embalagem de tuplas: os 
valores `12345`, `54321` e `olá!` são agrupados juntos em uma tupla. 

Alguns outros métodos de lista também são 
aplicáveis a tuplas. Você pode ler mais sobre tuplas <a href="https://docs.python.org/3/tutorial/datastructures.html#tuples-and-sequences">aqui</a>.

Para obter informações mais estruturadas e detalhadas, você também pode se referir a [esta página de base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/7462?utm_source=jba&utm_medium=jba_courses_links).
  
### Tarefa
Imprima o comprimento da tupla `alfabeto`. Em seguida, crie uma tupla com um único elemento `'tupla_divertida'`. 
Você pode executar o código para ver o que ele imprime.  

<div class='hint'>Use a função <code>len()</code>.</div>

<div class='hint'>Não esqueça a vírgula no final na tupla com um elemento.</div>