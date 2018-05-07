# ** Sprint 0 **

Número da Sprint: 0

Data de Início: 06/04/2017

Data de Término: 20/04/2017

Duração: Quatorze Dias (Duas Semanas)

Scrum Master: Bernardo Henrique

## ** 1. Pareamento** 

![Pareamento Sprint 0](../img/sprints/pareamentoSprint0.png)


## ** 1. Planejamento das Histórias ** 
Para esta sprint foram constatadas depedências entre features, sendo então focada a feature E1FE1 - Manter Usuários. Sendo as histórias de usuário planejadas derivando desta. 

Além das histórias de usuário, foram realizadas também algumas histórias técnicas, que por sua vez foram importantes para manter a continuidade da entrega de valor (como dockerizar aplicação), melhorar o SGBD (migrar o banco de dados do projeto para postgree) e mudanças no layout.


## ** 2. Histórias de Usuário **


### ** US01 Realizar Login  ** 
** Descrição: ** Eu, como usuário, desejo realizar login no sistema para ter acesso às minhas funcionalidades no sistema.

** Critérios de Aceitação: **

As matrículas devem possuir os dois primeiros dígitos correspondentes aos do ano atual.

Validar os campos do registro.

Verificar se o usuário já existe.

** Responsáveis: ** Bernardo Henrique, Felipe Hargreaves e Mariana Pícolo.
<br><br>


### ** US07 Ver perfil ** 
** Descrição: ** Eu, como membro do projeto, desejo ver o perfil de outros usuários do sistema para que eu possa ter acesso aos seus dados.

** Critérios de Aceitação: **

Exibir o perfil de um aluno;

Exibir o perfil de um administrador.

** Responsáveis: ** Clarissa Lima e Mariana Pícolo.
<br><br>


### ** US08 Ver Meu Perfil ** 
** Descrição: ** Eu, como usuário, desejo ver o meu perfil para que eu possa verificar os meus dados.

** Critérios de Aceitação: **

Devem ser exibidos campos de nome, matrícula, e-mail e telefone, além de uma possível foto enviada pelo usuário.

** Responsáveis: ** Clarissa Lima e Felipe Hargrives.
<br><br>



### ** US09 Listar Membros ** 
** Descrição: ** Eu, como membro do projeto, desejo listar os membros para ter acesso a todos os membros cadastrados no sistema.

** Critérios de Aceitação: **

Deve ser possível buscar os membros listados pelo nome.

** Responsáveis: ** Bernardo Henrique e Daniel Teles.
<br><br>


### ** US19 Ver notícia detalhadamente ** 
** Descrição: ** Eu, como usuário, desejo ter uma visão detalhada de uma notícia escolhida na lista de notícias para que eu possa ler a notícia por completo.

** Critérios de Aceitação: **

Apenas os grupos de usuários apropriados terão permissão para acessar notícias (admin, diretores, RH).

** Responsáveis: ** Halê Valente e Mariana Pícolo.
<br><br>



### ** US38 Enviar convite de cadastro ** 
** Descrição: ** Eu, como administrador, desejo enviar um convite de acesso ao sistema para que um usuário possa se cadastrar.


** Responsáveis: ** Clarissa Lima e Leticia Souza.
<br><br>


## ** 3. Histórias Técnicas **

** Migrar Banco de Dados do Projeto: ** Mudança do SGBD do projeto para que se torne mais robusto.

** Mudança no Layout do Admin: ** Mudança na apresentação das informações da página de administração do projeto.

** Criar Navbar: ** Criação de Navbar para que haja navegabilidade no projeto.

** Padronizar Usuário: ** Usuário padronizado para o usuário padrão do Django, facilitando o processo de login no sistema.

** Dockerizar Aplicação: ** Adição do Docker para facilitar a ambientação da aplicação.
<br><br>


## ** 4. Fechamento da Sprint **
| Histórias Planejadas | Status |
|----------------------|--------|
| US01: Realizar Login | ** Completo ** |
| US07: Ver perfil  | Incompleto | 
| US08: Ver Meu Perfil | ** Completo ** |  
| US09: Listar Membros | ** Completo ** |  
| US19: Ver notícia detalhadamente | Incompleto |  
| US38: Enviar convite de cadastro | Incompleto |  

| Histórias Técnicas | Status |
|----------------------|--------|
| Migrar Banco de Dados do Projeto | ** Completo ** |
| Mudança no Layout do Admin  | ** Completo ** | 
| Criar Navbar | ** Completo ** |  
| Padronizar Usuário | ** Completo ** |  
| Dockerizar Aplicação | ** Completo ** | 



## ** 5. Análise do Scrum Master **
Nesta sprint, foram realizadas cinco histórias técnicas e três, das seis, histórias de usuário planejadas. Estas histórias não foram entregues pelos seguintes fatos: 

* Durante o período da Sprint 0 os membros se encontraram atarefados com outras disciplinas.
* Alguns membros possuem dificuldade na tecnologia usada.
* Dificuldade de encontrar horários com a dupla de pareamento.


A não entrega das tarefas pode dificultar o desenvolvimento das tarefas a seguir, uma vez que as histórias priorizadas para essa sprint são base para o restante do software. As histórias que não foram concluídas serão replanejadas para as próximas sprints.