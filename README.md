# Configurações do Projeto

## Conectando ao PostgreSQL Usando Docker

Para se conectar ao banco de dados PostgreSQL, siga estas etapas:

1. Inicie o contêiner do PostgreSQL executando o seguinte comando no terminal:

   ```bash
   docker compose up -d
   ```

2. Execute o seguinte comando para se conectar ao banco de dados:

   ```bash
   docker run -it --name sales-postgres-client --network sales_network --rm postgres:latest psql -h sales_postgres -U rviana -d sales_db
   ```
