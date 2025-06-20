## Escreva no arquivo

Como já mencionamos, se você usar `'w'` como o segundo argumento em `open()`, o arquivo é aberto 
apenas para escrita. Um novo arquivo vazio será criado. Se outro arquivo com o mesmo nome já existir, ele 
será apagado. Se você deseja adicionar algum conteúdo a um arquivo existente, você deve usar o modificador `'a'` 
(anexar).

Outro método do objeto de arquivo, `f.write(string)`, escreve o conteúdo de uma <i>string</i> no arquivo, retornando o 
número de caracteres escritos.

```python
f.write('Este é um teste\n')
```
```text
15
```
Outros tipos de objetos no modo de texto precisam ser convertidos em uma string primeiro:
```python
value = ('a resposta', 42)
s = str(value)  # converte a tupla em string
f.write(s)
```
```python
18
```
Onde o texto especificado será inserido no arquivo depende do modo do arquivo (`'a'` vs `'w'`).

`'a'`: o texto será inserido no final do arquivo.

`'w'`: o arquivo será esvaziado antes do texto ser inserido no início.

Se você deseja incluir um símbolo como uma quebra de linha, em sua string (para começar a partir de uma nova linha),
adicione-o com um `+`:
```python
f.write('\n' + 'string,' + ' ' + 'outra string')
```
Isso adicionará uma nova linha e escreverá `'string, outra string'`.

Para informações mais estruturadas e detalhadas, você pode se referir a [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/8334?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
No editor de código, **anexe** uma nova linha ao `output.txt` com todos os elementos da lista `zoo` separados por `' e '`. 
Use a sintaxe <code>' e '.join(lst)</code> para juntar os elementos da lista na string requerida. Depois,
anexe outra linha com o `número` ao mesmo arquivo de saída.

<div class='hint'>Use o modificador <code>'a'</code> para adicionar linhas ao final de um arquivo.</div>
<div class='hint'>Use o método <code>write()</code>.</div>
<div class='hint'>Converta <code>número</code> em uma string antes de escrever.</div>
<div class="hint">Adicione <code>\n</code> no início de cada string a escrever, para que acabe em uma linha separada.</div>