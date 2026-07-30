## Alter: Alterando dados de uma tabela

## Como inserir uma coluna em uma tabela existente?

Use o comando alter table adicionar uma tabela já existente, por exemplo se você esqueceu de adicionar uma coluna de salario:


```sql
alter table alunos add salario number(10,2) default 3500;

```

No comando acima, ele irá alternar a tabela e inserir por padrão a informação 3500