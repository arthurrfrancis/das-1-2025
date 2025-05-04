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


## Aula 13/03

  https://integrada.minhabiblioteca.com.br/reader/books/9788550819754/epubcfi/6/22[%3Bvnd.vst.idref%3Dcap2.xhtml]!/4/2/2/1:0[%2CCAP]

  - Amplitute técninca
  - Geralmente o programador é especializado em certas tecnologias
  - O arquiteto precisa ter uma visão mais ampla, apesar de não saber tudo

## Aula 19/03

- Arquitetura é o que você não consegue pesquisar no Google
- Não existe resposta certa nem errada, o que existe são trade-offs

## Aula 23/04

-  Resumo Características Arquiteturais  https://integrada.minhabiblioteca.com.br/reader/books/9788550819754/epubcfi/6/26%5B%3Bvnd.vst.idref%3Dcap4.xhtml%5D!/4

Introdução  
Quando uma empresa desenvolve um software para resolver um problema, além dos requisitos funcionais, os arquitetos precisam considerar as características da arquitetura — aspectos críticos que influenciam o design e o sucesso do sistema, mas que não estão diretamente ligados ao domínio do problema.  

O que são Características da Arquitetura?  
São critérios de design que:  
1. Vão além do domínio
2. Influenciam a estrutura do sistema
3. São essenciais para o sucesso da aplicação

Exemplos: desempenho, segurança, escalabilidade, manutenibilidade

Terminologia  
- Requisitos não funcionais: Termo comum, mas considerado depreciativo
- Atributos de qualidade: Termo usado, mas sugere avaliação posterior, não design
- Características da arquitetura: Termo preferido, pois destaca sua importância crítica

Classificação das Características da Arquitetura  
1. Operacionais:  
   - Disponibilidade, desempenho, recuperabilidade, escalabilidade
2. Estruturais:  
   - Modularidade, reutilização, manutenibilidade, portabilidade
3. Transversais: 
   - Segurança, acessibilidade, conformidade legal

Desafios e Trade-offs  
- Interdependência: Melhorar uma característica pode prejudicar outra
- Complexidade: Adicionar muitas características aumenta a complexidade do design
- Arquitetura "menos pior": Não existe uma solução perfeita; o objetivo é equilibrar as necessidades

Padrões e Ambiguidades  
- Não há uma lista universal de características da arquitetura
- Termos como interoperabilidade e compatibilidade podem ter significados diferentes em contextos distintos
- Organizações como a ISO tentam padronizar, mas as definições ainda são flexíveis

Conclusão  
Arquitetos devem:  
- Identificar as características mais relevantes para o projeto
- Equilibrar trade-offs para evitar soluções superdimensionadas
- Adotar abordagens iterativas, permitindo ajustes conforme o sistema evolui
A arquitetura de software não busca a perfeição, mas sim a melhor solução possível dentro das restrições e necessidades do projeto.
  

## Aula 24/4 

- Resumo Fundamentos da Arquitetura de Software https://integrada.minhabiblioteca.com.br/reader/books/9788550819754/epubcfi/6/38%5B%3Bvnd.vst.idref%3Dcap9.xhtml%5D!/4

### Fundamentos dos Estilos de Arquitetura de Software  

Os estilos de arquitetura, também chamados de padrões de arquitetura, descrevem formas nomeadas de organizar componentes de software, abrangendo diversas características arquiteturais. Esses estilos funcionam como atalhos para arquitetos experientes, permitindo discussões rápidas sobre estrutura, pontos fortes, fraquezas e estratégias de implementação.  

 Estilos Fundamentais  

1. Grande Bola de Lama (Big Ball of Mud)
   - Sistema sem estrutura definida, com código desorganizado e acoplamento excessivo 
   - Problemas: Dificuldade de manutenção, escalabilidade e testabilidade
   - Comum em sistemas que cresceram sem governança

2. Arquitetura Unitária
   - Todo o software roda como uma única unidade, comum em sistemas embarcados ou restritos
   - Limitações: Dificuldade em escalar ou adicionar funcionalidades complexas

3. Cliente/Servidor
   - Separa front-end (cliente) e back-end (servidor)
   - Variações:  
     - Desktop + banco de dados
     - Navegador + servidor web

4. Três Camadas
   - Camada de apresentação, lógica de negócio e dados
   - Popular em sistemas corporativos dos anos 1990/2000

Monolítico vs. Distribuído  

1. Monolítico
   - Todo o código é implementado como uma única unidade
   - Exemplos:
     - Arquitetura em Camadas
     - Pipeline
     - Microkernel

3. Distribuído  
   - Componentes independentes comunicando-se via rede
   - Exemplos: 
     - Baseada em Serviços
     - Orientada a Evento
     - Baseada em Espaços
    
Falácias da Computação Distribuída  

1. A rede é confiável
   - Problemas de conexão podem causar falhas inesperadas

2. A latência é zero
   - Chamadas remotas são mais lentas que locais

3. A largura de banda é infinita 
   - Tráfego excessivo entre serviços pode congestionar a rede

4. A rede é segura*
   - Cada endpoint distribuído precisa de proteção adicional

5. A topologia nunca muda
   - Alterações na infraestrutura afetam a comunicação

6. Existe apenas um administrador
   - Coordenação entre múltiplas equipes é complexa

7. O custo do transporte é zero
   - Infraestrutura distribuída exige mais hardware e configuração

8. A rede é homogênea
   - Dispositivos de diferentes fabricantes podem ter incompatibilidades

Outros Desafios em Sistemas Distribuídos  
- Log distribuído: Dificuldade em rastrear erros em múltiplos serviços
- Transações distribuídas: Consistência eventual em vez de ACID
- Versionamento de contratos: Manter compatibilidade entre APIs evolutivas

Conclusão  
Escolher um estilo arquitetural envolve trade-offs entre simplicidade, escalabilidade e resiliência. Arquiteturas monolíticas são mais simples, enquanto distribuídas oferecem flexibilidade, mas exigem lidar com complexidades de rede. O entendimento desses fundamentos ajuda arquitetos a tomar decisões equilibradas.
