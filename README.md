# SQL-learning
Learning about SQL
<br><br>

> <h2>Comandos para criar uma tabela </h2>  

```sql 
  CREATE TABLE aluno_curso (
    id SERIAL PRIMARY KEY,
    nome VARCHAR(255) not null
  ); 
```
No exemplo acima foi inserido uma chave primária, como se fosse um cpf do campo.
***  
<br><br>

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
<br><br>

***
> <h2>What is the UNIQUE ?  </h2>
>
> The UNIQUE is use then you can't repeat the value for the
> fields, for example the cpf, never person it going have iguals cpf.
> ```sql
> CREATE TABLE curso (
> id INTEGER NOT NULL UNIQUE,
> nome varchar(255) NOT NULL 
> );
>```


***
> <h2> Can I repeat PRIMARY KEY? </h2>
>
> No, you can't repeat PRIMARY KEY. because, these is a similar
> to the UNIQUE.
> PRIMARY KEY is how if was UNIQUE, but , the main key.
> 
***
<br><br>
> <h2> Creating keys foreign - criando chaves estrangeiras </h2>
>
> For example:
> ```sql
> CREATE TABLE aluno (
>       id SERIAL PRIMARY KEY,
>       nome VARCHAR(255) NOT NULL
> ) ;
> ```
> Now, we will insert two values:
> ``` sql
> INSERT INTO aluno (nome) VALUES ('Diogo');
> INSERT INTO aluno (nome) VALUES ('Vinicius');
> 
>```
> After this, we will go create the relations between the tables:
> 
> ```sql
> CREATE TABLE aluno_curso (
>       aluno_id INTEGER,
>       curso_id INTEGER,
>       PRIMARY KEY (aluno_curso, curso_id)
> 
>       FIREIGN KEY (aluno_id)
>       REFERENCES aluno(id),
> 
>       FOREIGN KEY (curso_id)
>       REFERENCES curso (id)        
>  
> )
> ```
> In the example above
> 





