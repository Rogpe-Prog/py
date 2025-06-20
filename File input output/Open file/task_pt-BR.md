## Abrir arquivo
Python possui várias funções embutidas para ler e escrever informações em um arquivo no seu computador.

`open()` retorna um objeto de arquivo e é mais comumente usado com dois argumentos: `open(filename, mode)`:
```python
f = open('somefile.txt', 'w')
```
O primeiro argumento é uma string contendo o nome do arquivo. O segundo argumento é outra string contendo
alguns caracteres descrevendo a maneira como o arquivo será usado. Pode ser `'r'` se o arquivo
será apenas lido, `'w'` - para escrita apenas (um arquivo já existente com o mesmo nome será apagado) e
`'a'` abre o arquivo para adição – qualquer dado escrito no arquivo é adicionado ao seu final.
`'r+'` abre o arquivo para leitura e escrita. O argumento do modo é opcional; `'r'` será presumido 
se for omitido.

É uma boa prática usar a palavra-chave `with` ao lidar com objetos de arquivo. A vantagem é que o
arquivo é devidamente fechado depois que a suíte de código termina.

```python
with open('somefile.txt') as f:
    read_data = f.read()

# Podemos verificar que o arquivo foi automaticamente fechado.
f.closed
```
```text
Verdadeiro
```
**Importante**: Se você não está usando a palavra-chave `with`, então você deve chamar `f.close()` para fechar o arquivo e
liberar quaisquer recursos do sistema usados por ele. Você não pode usar o objeto de arquivo depois que ele é fechado, seja por uma declaração `with` ou por chamar `f.close()`.

Para informações mais estruturadas e detalhadas, você pode se referir a [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/8691?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
- No editor de código, abra o arquivo `input1.txt` no modo de leitura, usando corretamente a declaração `with`. O arquivo `input1.txt` armazena o nome do arquivo onde a string `Olá Mundo` deve ser saída. A leitura deste nome já está implementada na variável `outfile_name`.
- Abra o arquivo com o nome `outfile_name` no modo de gravação.
- Posteriormente, feche o arquivo de saída que foi aberto.

Depois de executar seu código, confira o arquivo de saída que apareceu na visualização do curso entre os outros arquivos.

<div class="hint">Forneça o argumento <code>r</code> para o método <code>open()</code>,
apenas para fins de prática!</div>