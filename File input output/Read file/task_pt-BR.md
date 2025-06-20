## Ler arquivo

Para ler o conteúdo de um arquivo, você pode chamar `f.read(size)`, que lê uma quantidade de dados e a retorna como 
uma string. Quando o size é omitido ou negativo, todo o conteúdo do arquivo será lido e retornado.

```python
com open('somefile.txt') como f:
    print(f.read())
```
```text
Aqui está tudo que está no arquivo.\n
```
<i>**Nota**: haverá um problema se o arquivo for duas vezes maior que a memória do seu computador.</i>

`f.readline()` lê uma única linha do arquivo; um caractere de nova linha (`\n`) é deixado no final da 
string e só é omitido na última linha do arquivo se o arquivo não terminar em uma nova linha. Se `f.readline()` 
retorna uma string vazia, o final do arquivo foi alcançado, enquanto uma linha em branco é representada por `\n`,
uma string contendo apenas uma nova linha.

```python
f.readline()
```
```text
'Esta é a primeira linha do arquivo.\n'
```
```python
f.readline()
```
```text
'Segunda linha do arquivo\n'
```
```python
f.readline()
```
```text
''
```
Para ler as linhas de um arquivo, você pode fazer um loop no objeto do arquivo. Isso é eficiente em termos de memória, rápido e 
simplifica o código:
```python
for line in f:
    print(line)
```
```text
Esta é a primeira linha do arquivo.
Segunda linha do arquivo
```
Se você quiser ler todas as linhas de um arquivo em uma lista, você também pode usar `list(f)` ou `f.readlines()`.

Para mais detalhes, confira a seção [Métodos dos Objetos de Arquivo](https://docs.python.org/3/tutorial/inputoutput.html#methods-of-file-objects) no Tutorial Python.

Para informações mais estruturadas e detalhadas, você também pode se referir a [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/8139?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
Imprima o conteúdo de "input.txt" na saída iterando sobre as linhas do arquivo e imprimindo cada uma.
Em seguida, imprima apenas a primeira linha de "input1.txt".

<div class="hint">Faça um loop no objeto do arquivo como no exemplo na descrição da tarefa.</div>
<div class='hint'>Use a função <code>print</code>.</div>
<div class='hint'>Use o método <code>readline()</code> para imprimir uma única linha.</div>