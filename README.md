Instruções para rodar o PostgreSQL no Docker

1. Instalar o Docker
   Se você ainda não tem o Docker instalado, siga as instruções oficiais para instalar o Docker.

2. Baixar a imagem do PostgreSQL
   Abra o terminal e execute o seguinte comando para baixar a imagem oficial do PostgreSQL:

bash
Copiar
Editar
docker pull postgres 3. Subir o container do PostgreSQL
Agora, vamos rodar o container com o PostgreSQL. Use o comando abaixo, onde:

-e POSTGRES_PASSWORD=senha define a senha do usuário postgres.

-p 5432:5432 mapeia a porta do PostgreSQL para a máquina local.

--name postgres-container dá o nome ao seu container.

bash
Copiar
Editar
docker run --name postgres-container -e POSTGRES_PASSWORD=senha -p 5432:5432 -d postgres
Nota: Substitua senha pela senha desejada para o usuário postgres.
