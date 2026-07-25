## Insert: Como fazer o insert?

Após nossa tabela estar criada, vamos realizar as inserções:

```sql
insert into alunos (cpf, nome, telefone, email, curso, cidade) values ('12345678901', 'joao', '14998123456', 'joao.silva@gmail.com','Engenharia', 'Bauru');


```

## Como inserir uma coluna em uma tabela existente?

Use o comando alter table adicionar uma tabela já existente, por exemplo se você esqueceu de adicionar uma coluna de salario:


```sql
alter table alunos add salario number(10,2) default 3500;

```

No comando acima, ele irá alternar a tabela e inserir por padrão a informação 3500