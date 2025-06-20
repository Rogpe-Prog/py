## Declarações Else e Elif

As declarações `elif` e `else` complementam a declaração `if`. 
Pode haver zero ou mais partes `elif`, e a parte `else` é opcional. A palavra-chave 
`elif` é a abreviação de 'else if', e é útil para evitar indentação excessiva.

<div class="hint">Uma sequência <code>if ... elif ... elif ...</code> é um substituto para as declarações <code>switch</code> ou 
<code>case</code> encontradas em outras linguagens, como Java.</div>

Na execução condicional, apenas uma das suítes é selecionada avaliando as expressões uma por uma até que uma seja considerada
`True`. Então essa suíte é executada e nenhuma outra parte da declaração `if` é avaliada.
Se todas as expressões são falsas, a suíte da cláusula `else`, se presente, é executada.

```python
a = 200
b = 33
if b > a:
  print("b é maior que a")
elif a == b:
  print("a e b são iguais")
else:
  print("a é maior que b")
```
```text
a é maior que b
```

<details>

Uma declaração if-else simples também pode ser ajustada em uma linha de código, assim como mostramos na tarefa anterior. Por exemplo,
```python
if a > b:
    a += 1
else: 
    a -= 1
```
pode ser escrita como
```python
a += 1 if a > b else a -= 1
```
</details>
  
Para informações mais estruturadas e detalhadas, você pode se referir a [esta](https://hyperskill.org/learn/step/5932?utm_source=jba&utm_medium=jba_courses_links) e [esta](https://hyperskill.org/learn/step/5926?utm_source=jba&utm_medium=jba_courses_links) páginas da base de conhecimento Hyperskill.

### Tarefa
Imprima `True` se `name` for igual a `"John"` e `False` caso contrário.  

<div class='hint'>Use a palavra-chave <code>if</code> e o operador <code>==</code>.</div>
<div class='hint'>Use a palavra-chave <code>else</code>.</div>