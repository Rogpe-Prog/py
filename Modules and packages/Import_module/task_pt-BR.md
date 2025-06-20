## Importar módulo

Conforme seu programa fica mais longo, você pode querer dividi-lo em vários arquivos para 
facilitar a manutenção. Você também pode querer usar uma função prática que você escreveu 
em vários programas sem copiar sua definição para cada um deles.

Os módulos em Python são simplesmente arquivos Python com a extensão `.py` que contêm 
definições e declarações Python.
Os módulos são importados de outros módulos utilizando a palavra-chave `import` 
e o nome do arquivo sem a extensão `.py`. 

Digamos que você escreveu um script chamado `my_funcs.py` com um monte de funções (`func1`, `func2`, 
etc.). Agora, se você quiser usar essas em outro script que está no mesmo diretório, 
você pode fazer `import my_funcs`. Isso não importa os nomes das funções definidas em `my_funcs` 
diretamente, mas usando o nome do módulo, você pode agora acessar as funções, por exemplo:
```python
my_funcs.func1()
```
  
Para informações mais estruturadas e detalhadas, você também pode se referir a [esta página da base de conhecimento Hyperskill](https://hyperskill.org/learn/step/6019#module-loading?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
No editor de código, você já importou o módulo `my_funcs`. 
Chame a função `hello_world` deste módulo com o argumento `"John"`.

<div class='hint'>Acesse a função do módulo usando a sintaxe como <code>module.function()</code>.</div>
<div class="hint">Não se esqueça de fornecer um argumento para a função.</div>