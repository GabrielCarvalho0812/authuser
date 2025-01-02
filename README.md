# Microsserviço AuthUser (o Projeto ainda está sendo desenvolvido)

O microsserviço **AuthUser** é responsável por gerenciar a autenticação, controle de acesso e a manipulação de dados dos usuários em uma plataforma de estudos. Ele garante que apenas usuários autenticados e autorizados possam acessar recursos protegidos, além de fornecer funcionalidades para realizar operações CRUD (Criar, Ler, Atualizar, Deletar) sobre os dados dos usuários.

# Tecnologias Utilizadas (até o momento)
- **Java 17**: Linguagem de programação usada para o desenvolvimento do microsserviço.
- **Spring Boot 3.4.0**: Framework utilizado para facilitar o desenvolvimento e configuração do microsserviço.
- **Spring Data JPA**: Utilizado para interagir com o banco de dados relacional de maneira simplificada, permitindo a realização de operações CRUD.
- **PostgreSQL**: Banco de dados relacional utilizado para armazenar as informações dos usuários e dados da aplicação.
- **Spring Boot Starter Web**: Dependência que habilita a criação de serviços web RESTful, permitindo a comunicação entre o microsserviço e o cliente.
- **Spring Boot Starter Test**: Dependência usada para realizar testes automatizados no microsserviço, garantindo a qualidade do código.
- **Spring Boot Starter Validation**: Usado para validação de dados de entrada, como o cadastro de usuários, garantindo que as informações fornecidas estejam corretas.


## Funcionalidades

- **Autenticação de Usuários**: Permite que os usuários façam login na plataforma de estudos com credenciais seguras.
- **Controle de Acesso**: Garante que apenas usuários com permissões adequadas possam acessar certos recursos e funcionalidades.
- **Gestão de Dados dos Usuários**: Realiza operações CRUD sobre os dados dos usuários, como:
    - Criação de novos usuários.
    - Atualização de informações de usuários.
    - Visualização de dados de usuários.
    - Exclusão de contas de usuários.


## Endpoints Principais

- `POST /login`: Realiza a autenticação de um usuário com email e senha.
- `POST /register`: Cria um novo usuário na plataforma.
- `GET /user/{id}`: Obtém as informações de um usuário específico.
- `PUT /user/{id}`: Atualiza os dados de um usuário específico.
- `DELETE /user/{id}`: Exclui uma conta de usuário