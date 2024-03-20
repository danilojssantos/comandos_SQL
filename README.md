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
	create_at TIMESTAMP CURRENT_TIMESTAMP,
	update_at TIMESTAMP CURRENT_TIMESTAMP
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

