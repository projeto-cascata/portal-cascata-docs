### Histórico da Revisão

| Data  | Versão |                  Descrição                  |    Autor     |
| :---: | ------ | :-----------------------------------------: | :----------: |
| 03/04 | 0.1    |     Criação e estruturação do documento     | Daniel Teles |
| 03/04 | 0.2    |                 Introdução                  | Daniel Teles |
| 03/04 | 0.3    |         Representação Arquitetural          | Daniel Teles |
| 03/04 | 0.4    |             Metas e Restrições              | Daniel Teles |
| 03/04 | 0.5    | Qualidade e link para o Diagrama de Classes | Daniel Teles |
| 03/04 | 0.6    |        Refatorando finalidade e escopo      | Letícia de Souza |
| 04/04 | 0.7    | Refatorando Representação Arquitetural      | Letícia de Souza |
| 04/04 | 0.8    | Reescrevendo Metas e Restrições de Arquitetura| Letícia de Souza |
| 04/04 | 0.9    | Preenchendo campo de Visão Lógica e Qualidade | Letícia de Souza

## **Sumário**

[1. Introdução](#1-introdu%C3%A7%C3%A3o)

* [1.1 Finalidade](#11-finalidade)

* [1.2 Escopo](#12-escopo)

* [1.3 Definições, Acrônimos e Abreviações](#13-defini%C3%A7%C3%B5es-acr%C3%B4nimos-e-abrevia%C3%A7%C3%B5es)

[2. Representação Arquitetural](#2-representa%C3%A7%C3%A3o-arquitetural)

[3. Metas e Restrições da Arquitetura](#3-metas-e-restri%C3%A7%C3%B5es-da-arquitetura)

[4. Visão de Casos de Uso](#4-vis%C3%A3o-de-casos-de-uso)

[5. Visão Lógica](#5-vis%C3%A3o-l%C3%B3gica)

* [5.1 Diagrama de Classes](#51-diagrama-de-classes)

[6. Qualidade](#6-qualidade)

## **1. Introdução**

### **1.1. Finalidade**

Este documento oferece uma visão geral da arquitetura do sistema, utilizando diversas visões arquiteturais para representar diferentes aspectos do sistema. O objetivo deste documento é capturar e comunicar as decisões arquiteturais significativas, trazendo uma melhor compreensão dos requisitos e forma do projeto.

### **1.2 Escopo**

A aplicação web Portal Cascata tem por objetivo solucionar alguns dos problemas enfrentados pelos alunos da UnB que se dedicam ao projeto Cascata, que visa ajudar alunos oriundos da rede pública de ensino no processo de preparação para vestibulares. Dentre os problemas enfrentados pelos participantes do projeto atualmente, está a falta de centralização da comunicação e de um local para a postagem de materiais e notícias. Sendo assim, este documento rege os paradigmas arquiteturais que serão aplicados ao software, além de proporcionar uma visão mais abrangente do Portal Cascata, explorando seus aspectos, explicitando as tecnologias utilizadas e auxiliando na objetividade do desenvolvimento.

### **1.3 Definições, Acrônimos e Abreviações**

Alguns termos utilizados nesse documento, são oriundos de uma língua estrangeira, são abreviações ou acrônimos.

* **RUP**: Rational Unified Process - Metodologia atualmente mantida pela IBM que visa ser customizável, prevê a colaboração entre as equipes e busca a qualidade na processo de criação de um software.
* **UML**: Unified Modelling Language - Linguagem de representação de modelos, apresentados de forma padronizada e independente de uma linguagem de programação.
* **Python**: Python é uma linguagem de programação de alto nível, interpretada, de script, imperativa, orientada a objetos, funcional, de tipagem dinâmica e forte.
* **Django**: É um Framework Python de alto nível que encoraja o desenvolvimento rápido e limpo. Construído por desenvolvedores experientes é gratuito e de código-aberto.

## **2. Representação Arquitetural**

A arquitetura proposta seguirá o padrão Model, Template, View, própria do Django e aderente ao MVC. Utilizando este padrão iremos separar estruturalmente a interação com o usuário das regras de negócio facilitando o mapeamento do domínio e a manutenção da aplicação.
As camadas serão utilizadas da seguinte forma:

* **Model**: As models do MVC e do Mvt possuem responsabilidades equivalentes. Cada classe da Model se compora a uma tabela do banco de dados, enquanto as instâncias dessas classes, representam os registros dessas tabelas. Nesta camada será possível definir o domínio da aplicação e as especificações a respeito dos dados (como validar, acessar, comportamentos e as relações entre os dados).
* **Template**: Será a responsável por toda a parte visual e de interação com o aplicativo, incluindo layouts e telas para mapear as entradas dos usuário.
* **View**: Será a camada central da estrutura realizando a comunicação entre as duas outras camadas, responsável por trafegar as informações entre camadas com segurança.

![MTV Architecture](https://user-images.githubusercontent.com/22121504/29645196-4481529c-8852-11e7-90c4-d0bc8bd62193.jpg)
Figura 1: Diagrama simplificado de apresentação do MTV

## **3. Metas e Restrições da Arquitetura**

<table style="width:100%">
  <tr>
    <td align="center"><b>Metas</b></td>
    <td align="left">A aplicação deve ser eficiente e atender bem aos recursos do sistema respondendo às requisições rapidamente. Além disso, atender a requisitos não funcionais como facilidade de manutenção, estruturando o código de maneira organizada, visando a manutenabilidade do sistema. </td>
  </tr>
  <tr>
    <td align="center"><b>Restrições de Arquitetura</b></td>
    <td align="left">O software será funcional em navegadores que possuem acesso à internet. Será utilizado a ferramenta virtualenv para a criação de um ambiente virtual para nosso programa, juntamente com o Python3 e o Django. Além disso, será adotado como ferramenta para o banco de dados o PostgreSQL.</td>
  </tr>
  </table>


## **4. Visão de Casos de Uso**

| Atores | Descrição |
|:------:|---------|
|  Aluno | O aluno consumirá os serviços providos pela portal, dentro de suas permissões, como visualizar notícias e materiais, bem como justificar faltas. |
| Membro interno do projeto | O membro poderá realizar o controle de frequência dos alunos e alimentar a plataforma com materiais relacionados às disciplinas ministradas, bem como postar notícias a respeito do projeto.


## **5. Visão Lógica**

O Portal Cascata utiliza a base da arquitetura MTV e design responsivo, em que o site se adapta ao browser do usuário. Os dois tipos de usuários, quando acessarem o site, terão contato com a view, que realizará uma requisição, executando as ações lógicas.

### **5.2 Pacotes de Design Significativos do Ponto de Vista da Arquitetura**

### **5.3 Diagrama de classes**

![Diagrama de Classes](https://raw.githubusercontent.com/projeto-cascata/portal-cascata-docs/arquitetura/docs/img/Classes/class_diagram.png)
Figura 2: [Diagrama de classes](https://github.com/projeto-cascata/portal-cascata-docs/blob/arquitetura/docs/arquitetura/diagrama_classes.md)

## **6. Qualidade**

O uso da arquitetura MTV, que é necessária devido à utilização do Django, propõe uma maneira de organização das camadas da aplicação que as tornam mais independentes e torna o código mais compreensível e manutenível. Além disso, é uma arquitetura com uma grande comunidade, difundida e utilizada.
