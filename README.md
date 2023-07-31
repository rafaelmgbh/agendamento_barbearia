# Projeto de Portfolio: Sistema de Agendamento para Barbearia
## Descrição do Projeto

O projeto consiste em desenvolver um sistema de agendamento para uma barbearia, permitindo que os clientes possam agendar horários de cortes de cabelo com os profissionais disponíveis. Os profissionais, por sua vez, poderão visualizar sua agenda e atualizar o status dos agendamentos.

O sistema será construído utilizando o framework FastAPI em Python para criar a API que será responsável por gerenciar as operações de agendamento e a interação com o banco de dados PostgreSQL. O Alembic será utilizado para gerenciar as migrações do banco de dados, garantindo que o esquema do banco de dados seja mantido atualizado.

O front-end do sistema será desenvolvido utilizando a biblioteca React para criar uma interface de usuário interativa e amigável. O React será responsável por consumir a API do backend e apresentar as informações para os clientes e profissionais da barbearia.

### Requisitos Funcionais

    Os clientes devem poder se cadastrar no sistema.
    Os profissionais da barbearia devem poder se cadastrar no sistema.
    Os clientes devem poder visualizar a agenda disponível com os horários livres dos profissionais.
    Os clientes devem poder selecionar um horário disponível e marcar um agendamento com um profissional específico.
    Os profissionais devem poder visualizar sua agenda com os agendamentos marcados.
    Os profissionais devem poder atualizar o status de um agendamento (iniciado o corte, concluído, etc.).
    Os clientes e profissionais devem poder visualizar o histórico de agendamentos anteriores.

### Requisitos Não-Funcionais

    O sistema deve ser implementado em Python.
    O banco de dados a ser utilizado é o PostgreSQL.
    O framework web a ser utilizado é o FastAPI para construir as APIs.
    O Alembic será utilizado para versionamento do banco de dados.
    O sistema será empacotado em um contêiner Docker para facilitar a implantação.

### Configuração do Ambiente de Desenvolvimento

    Instale o Python na versão compatível com o FastAPI (recomendado Python 3.7 ou superior).
    Instale o PostgreSQL e crie um banco de dados para o projeto.
    Instale o Docker para empacotar o aplicativo em contêineres.
    Instale o Alembic para gerenciar a migração do banco de dados.

### Estrutura do Projeto utilizando arquitetura baseada em MVC

    app/: Contém o código principal do aplicativo.
        main.py: Arquivo principal que inicia o servidor FastAPI e configura as rotas.
    controllers/: Contém os controladores (controllers) que gerenciam as requisições da API.
        user_controller.py: Controlador responsável pelas operações relacionadas aos usuários (clientes e profissionais).
        appointment_controller.py: Controlador responsável pelas operações relacionadas aos agendamentos.
    services/: Contém a lógica de negócio do aplicativo.
        user_service.py: Serviço que implementa as regras de negócio relacionadas aos usuários.
        appointment_service.py: Serviço que implementa as regras de negócio relacionadas aos agendamentos.
    database/: Contém a configuração do banco de dados utilizando o SQLAlchemy.
        database.py: Configuração do banco de dados e sessão do SQLAlchemy.
        crud.py: Implementa as operações CRUD (Create, Read, Update, Delete) para os modelos.
    migrations/: Contém as configurações do Alembic para gerenciar as migrações do banco de dados.
        alembic.ini: Arquivo de configuração principal do Alembic.
        versions/: Pasta que conterá os scripts de migração gerados pelo Alembic.
    models/: Contém os modelos de dados utilizados no sistema.
        user.py: Modelo para representar os usuários (clientes e profissionais).
        appointment.py: Modelo para representar os agendamentos.
    schemas/: Contém os esquemas de dados utilizados nas requisições e respostas da API.
        user_schemas.py: Esquemas para validar dados relacionados aos usuários.
        appointment_schemas.py: Esquemas para validar dados relacionados aos agendamentos.
    docker/: Contém os arquivos para a criação do contêiner Docker.
        Dockerfile: Arquivo para criar a imagem Docker do aplicativo.
        docker-compose.yml: Define os serviços para a execução do aplicativo e do banco de dados PostgreSQL.
    README.md: Documentação detalhada do projeto, incluindo instruções de instalação, configuração e uso.

### Executando o Projeto

    Clone o repositório do projeto.
    Configure o ambiente de desenvolvimento conforme as instruções no README.
    Execute as migrações do banco de dados utilizando o Alembic.
    Inicie o aplicativo usando o servidor FastAPI.
    Acesse o aplicativo em um navegador ou por meio de ferramentas de API como o Postman.

Considerações Finais

Este projeto é uma aplicação básica de agendamento de barbearia, que pode ser expandida e personalizada conforme necessário. Ele serve como um exemplo de como utilizar as tecnologias mencionadas para construir um sistema funcional para atender às necessidades de uma barbearia.

Lembre-se de incluir detalhes de instalação, configuração e uso no arquivo README.md para que outros desenvolvedores possam entender e utilizar seu projeto facilmente. Boa sorte com o desenvolvimento do sistema de agendamento para a barbearia!
