# Desafio Clean Architecture

## Descrição

Para este desafio, você precisará criar o usecase de listagem das orders.
Esta listagem precisa ser feita com:

- Endpoint REST (GET /order)
- Service ListOrders com GRPC
- Query ListOrders GraphQL
  Não esqueça de criar as migrações necessárias e o arquivo api.http com a request para criar e listar as orders.

Para a criação do banco de dados, utilize o Docker (Dockerfile / docker-compose.yaml), com isso ao rodar o comando docker compose up tudo deverá subir, preparando o banco de dados.
Inclua um README.md com os passos a serem executados no desafio e a porta em que a aplicação deverá responder em cada serviço.

## Pré-requisitos:

- Docker instalado na máquina local
- GO Intalado

## Comando Necessários para Executar o Sistema:

1. Subir o Docker:

```bash
docker compose up -d

```

2. Realizar a Migrations:

```
make migrate
```

## Portas Disponíveis para cada Sistema:

- web server on port :8000
- gRPC server on port 50051
- GraphQL server on port 8080

## Modo de acesso de Sistema:

- web server utilizar as Requisições dentro da pasta Api
- gRPC server utilizar o Evans para as requisições
- GraphQL server utilizar o próprio Playground do graphql.
