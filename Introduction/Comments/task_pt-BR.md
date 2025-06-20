## Comentários

Comentários em Python começam com o caractere de hash (`#`) e um espaço simples, 
e se estendem até o final da linha física. Você pode usar &atalho:ComentarioPorLinhaDeComentário; para comentar 
ou descomentar a linha inteira ou um bloco de código no PyCharm.

Sempre priorize manter os comentários atualizados quando o código mudar!
Comentários que contradizem o código são piores do que nenhum comentário.
Além disso, eles são desnecessários e de fato bastante distrativos se eles afirmarem o óbvio. Não faça isso:

```python
x = x + 1                 # Incrementa x
```

Comentários devem ser frases completas. A primeira palavra deve ser maiúscula, 
a menos que seja um identificador que comece com uma letra minúscula. Certifique-se de que 
seus comentários são claros e facilmente compreensíveis para outras pessoas.

#### Comentários de Bloco

Comentários de bloco geralmente se aplicam a algum (ou todo) código que os segue, e 
são indentados ao mesmo nível desse código.

#### Comentários em Linha
Use comentários em linha com parcimônia. Um comentário em linha é um comentário na 
mesma linha de uma declaração. Comentários em linha devem ser separados por pelo menos dois espaços da declaração.

Você pode ler mais sobre como comentar corretamente em <a href="https://www.python.org/dev/peps/pep-0008/#comments">PEP 8 – Guia de Estilo para Código Python</a>.

Você também pode comentar uma linha ou um bloco de código se você não quiser deletá-lo, mas não é necessário no momento.

Para obter informações mais estruturadas e detalhadas, você pode se referir a [esta página da base de conhecimentos Hyperskill](https://hyperskill.org/learn/step/6081?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
No editor de código, comente a linha com a declaração `print` que diz que não deveria ser impressa.
Veja como o código não é mais destacado.

<div class="hint">
  Adicione um <code>#</code> e um espaço antes dessa declaração <code>print</code>. Deixe todo o resto como está.
</div>