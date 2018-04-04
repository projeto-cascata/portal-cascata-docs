<style> p { text-align: justify; text-indent: 30px; } </style>

# Plano de Gerenciamento de Tempo

| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
|02/04/2018| 1.0 | Introdução, Processo de Gerenciamento de Tempo, Regras para medição do Desempenho, Cronograma | Bernardo Henrique |  

## **1. Introdução**
O Gerenciamento de Tempo de um projeto não é nada mais que estabelecar políticas, procedimentos e documentação para planejar, desenvolver, gerenciar, executar e controlar procedimentos, atividades, e documentação. Segundo o PmBok, este plano tem como objetivo guiar todo o ciclo de vida do software, garantindo que não hajam atrasos.

<br>
## **2. Processo de Gerenciamento do Tempo**
De acordo com o David M. Cirello, são definidas cinco atividades, sendo quatro delas focadas na fase de construção e planejamento, e uma delas em monitoração e controle. Abaixo temos estas fases explicadas, com seus conceitos e atividades.<sup><sup>[2]</sup></sup>

### **2.1 Identificar as Entregas**
As entregas devem ser as forças motora de um projeto, então deve ser bem definido quais são as atividades que devem ser realizadas nestas. É importante ressaltar que as entregas devem ser facilmente identificaveis dentro do cronograma.

### **2.2 Determinar a estrutura de Tarefas**
Esta atividade pode ser chamda de lista de atividades ou rascunho inicial do projeto. Antes de adicionar informações (inicio, fim, duração) nas tarefas, deve-se lista-las, isso permite que sejam apresentadas em uma ordem mais lógica. Nesta fase também é facil identificar sub-tarefas.

### **2.3 Identificação de dependências das tarefas principais**
Depois que todas as tarefas e sub-tarefas estão definidas, pode-se traçar quais são dependencias específicas entre elas. Uma dependência significa que uma tarefa não pode começar ou terminar até que outra seja finalizada. 

### **2.4 Decisão sobre a unidade de medida do tempo**
A seleção desta unidade determina o nível de detalhe e, assim, esforço na concepção e gestão do cronograma do projeto. Alguns fatores que devem ser levador em consideração na hora desta escolha são, entre outras:

* Quais são as obrigações contratuais para relatar ou faturar pelo seu tempo e qual é a estrutura de taxas para seu contato ou projeto?
* A sua equipe será paga por hora ou com base na entrega do produto/serviço?
* Qual duração do seu projeto e quantos recursos você possui?
* Quantas entregas são?

### **2.5 Revisão constante do plano**
"Depois de ter um cronograma do projeto pronto é importante lembrar que o seu plano não é um documento estático, ao contrário, é um veículo de comunicação dinâmico; portanto o objetivo é reportar a informação contida no plano de uma maneira fácil de entender sob a perspectiva de um observador de fora" <sup><sup>[2]<sup><sup>


<br>
## **3. Regras para a Medição de Desempenho**

É fundamental o acompanhamento do desempenho do projeto. Ao realizar esta atividade, pode-se:

* Utilizar dados a fim de definir o quão atrasado ou adiantado o projeto está.
* Analisar o grau de eficácia do planejamento do projeto.
* Aperfeiçoar o replanejamento do cronograma, baseando-se em dados históricos.
* Melhorar o controle para atingir o desempenho previamente definido.

Existem diversos métodos para análise de desempenho. Nesse projeto utilizaremos o Gerenciamento de Valor Agregado (GVA). Ele baseia-se na Variação do Cronograma e no Índice de Desempenho de Prazos. 

O Índice de Desempenho de Prazos (Schedule Performance Index ou SPI) é calculado pela razão entre o Valor Agregado (VA) e o Valor Planejado (VP).

SPI = VA / VP

O resultado obtido indica a eficácia do planejamento, e pode ser interpretada como:

* SPI < 1 - Sinal de atraso no projeto.
* SPI = 1 - Eficácia plena no planejamento
* SPI > 1 - Sinal de adiantamento no projeto.

Deve-se notar que após algumas sprints será possível ter acesso a valores de Burndown e alguns SPI's, no caso de constantes atrasos com SPI's abaixo de zero e Burndowns que não acompanham a meta, deve-se considerar algumas estratégias para melhorar o desempenho da equipe.


<br>
## **4. Cronograma**
O cronograma do Projeto Cascta pode ser encontrado acessado [este link](../gerenciamento/cronograma.md).


<br>
## **Referências**
[1] PMI. Um guia do conhecimento em gerenciamento de projetos. Guia PMBOK 5a. ed. - EUA: Project Management Institute, 2013.

[2] David M. Ciriello. Estratégias para o gerenciamento do cronograma do projeto: Dicas úteis para os gerentes de projetos e membros da equipe. Disponível em: <https://brasil.pmi.org/brazil/KnowledgeCenter/Articles/~/media/C1CEEAF8C9364BAA9FAB0D7F2B92203F.ashx>. Acessado em: 03/04/2018.