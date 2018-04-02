# Folha de Estilo

## Histórico de Revisões

| Data     | Versão | Descrição                  | Autor(es)         |
|:--------:|:------:|:--------------------------:|:-----------------:|
|02/04/2018| 1.0    | Criação da Folha de Estilo | Felipe Hargreaves |

## 1. Disposição de Código

### 1.1 Identação
* O código Python deve ser identado utilizando 4 espaços por nível de identação.
* Templates HTML devem ser identados com 2 espaços por nível de identação.
* Deve se utilizar identação suspensa ao invés de alinhamento vertical para para separar parâmetros de métodos ou strings muito longas. 
* **Forma correta**:
```python
raise AttributeError(
    'Mensagem dividida ao longo de '
    'múltiplas linhas de forma correta'
)
```
* **Forma incorreta**:
  
```python
raise AttributeError('Mensagem dividida ao longo de '
                    'múltiplas linhas de forma incorreta')
```

### 1.2 Espaços vs. Tabs
* O código deve utilizar apenas espaços como forma de identação. O uso misto de tabs e espaços não é permitido pelo Python 3.

### 1.3 Tamanho Máximo de Linhas
* O tamanho das linhas de código deve ser limitado a 119 caracteres por linha.

### 1.4 Linhas em Branco
* Declarações de classes, métodos e grupos lógicos devem ser separados por uma linha em branco.

### 1.5 Imports
* Imports devem sempre estar localizados no topo do arquivo.
* Os imports devem estar agrupados da seguinte forma:
  * Standard library (biblioteca padrão do Python)
  * Bibliotecas externas
  * Componentes do Django
  * Componentes locais do Django
  * try/excepts
* Dentro de cada grupo as linhas devem estar organizadas em ordem alfabética, de acordo com o nome completo de cada módulo.
* Dentro de cada grupo, declarações de **import module** devem vir antes de declarações do tipo **from module import objects**.
* Deve se usar imports absolutos para componentes do Django e imports relativos para componentes locais.
* Linhas muito longas devem ser divididas utilizando parênteses e linhas de continuação de 4 espaços. Deve se colocar uma vírgula à direita após o último import e o parênteses final deve estar em linha separada.
* Deve se botar uma linha em branco entre o último import e qualquer código a nível de módulo, e duas linhas em branco acima da primeira função ou classe.
* Exemplo:
```python
# standard library
import json
from itertools import chain

# third-party
import bcrypt

# Django
from django.http import Http404
from django.http.response import (
    Http404, HttpResponse, HttpResponseNotAllowed, StreamingHttpResponse,
    cookie,
)

# local Django
from .models import LogEntry

# try/except
try:
    import yaml
except ImportError:
    yaml = None

CONSTANT = 'foo'


class Example:
    # ...
```

## 2. Comentários

* Comentários devem ser escritos na mesma linguagem utilizada para o restante do desenvolvimento.

* Comentários devem começar com letra maiúscula e serem terminados com ponto final.

### 2.1 Comentário de Bloco
* Comentários de bloco devem se referir ao conjunto de código que o segue, e devem estar no mesmo nível de identaçao deste código.
* Cada linha de um comentário de bloco deve começar com um '#' e um espaço em branco.

### 2.2 Comentários de Linha
* Devem ser utilizados com cuidado.
* Um comentário de linha deve estar separado por no mínimo 2 espaços da linha de código que o precede.
* Deve começar com um '#' e um espaço em branco.

### 2.3 Comentários TODO
* Utilize comentários TODO para indicar trechos de código temporários ou soluções a curto prazo.

## 3. Convenções de Nomes
* Nomes de classes devem ser escritos de acordo com o padrão **InitialCaps**. Isto é, a primeira letra de cada palavra que constitui o nome da classe deve ser maiúscula.

* Atributos, funções e métodos devem seguir o padrão **snake_case**. Isto é, devem fazer o uso do underscore para separar as palavras.
  * Uma exceção são *factory methods* que retornam classes. Estes devem seguir a convenção **InitialCaps** mencionada acima.

* Atributos devem ter nomes auto explicativos.

* Funções e métodos devem ter nomes que representem de forma clara a ação a ser realizada, de preferência utilizando de verbos.

## 4. Recomendações de Programação
* Nunca utilizar comparadores de igualdade (==, !=) para realizar comparações com *singletons* como None. Utilizar sempre **is** ou **not**.

* Utilizar o operator **is not** ao invés de **not ... is**, por questões de clareza.
* **Forma Correta**:
```python
if foo is not None:
```
* **Forma Incorreta**:
```python
if not foo is None:
```

* Derivar exceções de **Exception** ao invés de **BaseException**.

* Ser consistente com expressões de retorno. Todos os returns de uma função devem retornar uma expressão, ou então nenhum deve. 

* Se qualquer return em uma função retornar uma expressão, quaisquer returns adicionais sem valor retornado devem explicitamente retornar **None**.

* Para sequências, como listas, strings e tuplas, aproveitar do fato que sequências vazias são consideradas como **False**.
* **Usar**:
```python
if not seq:
if seq:
```
* **Ao invés de**:
```python
if len(seq):
if not len(seq):
```

* Não comparar valores booleanos com **True** ou **False**.
    * Correto: **if bool_value**
    * Incorreto: **if bool_value == True**
    * Incorreto: **if bool_value is True**

## 5. Estilo de Templates

* Deve haver apenas um espaço entre as chaves e o conteúdo do template.
* **Forma Correta**:
```django
{{ data }}
```
* **Forma Incorreta**:
```django
{{data}}
```

## 6. Estilo de Views

* O primeiro parâmetro em uma função de view deve se chamar **request**.
* **Forma Correta**:
```python
def my_view(request, foo):
    # ...
```
* **Forma Incorreta**:
```python
def my_view(req, foo):
    # ...
```

## 7. Estilo de Models
* Nomes de campos devem ser minúsculos, usando underscores ao invés de camelCase.

* **Forma Correta**:
```python
class Person(models.Model):
    first_name = models.CharField(max_length=20)
    last_name = models.CharField(max_length=40)
```
* **Forma Incorreta**:
```python
class Person(models.Model):
    FirstName = models.CharField(max_length=20)
    Last_Name = models.CharField(max_length=40)
```

* A classe **Meta** deve aparecer após a definição dos campos, com uma linha em branco separando os campos e a definição da classe.

* **Forma Correta**:
```python
class Person(models.Model):
    first_name = models.CharField(max_length=20)
    last_name = models.CharField(max_length=40)

    class Meta:
        verbose_name_plural = 'people'
```
* **Forma Incorreta**:
```python
class Person(models.Model):
    first_name = models.CharField(max_length=20)
    last_name = models.CharField(max_length=40)
    class Meta:
        verbose_name_plural = 'people'
```
* **Forma Incorreta**:
```python
class Person(models.Model):
    class Meta:
        verbose_name_plural = 'people'

    first_name = models.CharField(max_length=20)
    last_name = models.CharField(max_length=40)
```

* A ordem de classes internas da model e métodos padrão deve seguir o formato (nem todos são necessários):
    * Campos de banco de dados
    * Atributos de gerenciador customizados
    * **class Meta**
    * **def \__str__()**
    * **def save()**
    * **def get_absolute_url()**

## 8. Referências

1. [PEP 8 -- Style Guide for Python Code](https://www.python.org/dev/peps/pep-0008/)
2. [Django Documentation - Coding style](https://docs.djangoproject.com/en/dev/internals/contributing/writing-code/coding-style/)
3. [Google Python Style Guide](https://google.github.io/styleguide/pyguide.html)