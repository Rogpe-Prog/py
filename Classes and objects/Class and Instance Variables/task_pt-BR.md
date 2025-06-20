## Variáveis de Classe e de Instância

Em geral, as variáveis de instância são para dados exclusivos de cada instância,
e as variáveis de classe são para atributos e métodos compartilhados por todas as instâncias da classe:

```python
class Gato:

    especie = "Felis catus"  

    def __init__(self, raca, nome):
        self.raca = raca  
        self.nome = nome

cleo = Gato('mix', 'Cleo')
furry = Gato('bengal', 'Furry')

print(cleo.nome)
print(cleo.especie)
print(furry.nome)
print(furry.especie)
```

```text
Cleo
Felis catus
Furry
Felis catus
```
Você pode ver que `especie` é uma variável de classe compartilhada por todas as instâncias, enquanto
`nome` e `raca` são variáveis de instância únicas para cada instância.

Dados compartilhados podem ter efeitos possivelmente surpreendentes quando envolvem objetos mutáveis, 
como listas e dicionários. Se uma variável de classe é uma lista e você a modifica para
um objeto, ela será modificada para todos os objetos da classe (confira o exemplo no editor de código
– veja o que `print(barsik.comida_favorita)` vai imprimir). Se você pretende usar uma lista para acompanhar
as características exclusivas de cada instância, você precisa torná-la um atributo de instância.

Para obter informações mais estruturadas e detalhadas, você pode consultar [esta página da base de conhecimento do Hyperskill](https://hyperskill.org/learn/step/6677?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
No editor de código, complete a implementação da classe `Animais` para que a instrução `print`
abaixo imprima uma linha como esta: `"Este é o Doggy, o cachorro, um dos meus animais de estimação."` para cada um dos animais de estimação.

<div class="hint">A variável de classe deve conter informações compartilhadas entre todas as instâncias (é um dos <code>"animais de estimação"</code>).</div>
<div class="hint">As variáveis de instância devem conter informações únicas para as instâncias (o nome é único).</div>