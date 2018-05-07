<style> p { text-align: justify; text-indent: 30px; } </style>

# Padrões GOF

## Introdução

Uma das primeiras tentativas de estudo e documentação de padrões de projeto foi um livro chamado **Padrões de Projeto - Soluções Reutilizaveis de Software Orientado a Objetos**, escrito por *Erich Gamma, Richard Helm, Ralph Johnson*, e *John Vlissides*, que posteriormente ficariam conhecidos como *Gang of Four* (GoF). O trabalho realizado por eles e documentado neste livro se tornou tão importante que para muitos os 23 padrões de projeto descritos na obra são peças fundamentais na Engenharia de *Software*

Os 23 padrões tem sido classificados da seguinte forma:

- **Criacionas**, são padrões voltados para a criação de objetos.
    - Abstract Factory
    - Builder
    - Factory Method
    - Prototype
    - Singleton
- **Estruturais**, são padrões focados na forma como devem ser estruturados(as) classes e objetos.
    - Adapter
    - Bridge
    - Composite
    - Decorator
    - Facade
    - Flyweight
    - Proxy
- **Comportamentais**, são padrões que tratam a forma como certas responsabilidades são delegadas para algumas entidades.
    - Chain of Responsibility
    - Command
    - Interpreter
    - Iterator
    - Mediator
    - Memento 
    - Observer
    - State
    - Strategy
    - Template Method
    - Visitor

## GoF's no projeto

|      Tipo      |       Padrão      | Implementado por | Explanação                                                                                                                                                                                                                                                                                                                    |
|:--------------:|:-----------------:|:----------------:|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Criacional     | *Factory Method*  | Equipe/*Django*  | Devido à criação de usuários comumente se tornar um gargalo no desenvolvimento de *software*, o *Django*, visando mitigar esse problema, fornece um módulo responsável por essa parte. O que a equipe fez foi adaptar este módulo para o contexto do projeto de forma que ele também se adequasse ao padrão *Factory Method*. |
| Estrutural     |  *Decorator*      | Equipe           | Na *feature* de gerenciamento de notícias em um dado momento é requisitado que as permissões sejam adequadas ao tipo de usuário que está logado no sistema. Para adaptar a permissão ao usuário atual foi utilizado um *decorator*.                                                                                           |
| Estrutural     | *Facade*          | *Django*         | O *Django* em sua estrutura já implementa o padrão *Facade*, o arquivo de *URL's* (gerado pelo *framework*) é onde é feito todo o gerenciamento de rotas da aplicação. Dentro do *Django* existem vários *apps* e cada um tem a sua *url*, o arquivo *urls.py* nada mais é do que uma fachada que gerencia outras fachadas.   |
| Comportamental | *Command*         | *Django*         | Visto que o *Django* utiliza *class based views* em sua estrutura, sempre que é realizada uma requisição é necessário resolvê-la. É aí que entra o padrão *command*, que trata de encapsular a requisição em um objeto.                                                                                                       |
| Comportamental | *Template Method* | *Django*         | O *Template Method* é implementado devido a utilização de *class based generic views* pelo *Django*, é possível observar isso ao alterar os passos de um algoritmo sem necessidade de mudança na sua estrutura.                                                                                                               |


## Referências

1. [Django Design Patterns and Best Practices](https://doc.lagout.org/programmation/Django/Django%20Design%20Patterns%20and%20Best%20Practices%20%5BRavindran%202015-03-26%5D.pdf)