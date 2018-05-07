# Padrões GRASP

## Introdução
O GRASP, sigla para General Responsibility Assignment Software Patterns, consiste em uma série de diretrizes relacionadas à atribuição de responsabilidades a classes e objetos em sistemas de software orientados a objetos, expressadas nos seguintes padrões:

- Especialista
- Criador
- Alta Coesão
- Baixo Acoplamento
- Polimorfismo
- Fabricação Pura
- Indireção
- Controller
- Variações Protegidas

A seguir se mostra a aplicação desses padrões na implementação do projeto.

# Criador
O padrão criador trata da responsabilidade de criação de objetos. Mais especificamente, delega a responsabilidade de criação a uma classe distinta. Pode se notar a aplicação desse conceito no sistema de usuários da aplicação, com as classes *Account* e *AccountManager*, onde AccountManager é responsável pela criação de objetos Conta.

# Alta Coesão
Padrão que visa manter os objetos com um foco apropriado, de forma que suas responsabilidades sejam relacionadas e focadas, facilitando o entendimento e manutenção do código. Esse princípio foi facilitado pelo uso do Django como framework de escolha, pela grande modularização que o mesmo proporciona. Nota-se a separação das diversas partes da aplicação em *apps*, cada um responsável por um módulo específico do sistema, como o app de Usuários, de Notícias, etc. Essa coesão ainda é mantida dentro de cada app, ao se delimitar classes específicas para Models, Forms, Views, entre outros aspectos.

# Baixo Acoplamento
O princípio do Baixo Acoplamento visa melhorar a manutenibilidade do sistema, ao garantir que os elementos da aplicação não estejam fortemente dependentes ou conectados uns aos outros. Novamente, a escolha do Django como framework facilita a aplicação deste padrão, devido à grande modularização do projeto. Pode se usar como exemplo o próprio modelo arquitetural garantido pelo Django, Model-View-Template (MTV), que faz uma separação clara entre o domínio (Model), a exibição dos dados (Template) e a comunicação entre as duas camadas (View).

# Indireção
O padrão da indireção auxilia com o baixo acoplamento entre dois elementos ao atribuir a um objeto intermediário a responsabilidade de mediação entre eles. O exemplo mais comum desse padrão é a popular arquitetura Model-View-Controller (MVC).

Como já mencionado, o Django faz uso do MTV, que pode ser visto como uma adaptação do MVC clássico. A ideia da indireção permanece, no entanto, com a View sendo a mediadora entre os dados (Model) e a apresentação dos mesmos (Templates).


