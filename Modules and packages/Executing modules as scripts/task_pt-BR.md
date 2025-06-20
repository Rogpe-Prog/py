## Executando módulos como scripts

Um módulo Python é um arquivo que contém instruções executáveis, bem como definições de funções ou classes.
Essas instruções são executadas pela primeira vez que o nome do módulo é encontrado em uma instrução `import`.
O nome do arquivo é o nome do módulo com o sufixo .py anexado. Dentro de um módulo, o
nome do módulo (como uma string) está disponível como o valor da variável global `__name__`.

Quando você executa um módulo **diretamente** (ou seja, não o importando em outro),
o código no módulo será executado, assim como se você o tivesse importado, mas com
`__name__` definido como `"__main__"`.

Você pode usar `__name__` e `__main__` assim:

```python
if __name__ == "__main__":
   # Faça algo aqui
```

As instruções dentro deste bloco serão executadas apenas se o módulo for executado diretamente e não através da importação
em outro módulo. Por exemplo, vamos considerar dois arquivos:

programa_principal:
```python
import algum_modulo

print(f"programa_principal __name__ é: {__name__}")

if __name__ == "__main__":
   print("programa_principal executado diretamente")
else:
   print("programa_principal executado quando importado")
```

algum_modulo:
```python
print(f"algum_modulo __name__ é: {__name__}")

if __name__ == "__main__":
   print("algum_modulo executado diretamente")
else:
   print("algum_modulo executado quando importado")
```

Saída após executar `programa_principal`:
```text
algum_modulo __name__ é: algum_modulo
algum_modulo executado quando importado
programa_principal __name__ é: __main__
programa_principal executado diretamente
```

Saída após executar `algum_modulo`:
```text
algum_modulo __name__ é: __main__
algum_modulo executado diretamente
```

Para obter informações mais estruturadas e detalhadas, você pode se referir a [esta página da base de conhecimento Hyperskill](https://hyperskill.org/learn/step/6057?utm_source=jba&utm_medium=jba_courses_links).

### Tarefa
<i>Os arquivos nesta tarefa têm o mesmo nome que nos exemplos acima, mas seu código é um pouco diferente.</i>

Modifique `task.py` e `algum_modulo.py` de modo que, quando você executa `task.py`, sua saída seja a seguinte:

```text
Esta é uma mensagem de algum_modulo.
Esta é uma mensagem de __main__.
Esta é uma mensagem da função no módulo importado.
Isso deve ser impresso APENAS quando task.py é chamado diretamente.
```