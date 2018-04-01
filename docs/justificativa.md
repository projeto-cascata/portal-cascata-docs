<style> p { text-align: justify; text-indent: 30px; } </style>

# Justificativa Metodológica

## Histórico de Revisão

| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
|18/03/2018|1.0| Justificativa Metodológica, Metodologias Tradicionais, Metodologias Ágeis, Análise Comparativa | Bernardo Henrique |   

---

## **Introdução a Problemática**   

Os interessados para a execução do produto são os membros do Projeto Cascata. Este projeto surgiu da ideia de ingressos da Universidade de Brasília, campus Gama, que viram a dificuldade de alguns alunos da rede de escolas públicas em conseguir material e cursos preparatórios para o vestibular, desta forma estes universitários, de forma voluntária, trabalham de maneira a ministrar aulas e expor materiais para ajudar os alunos carentes no processo de estudo para o vestibular.

Com o atendimento de vários alunos e voluntários por este projeto, ficou claro para eles a necessidade de controlar a distribuição de materiais e a frequência dos alunos e dos membros internos e divulgar informações para estes.

Logo, o produto pedido é uma plataforma para acesso dos membros voluntários, para justificar suas faltas e controlar a frequência dos alunos, sendo esses recursos restritos, além de divulgação de informativos para a comunidade. Assim, necessitamos uma metodologia de projeto, para fazer com que o produto seja entregue da melhor maneira possível, tanto para a equipe quanto para o cliente. 

</br>

## **Justificativa Metodológica**

> “Metodologia de desenvolvimento é um conjunto de práticas recomendadas para o desenvolvimento de softwares, sendo que essas práticas, geralmente, passam por fases ou passos, que são subdivisões do processo para ordená-lo e melhor gerenciá-lo”. (Sommerville, 2000).

A etapa de definição de uma abordagem é de suma importância para qualquer empresa, afinal, esta depende de aspectos fundamentais, tais como:  qual o perfil do cliente, como serão feitas as tomadas de decisão, como serão realizados projetos, separação de setores, como será feita a organização dos funcionários e até mesmo como será o processo de trabalho de tais.

No nível de projeto a escolha de uma metodologia possui também um grande impacto, podendo definir os papéis (Scrum Master, Product Owner, Líder de time e etc.), os artefatos que serão produzidos e como será a interação com o cliente, e até entre os próprios membros. Abaixo serão abordadas duas diferentes metodologias e seus frameworks:

### **Metodologias Tradicionais**

O foco principal das metodologias tradicionais é a previsibilidade dos requisitos do sistema, que traz a grande vantagem de tornar os projetos completamente planejados, facilitando a gerência do mesmo, mantendo sempre uma linha, caracterizando o processo como bastante rigoroso. <sub><sup>[5]</sup></sub>

Deste tipo de metodologia, o framework mais utilizado hoje em dia é o RUP <sub><sup>[5]</sup></sub>. Esta metodologia é dividida em quatro fases: Concepção, Elaboração, Construção e Transição. Cada uma  delas com focos específicos, abrangendo todo o ciclo de vida de um software.

O RUP é um processo iterativo, ou seja, atividades similares podem ocorrer em diferentes ciclos de desenvolvimento, ainda mais se tratando de alterações no projeto.

Um ponto marcante do RUP são os seus artefatos, que são produtos feitos e usados durante e depois do desenvolvimento do projeto. Estes são geralmente documentos, diagramas e modelagens.

Para melhor funcionamento do projeto, decidimos adequar a nossa metodologia os artefatos comumente utilizados pelo RUP. Os artefatos escolhidos foram:
  
  * Documento de Visão: descreve, em linguagem natural o problema proposto, a solução e seus possíveis concorrentes e também é listado
  os requisitos funcionais que devem ser atentidos para o funcionamento do sistema e a satisfação do cliente;
  * Documento de Arquitetura: relata a arquitetura que deve ser aderir para a melhor estruturação do produto de software;
  * Diagrama de Classe: que nos dá a visão de implementação do projeto;
  * Diagramas de Caso de Uso: que representa o fluxo de funcionamento de um requisito específico, assim como seus atores;
  * Diagrama de Sequência: retrata a interação entre componentes, mas está focado na sequência de mensagens, suas entradas e saídas. 

### **Metodologias Ágeis**

Metodologias ágeis são caracterizadas pelo fato de serem muito adaptativas e focadas em pessoas. Parte do princípio que o cliente deve estar junto ao processo de desenvolvimento e assim aprender mais sobre suas necessidades conforme o andamento do projeto, reavaliando suas necessidades e prioridades.

Há muitos frameworks classificados como ágeis, que possuem princípios e propósitos ligeiramente diferentes, tais como o Extreme Programming (XP), que é focado na produção de código com maior qualidade e no menor tempo possível, e o Scrum, que parte do fundamento de que um bom projeto deve ser focado nas pessoas envolvidas nele (seus integrantes e o cliente) e na visibilidade e transparência de informações. Um framework mais atual é o SAFe, que utiliza do Scrum e possui grande escalabilidade.

O SAFe é uma metodologia ágil que foi criada focando em grandes projetos, que tem como objetivo gerenciar vários times, que trabalham para entregar uma parte do produto (PSI). Estes é separado em três partes:    

* **Portfólio:** Setor que organiza a empresa e de forma que o trabalho seja focado em um objetivo, definindo quais serão as próximas tarefas a serem executadas e medidas que serão tomadas. Também é responsável pela alocação de recursos e garantia de retorno dos projetos.
* **Programa:** É onde os times de desenvolvedores e outros recursos (como DevpOps) são direcionados para os objetivos definidos no portfólio. Esta fase é organizada de acordo com o Trem de Entregas Ágeis (ART), um modelo de trabalho que define datas, elimina empecilhos e auxilia na transparência, fazendo com que o processo de trabalho seja o mais rápido possível.
* **Time:** É composto por desenvolvedores (geralmente de 4 a 7) e um Scrum Master, o qual é responsável por fazer que o time realize seu trabalho sem problemas. Há também a presença de um único Product Owner que orienta a produção dos times, para que eles supram as necessidades dos seus clientes (este papel pode ser desempenhado pelo próprio cliente). O time, além do produto, possui artefatos definidos que devem ser entregues (como sprint backlog, sprint planing, entre outros) e eventos (stand-up meetings, sprints e etc).

Como dito, esta metodologia possui a característica de ser escalável e de ser possível a adaptação para diversas equipes. Para o desenvolvimento do produto de software proposto, foi decidido que concentraremos os integrantes do grupo na parte de <b>Time</b> do SAFe, assim como utilizaremos as práticas adotas por equipes nesse fase que é o <i>ScrumXP</i>.

O <i>ScrumXP</i> é uma combinação de práticas de duas metodologias diferentes, , que encaixam muito bem para equipes auto-organizáveis do SAFe. Esta possui os papéis encontrados no <i>Scrum</i>, como <i>Product Owner</i>, caracterizado como representante do cliente na equipe e responsável pelo o produto de software e único que pode classificar uma história de usuário como concluída. O <i>Scrum Master</i>, que lida com o <b>Time</b> e mantem o desenvolvimento, tratando com os empecilhos caso ocorra. Do <i>Scrum</i> também se leva alguns artefatos, como as <i>Histórias de Usuário</i> que são os requisitos coletados do cliente escritas de maneira a ser possível atribuir valores, assim definir prioridades de execução, e também a atividade de <b>Iterações (Sprints)</b>, que nada mais é do que intevalos de tempo definidos pela equipe para realizar histórias de usuário seleciodas pelo <i>Product Owner</i>,.

Atrelado ao <i>Scrum</i>, temos a <i>XP (Extreme Programming)</i>, que disponhe de práticas como <i>Feedback</i>, ou seja, a comunicação entre a equipe para reportar acontecimentos que ocorreram durante a iteração, a <i> Programação Pareada</i> e a <i>Integração e Entrefa Contínua</i>.

Para finalizar, O SAFe adota estas práticas juntamente como o <i>Kanban</i>, que organiza as tarefas da equipe em um quadro geralmente dividido em tarefas a fazer, que estão acontecendo e aquelas que já foram terminadas, orientando assim o <i>Time</i>.

Especifico desta metodologia, levaremos sua estruturação de setores.
<br>

## **Análise Comparativa: Tradicional X Ágil**

A utilização de abordagens, como já falado, é uma questão situacional da equipe, empresa projeto e outros fatores. Os principais aspectos que devem ser levados em consideração são:

| Aspecto | Metodologias Ágeis | Metodologias Tradicionais |
|---|---|---|
| Ambiente de Mercado | Preferências do usuário e opções de soluções mudam frequentemente.      | Condições do mercado são estáveis e previsíveis. |    ||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||
| Envolvimento do Usuário e Cliente                    | Colaboração estreita e rápido feedback são possíveis. Usuários conseguem visualizar melhor o que querem de acordo com o progresso do projeto. | Requisitos são claros desde o início e se mantém estáveis. Clientes não estão disponíveis para colaborar constantemente. ||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||
| Necessidade de Inovação e Conhecimento da Equipe | Problemas são complexos e soluções desconhecidas pela equipe. Especificações do produto podem mudar. Colaboração multifuncional é vital. | Trabalho similar já foi feito antes, tendo solução clara. Especificações detalhadas e planos de trabalho são confiáveis para serem seguidos. ||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||
| Modularização do Trabalho | Desenvolvimento incremental é valorizado e podem ser usados pelo usuário. Mudanças tardias são gerenciáveis. | Clientes não podem começar a testar partes do produto antes de finalizado. Mudanças tardias são caras ou impossíveis. |||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||
| Impacto de erros provisórios | Proporcionam aprendizado para a equipe. | Podem ser catastróficas. ||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||

O IBM Certified IT Specialist, Moacyr Mello, em seu texto “Um Caminho Seguro para o Processo de Desenvolvimento - SAFe (Scaled Agile Framework®)” <sub><sup>[4]</sup></sub> cita que o framework SAFe dá ênfase no gerenciamento de requisitos; e este foi, inclusive, idealizado por Dean Lenffingwell, responsável por uma famosa ferramenta de gestão de requisitos nos anos 90. Os conceitos de histórias de usuário e épicos presentes nesse framework  ampliam a forma de capturar requisitos, melhor adequados à ênfase em colaboração, flexibilidade e iterações de projeto mais curtas.

É importante adaptar corretamente o processo de desenvolvimento para as necessidades reais do projeto. A quantidade de cerimônias, precisão e controle devem ser detalhadas de acordo com uma variedade de fatores, incluindo tamanho e distribuição da equipe, quantidade de restrições impostas e a fase no qual o projeto se encontra. <sub><sup>[2]</sup></sub>

Portanto, como consequência destas metologias apresentadas, o problema proposto e equipe disponível para a execução do projeto, foi delineado que a junção de artefatos e procedimentos de ambas, assim como citado anteriormente.
<br></br>

## **Referências**

1. Rigby, Darrel K. et al. Embracing Agile. Disponível em: <https://hbr.org/2016/05/embracing-agile> . Acesso em: 17 de março de 2018.
2. Corrêa, George Marsicano. Processo Tradicional. 
3. Schiel, Ulchir. Rational Unified Process. Disponível em:  <http://www.wthreex.com/rup/> Acesso em: 17 de março de 2018. 
4. Mello, Moacyr. Um Caminho Seguro para o Processo de Desenvolvimento -SAFe(ScaledAgileFramework®).Dispinível em: <https://www.ibm.com/developerworks/community/blogs/rationalbrasil/entry/um_caminho_seguro_para_o_processo_de_desenvolvimento_safe_scaled_agile_framework?lang=en>. Acesso em 23 de março de 2017.> Acessasdo em: 17 de março de 2018.
5. Santos, Domingos de A. Desenvolvimento de Software: Processos Ágeis ou Tradicionais? Uma visão crítica. Disponível em: <http://www.enacomp.com.br/2010/cd/artigos/completos/enacomp2010_4.pdf>. Acessado em: 17 de março de 2018.
6. Scaled Agile Framework, ScrumXP. Diponível em: http://www.scaledagile.com/permissions-form/https://www.scaledagileframework.com/scrumxp/.  Acessado em: 29 de março de 2018.
7. Scaled Agile Framework, Agile Team. Diponível em: http://www.scaledagile.com/permissions-form/https://www.scaledagileframework.com/agile-teams/.  Acessado em: 29 de março de 2018.
8. Programação Extrema.  Diponível em: https://github.com/fga-gpp-mds/A-Disciplina/wiki/Programa%C3%A7%C3%A3o-Extrema-(XP). Acessado em: 29 de março de 2018.