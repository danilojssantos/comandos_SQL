# comandos_SQL



## CREATE TABLE 

A CREATE TABLE instrução é usada para criar uma nova tabela em um banco de dados.

```bash
    CREATE TABLE users(
	id INTEGER PRIMARY KEY AUTOINCREMENT,
	name VARCHAR,
	email VARCHAR,
	password VARCHAR,
	avatar VARCHAR NULL,
	create_at DATETIME NOT NULL DEFAULT CURRENT_TIMESTAMP, 
	update_at DATETIME NOT NULL DEFAULT CURRENT_TIMESTAMP 
)
```
## ALTER TABLE

Para renomear uma tabela, use a seguinte exemplo:

```bash
ALTER TABLE clientes RENAME TO users
```
## ALTER TABLE ADD

Adiciona uma coluna, use a seguinte exemplo:

```bash
ALTER TABLE users ADD status VARCHAR
```

## ALTER TABLE RENAME COLUMN

Para renomear uma coluna em uma tabela, use a seguinte exemplo:

```bash
ALTER TABLE users RENAME COLUMN status TO active
```
## ALTER TABLE DROP COLUMN

Para excluir uma coluna de uma tabela, use a seguinte exemplo: 

```bash
ALTER TABLE users RENAME COLUMN status TO active
```


# SQL - Comandos DML (Data Manipulation Language)

C - Create -> `INSERT` 

R - Read   -> `SELECT`

U - Update -> `UPADATE`

D - Delete -> `DELETE`


## INSERT INTO 

A INSERT INTO instrução é usada para inserir novos registros em uma tabela.

```bash
INSERT INTO users(name, email, password)
VALUES
('Danilo','danilojssantos1@gmail.com','123')
```
## SELECT 
SELECT * FROM instrução é usada para selecionar dados de um banco de dados, retornar todas as colunas

```bash
SELECT * FROM users
```
instrução é usada para selecionar dados de um banco de dado por exemplo id nome email

```bash
SELECT id, name, email  FROM  users;
```

## UPDATE 
UPDATE instrução é usada para modificar os registros existentes em uma tabela.

```bash
UPDATE users SET avatar = 'danilo.png'
WHERE id = 1
```

