# Projeto_Docker

**Data Criação:** 14/07/2025 <br>
**Autor:** Leonardo <br>
**Objetivo:** Esse projeto tem como objetivo aprender e aperfeiçoar a ferramenta Docker fazendo o docker compose do banco de dados postgres e linkando ele ao pgadmin além de subir o banco northwind automaticamente

### Primeiros passos:

Para utilização desse repositório faça os comandos abaixo:


**Clone o repositório**
```
git clone https://github.com/LeonArmster/Projeto_Docker.git
```

**Criar arquivos**

Na pasta var, crie os arquivos com as senhas para acessar o postgres e o pgadmin como no exemplo:

Nome do arquivo: postgres.env
```
POSTGRES_DB=database_name
POSTGRES_USER=user
POSTGRES_PASSWORD=password
```

Nome do arquivo: pgadmin.env
```
PGADMIN_DEFAULT_EMAIL=username@email.com
PGADMIN_DEFAULT_PASSWORD=password
```


**Suba o compose**

Use o comando abaixo para subir o compose:
```
docker compose up -d
```
<br>

### Acessando o banco de dados

Após a criação do compose, para acessar o banco de dados basta utilizar a instrução abaixo para ser direcionado à página do pgadmin:
```
localhost:5050
```
Após essa instrução aparecerá a página abaixo onde colocaremos o usuário e a senha definidos no pgadmin.env:
![Página PG Admin](image/pgadmin.png)

Clicar com o botão direito em cima do server e clicar em Register para configurarmos o servidor. Por padrão é colocado postgres
![Configurando o servidor](image/server-pgadmin.png)

Após isso, clicar na aba Connection e inserir no hostname o nome postgres, no username e no password os mesmos que foram definidos no postgres.env como no exemplo abaixo:
![Configurando as conexões do server](image/conexao-pgadmin.png)

Após clicar em salvar nossas conexões estarão funcionais e o nosso servidor carregado e pronto pra uso
![Server funcional](image/server-funcional.png)

