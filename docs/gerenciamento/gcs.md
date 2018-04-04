<style> p { text-align: justify; text-indent: 30px; } </style>

# Plano de Gerenciamento de Configuração de *Software*

| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
|03/04/2018| 1.0 | Plano de Gerenciamento de Configuração de *Software* | Felipe Hargreaves, Mariana Pícolo | 

---   

## **1. Políticas adotadas**

### **1.1 Política de *branches* **

O projeto possuirá duas *branches* principais: a *master*, que conterá a versão mais estável do código, apenas com funcionalidades finalizadas, e a *development*, que conterá a versão de desenvolvimento. Quando uma funcionalidade for finalizada, esta deverá ser submetida à *branch development*, e, posteriormente, para a *master*, através de *pull request*. 
Nenhum *commit* deve ser realizado diretamente nestas *branches*, que estarão protegidas de publicações forçadas (*push force*).

A nomenclatura deve seguir o padrão "*CamelCase*". Entre o número e a descrição da história deve haver um hífen.   

> US01-LoginAluno    

O nome da *branch* deve referenciar a **História de Usuário** de acordo com seu *id*, (por exemplo: US01), seguido do nome referente ao que está sendo implementado, como "*Login*", por exemplo.   

> US01-Login    

O nome da *branch* deve referenciar a **História Técnica** de acordo com seu *id*, (por exemplo: TS01), seguido do nome referente ao que está sendo implementado, como "IntegrationAPI", por exemplo.
>TS01-IntegrationAPI


O nome da *branch* deve referenciar a correção que será feita em alguma história, com o uso de seu *id*, e o prefixo **“FIX”**.
> [FIXUS01]-LoginValidation


### **1.2 Política de *Commits* **

Os *commits* devem ser atômicos, com um objetivo bem explicitado. Devem corresponder a um conjunto funcional que represente parte da funcionalidade sendo desenvolvida.
  -  Sendo viável, grupos de *commits* considerados demasiadamente pequenos por si só poderão ser aglutinados (*squash*) antes de serem submetidos às *branches* principais.

O idioma padrão para as mensagens de *commit* no repositório de código é o inglês.

As mensagens de *commit* devem começar com verbo no infinitivo:
> “*Add login form authorization*”

Ao invés de:     

> “*Adding login form authorization*”    

Para commits com muitas alterações utilizar “*git commit*.”

### **1.2.1 *Commits* em Pares**

*Commits* realizados em duplas (ou grupos maiores) devem possuir a assinatura de todos os envolvidos. Para isto, se fará uso da opção **Co-authored-by**, através dos seguintes passos:   
Após adicionar todos os arquivos modificados, executar o comando de *commit* sem *tags* adicionais:    
> git commit    

O editor de texto configurado como padrão para o *Git* abrirá. Digite a mensagem de *commit*, e, com duas linhas em branco de separação, bote as assinaturas dos participantes. Exemplo:

```
Add commit example


Co-authored-by: Felipe Hargreaves <fhargreaves00@gmail.com>
Co-authored-by> Mariana Picolo <mariananpicolo@gmail.com> 
``` 

Opta-se pelo uso de *co-authored-by* ao invés de *signed-off-by* por manter um melhor registro dos participantes no histórico de *commits* e gráficos de participação do *Github*.
