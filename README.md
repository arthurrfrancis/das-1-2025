# Design e arquiterura de software 1

## Aula 26/02

[Livro Eng Soft Moderna - Cap 7] (https://engsoftmoderna.info/cap7.html)

- Maior parte dos softwares são formados por Front - End - Bd
- No Java, pacote é uma pasta (package), que é o diretório
- Pacotes são informações essenciais, principalmente para orientar um programador que está pegando o software feito
- É papel do arquiteto definir a estrutura que será utilizada
- As bibliotecas também são componentes
- APIs também devem estar na arquitetura


## Aula 27/02

- Camadas são importantes para separar responsabilidades (Ex: Front, Back e Bd)
- MVC é o mais comum (Model - View - Controller)
  - View desenha a tela
  - Controller a camada de controle faz com que os models possam ser repassados para as views e vice-versa
  - Model são os dados que vão aparecer na tela
  - A Classe entidade faz referência a uma entidade do banco de dados
  - A lógica não deve ser inserida no controlador
  
Monolito
  - Repositório único de código
  - Uso de uma única tecnologia padrão
  - Compilado, testado, único pacote
  - Deploy como um único sistema
  - Executado como um único processo no sistema operacional
  - Único banco de dados


## Aula 05/03

- Arquitetura orientada a mensagens está bem popular
- Big ball of mud é como se chama o padrão anti-arquitetural
- Padrão arquitetural = solução para um problema específico
  - MVC - Separa as responsabilidades (Model (dados) - View (tela) - Control(comportamento))
- Estilo de arquitetura = organização do projeto
- Linux possui arquitetura monolítica
- Arquitetura em camadas
  - Divisão de responsabilidade
  - Perfomance
  - Segurança
  - Manunibilidade
  - Camada de visualização
    - Possui requisitos próprios
  - Camada lógica de negócio
    - Local central para definição e atualização das regras
    - Escalar o Backend para suportar as requisições
  - Camada de persistência
    - Banco de dados relacional - consolidada
    - Resolve problemas de concorrência
    - Permite compartilhamento de dados 

## Aula 06/03

Who Needs an Architect? - https://martinfowler.com/ieeeSoftware/whoNeedsArchitect.pdf

- O que é arquitetura?
    - Segundo Fowler, Arquitetura é uma palavra que é usada quando queremos falar de design mas soar de um jeito mais importante. Já a RUP define arquitetura como "o nível mais alto de um conceito de um sistema e seu ambiente", é uma organização ou estrutura de componentes importantes interagindo com as interfaces. Porém Ralph Johnson diz que arquitetura é o conhecimento compartilhado do design de um software. Esse conhecimento diz a respeito dos componentes e como essses componentes interagem com a interface.
    
- Qual o comportamento do arquiteto da "Matrix"?
    - O arquiteto da Matrix faz todas as decisões importantes, faz elas sozinho pois pensa que o resto da equipe não possui habilidades suficientes para as decisões, e, geralmente, estas são feitas logo cedo para que todos tenham um plano para seguir.


- Qual o comportamento do arquiteto ideal?
    - O arquiteto deve estar bem atento ao que está acontecendo no projeto, procurando saber sobre problemas e tratando eles logo no início. Ele programa com o desenvolvedor
