## Argumentos por Palavras-Chave

Nós já sugerimos que funções também podem ser chamadas usando argumentos de palavras-chave na forma `kwarg=valor`. Por
exemplo, a função `cat()`, que nós definimos para você,
aceita um argumento obrigatório (`food`) e três argumentos opcionais (`state`, `action` e `breed`).
Pode ser chamada de qualquer uma das seguintes maneiras (você pode experimentar todas):

```python
cat('chicken')                     # 1 argumento posicional
cat(food='chicken')                # 1 argumento de palavra-chave
cat(food='fish', action='bite')    # 2 argumentos de palavras-chave
cat(action='bite', food='fish')    # 2 argumentos de palavras-chave
cat('beef', 'happy', 'hiss')       # 3 argumentos posicionais
cat('a hug', state='purrring')     # 1 posicional, 1 de palavra-chave
```
Em uma chamada de função, os argumentos de palavras-chave devem seguir os argumentos posicionais. Todos os argumentos de 
palavras-chave passados devem corresponder a um dos argumentos aceitos pela função (por exemplo, `book` não é um argumento válido 
para a função `cat`), e a ordem deles não é importante. Isso também inclui argumentos não opcionais 
(por exemplo, `cat(food='fish')` também é válido). Nenhum argumento pode receber um valor mais de uma vez.
Todas as seguintes chamadas seriam inválidas:

```python
cat()                              # argumento obrigatório ausente
cat(food='fish', 'dead')           # argumento posicional após um argumento de palavra-chave
cat('veggies', food='nothing')     # valor duplicado para o mesmo argumento
cat(actor='Johnny Depp')           # argumento de palavra-chave desconhecido
```

### Tarefa
No editor, complete a chamada da função com argumentos para que ela imprima o seguinte:
```text
-- Este gato não rosnaria se você desse sopa a ele
-- Pelo adorável, a Esfinge
-- Ainda está com fome!
```

<div class="hint">Para argumentos de palavras-chave, use a sintaxe como <code>state='asleep'</code>.</div>
<div class="hint">O argumento obrigatório <code>food</code> precisa estar na primeira posição, a menos que você o forneça como um argumento de palavra-chave.</div>