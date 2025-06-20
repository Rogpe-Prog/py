## Args e kwargs

Quando um parâmetro formal final na forma `**nome` está presente, ele recebe um dicionário 
(veja [Estruturas de Dados — Dicionários](curso://Estruturas de dados/Dicionários)) contendo 
todos os argumentos de palavras-chave, exceto aqueles correspondentes 
a um parâmetro formal. Isso pode ser combinado com um parâmetro formal na forma `*nome` que 
recebe uma tupla contendo qualquer número de argumentos posicionais além da lista de parâmetros formais 
(`*nome` deve ocorrer antes de `**nome`). Por exemplo, se definirmos uma função como a do
editor de código, ela poderia ser chamada como mostrado na chamada 1, que imprimiria:
```text
-- Você sabe como chegar à biblioteca?
-- Desculpe-me, eu não sou daqui, não tenho ideia sobre a biblioteca
Você pelo menos tem um charuto, senhor?
Claro, fique à vontade.
----------------------------------------
pessoa_perdida : banqueiro velho
outro_cara : palhaço de rua
cena : num parque
```
Esta função pode ser chamada com um número arbitrário de argumentos. Esses argumentos serão agrupados 
em uma tupla ou uma lista (veja [Tuplas](curso://Estruturas de dados/Tuplas), [Listas](curso://Estruturas de dados/Introdução às listas)). Antes do número variável de argumentos, podem ocorrer zero ou 
mais argumentos normais; no nosso caso existe um - `lugar`. Quaisquer parâmetros formais que ocorram 
após o parâmetro `*args` são argumentos ['somente-palavra-chave'](https://peps.python.org/pep-3102/), o que significa que eles só podem ser usados como palavras-chave 
em vez de argumentos posicionais. Uma outra maneira de chamar esta função é mostrada na chamada 2, e ela nos fornecerá 
o mesmo resultado.

Para obter informações mais estruturadas e detalhadas, você pode se referir a [esta](https://hyperskill.org/learn/step/8560?utm_source=jba&utm_medium=jba_courses_links) e [esta](https://hyperskill.org/learn/step/9544?utm_source=jba&utm_medium=jba_courses_links) páginas da base de conhecimento Hyperskill.

### Tarefa

No editor de código, modifique o código abaixo da função `gato()` para que imprima 
o seguinte:
```text
-- Esse gato comeria se você desse a ele qualquer coisa
-- Linda pelagem, o Maine Coon
-- Está gordo!
ESTÁ MUITO GORDO.
VOCÊ ESTÁ ALIMENTANDO SEU GATO DEMAIS.
```
<div class="dica">Lembre-se de desempacotar argumentos posicionais extras com <code>*</code>.</div>

<div class="dica">Lembre-se de desempacotar argumentos de palavras-chave com <code>**</code>.</div>

<div class="dica">Não se esqueça de fornecer o valor para o parâmetro formal <code>comida</code>.</div>
