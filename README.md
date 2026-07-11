# SQL-learning
Learning about SQL

> <h2>Comandos para criar uma tabela </h2>  

```sql 
  CREATE TABLE aluno_curso (
    id SERIAL PRIMARY KEY,
    nome VARCHAR(255) not null
  ); 
```
No exemplo acima foi inserido uma chave primária, como se fosse um cpf do campo.

> <h2>Why definy fields not null?</h2> 
If you not definy fields not null, him accepty value is blank, for example:

A number for CPF can't be null(blank), these can be 
empty, because the person can't know, otherwise, must be completed.

Below a example this:

```sql
CREATE TABLE curso (
  id INTEGER NOT NULL,
  nome varchar(255)
)
```



