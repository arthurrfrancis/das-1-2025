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
