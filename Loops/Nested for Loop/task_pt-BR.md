## Loops Aninhados

Um loop aninhado é um loop dentro de outro loop.
O loop interno é executado uma vez para cada iteração do loop externo.

```python
adjetivos = ["preto", "elegante", "caro"]
roupas = ["jaqueta", "camisa", "botas"]

for x in adjetivos:
  for y in roupas:
    print(x, y)
```
Saída:
```text
preto jaqueta
preto camisa
preto botas
elegante jaqueta
elegante camisa
elegante botas
caro jaqueta
caro camisa
caro botas
```
<details>

Note que qualquer tipo de loop pode ser aninhado dentro de outro loop. 
Por exemplo, um loop [`while`](course://Loops/While loop) (veja adiante) pode ser aninhado dentro de um loop `for`, ou vice-versa.
</details>

Para informações mais estruturadas e detalhadas, você pode se referir a [esta página da base de conhecimento Hyperskill](https://hyperskill.org/learn/step/6065#nested-loop?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
Foi dado a você um tabuleiro de jogo da velha de 3x3, sua tarefa é imprimir cada posição. As coordenadas ao longo de cada lado
são armazenadas na lista `coordenadas`. A saída deverá ser:
```text
1 x 1
1 x 2
1 x 3
2 x 1
...
```
e assim por diante para cada combinação de coordenadas.

<div class="hint">

No loop `for` aninhado, itere novamente sobre a mesma lista usando outro nome de variável
desta vez (`coordenada2`).
</div>