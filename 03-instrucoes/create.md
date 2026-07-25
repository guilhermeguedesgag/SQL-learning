# Create: Criando sua primeira tabela

Estou criando como exemplo uma tabela de alunos de uma faculdade

## Banco de dados Oracle

```sql
create table alunos (
    id NUMBER GENERATED ALWAYS as IDENTITY primary key,
    cpf char(11) unique not null,
    nome VARCHAR2(50)not null,
    telefone VARCHAR2(50),
    email varchar2(50),
    curso varchar2(50),
    cidade VARCHAR2(50)
    );

```
Criei o cpf como unique pois o aluno nunca deverá ter dois cadastros.

*obs.: Banco de dados Oracle, Banco de Dados SQL seus comandos mudam, por exemplo o serial não possui no Banco de dados Oracle.