<style> p { text-align: justify; text-indent: 30px; } </style>

| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
|18/03/2018|1.0| Justificativa Metodológica, Metodologias Tradicionais, Metodologias Ágeis, Análise Comparativa | Bernardo Henrique |


# **Justificativa Metodológica**

> “Metodologia de desenvolvimento é um conjunto de práticas recomendadas para o desenvolvimento de softwares, sendo que essas práticas, geralmente, passam por fases ou passos, que são subdivisões do processo para ordená-lo e melhor gerenciá-lo”. (Sommerville, 2000).

A etapa de definição de uma abordagem é de suma importância para qualquer empresa, afinal, esta depende de aspectos fundamentais, tais como:  qual o perfil do cliente, como serão feitas as tomadas de decisão, como serão realizados projetos, separação de setores, como será feita a organização dos funcionários e até mesmo como será o processo de trabalho de tais.

No nível de projeto a escolha de uma metodologia possui também um grande impacto, podendo definir os papéis (Scrum Master, Product Owner, Líder de time e etc.), os artefatos que serão produzidos e como será a interação com o cliente, e até entre os próprios membros. Abaixo serão abordadas duas diferentes metodologias e seus frameworks:

### **Metodologias Tradicionais:**

O foco principal das metodologias tradicionais é a previsibilidade dos requisitos do sistema, que traz a grande vantagem de tornar os projetos completamente planejados, facilitando a gerência do mesmo, mantendo sempre uma linha, caracterizando o processo como bastante rigoroso. <sub><sup>[5]</sup></sub>

Deste tipo de metodologia, o framework mais utilizado hoje em dia é o RUP <sub><sup>[5]</sup></sub>. Esta metodologia é dividida em quatro fases: Concepção, Elaboração, Construção e Transição. Cada uma  delas com focos específicos, abrangendo todo o ciclo de vida de um software.

O RUP é um processo iterativo, ou seja, atividades similares podem ocorrer em diferentes ciclos de desenvolvimento, ainda mais se tratando de alterações no projeto.

Um ponto marcante do RUP são os seus artefatos, que são produtos feitos e usados durante e depois do desenvolvimento do projeto. Estes são geralmente documentos, diagramas e modelagens.

### **Metodologias Ágeis:**

Metodologias ágeis são caracterizadas pelo fato de serem muito adaptativas e focadas em pessoas. Parte do princípio que o cliente deve estar junto ao processo de desenvolvimento e assim aprender mais sobre suas necessidades conforme o andamento do projeto, reavaliando suas necessidades e prioridades.

Há muitos frameworks classificados como ágeis, que possuem princípios e propósitos ligeiramente diferentes, tais como o Extreme Programming (XP), que é focado na produção de código com maior qualidade e no menor tempo possível, e o Scrum, que parte do fundamento de que um bom projeto deve ser focado nas pessoas envolvidas nele (seus integrantes e o cliente) e na visibilidade e transparência de informações. Um framework mais atual é o SAFe, que utiliza do Scrum e possui grande escalabilidade.

O SAFe é uma metodologia ágil que foi criada focando em grandes projetos, que tem como objetivo gerenciar vários times, que trabalham para entregar uma parte do produto (PSI). Estes é separado em três partes:    

* **Portfólio:** Setor que organiza a empresa e de forma que o trabalho seja focado em um objetivo, definindo quais serão as próximas tarefas a serem executadas e medidas que serão tomadas. Também é responsável pela alocação de recursos e garantia de retorno dos projetos.
* **Programa:** É onde os times de desenvolvedores e outros recursos (como DevpOps) são direcionados para os objetivos definidos no portfólio. Esta fase é organizada de acordo com o Trem de Entregas Ágeis (ART), um modelo de trabalho que define datas, elimina empecilhos e auxilia na transparência, fazendo com que o processo de trabalho seja o mais rápido possível.
* **Time:** É composto por desenvolvedores (geralmente de 4 a 7) e um Scrum Master, o qual é responsável por fazer que o time realize seu trabalho sem problemas. Há também a presença de um único Product Owner que orienta a produção dos times, para que eles supram as necessidades dos seus clientes (este papel pode ser desempenhado pelo próprio cliente). O time, além do produto, possui artefatos definidos que devem ser entregues (como sprint backlog, sprint planing, entre outros) e eventos (stand-up meetings, sprints e etc).
<br></br><br></br>

### **Análise Comparativa: Tradicional X Ágil**

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

<br>
## **Referências:**

1. Rigby, Darrel K. et al. Embracing Agile. Disponível em: <https://hbr.org/2016/05/embracing-agile> . Acesso em: 17 de março de 2018.
2. Corrêa, George Marsicano. Processo Tradicional. 
3. Schiel, Ulchir. Rational Unified Process. Disponível em:  <http://www.wthreex.com/rup/> Acesso em: 17 de março de 2018. 
4. Mello, Moacyr. Um Caminho Seguro para o Processo de Desenvolvimento -SAFe(ScaledAgileFramework®).Dispinível em: <https://www.ibm.com/developerworks/community/blogs/rationalbrasil/entry/um_caminho_seguro_para_o_processo_de_desenvolvimento_safe_scaled_agile_framework?lang=en>. Acesso em 23 de março de 2017.> Acessado em: 17 de março de 2018.
5. Santos, Domingos de A. Desenvolvimento de Software: Processos Ágeis ou Tradicionais? Uma visão crítica. Disponível em: <http://www.enacomp.com.br/2010/cd/artigos/completos/enacomp2010_4.pdf>. Acessado em: 17 de março de 2018.
