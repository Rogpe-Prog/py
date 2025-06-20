## Literais de string formatada

Um literal de string formatada, ou uma f-string, é um literal de string que é prefixado
com 'f' ou 'F'. Essas strings podem conter campos de substituição, que são
expressões delimitadas por chaves `{}`.

As partes da string fora das chaves são tratadas literalmente.
Sequências de escape são decodificadas como em literais de string comuns.
Expressões de substituição podem conter quebras de linha (por exemplo, em strings entre três aspas),
mas elas não podem conter comentários. Cada expressão é avaliada no contexto
onde o literal de string formatada aparece, em ordem da esquerda para a direita.

Aqui estão alguns exemplos:
```python
name = "Fred"
f"Ele disse que o nome dele é {name}."
```
```text
'Ele disse que o nome dele é Fred.'
```

Existem coisas mais sofisticadas que você pode fazer em f-strings, por exemplo:
```python
f"{name.lower()} é engraçado."
```

```text
'fred é engraçado.'
```

Para mais informações sobre literais de strings formatadas, você pode consultar <a href="https://docs.python.org/3/reference/lexical_analysis.html#formatted-string-literals"> Documentação do Python</a>.

Para informações mais estruturadas e detalhadas, você também pode se referir [a esta página da base de conhecimento Hyperskill](https://hyperskill.org/learn/step/6037?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa

Tente criar uma f-string você mesmo. Tente também executar o código para ver o que ele imprime.

<div class="hint">O valor atribuído à variável <code> name </code> deve ser uma string, então precisa estar entre aspas,
assim: <code>'Max'</code>.</div>
