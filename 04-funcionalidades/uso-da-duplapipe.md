# PIPE '||'  Quando usar?

A dupla pipe é usada para unir textos, por exemplo em nossa tabela, poderíamos unir:

```sql
select nome || 'mora em' || cidade as informacao from alunos;
```

>Lembrando que este valor tem que estar em aspas simples.

Ficando assim:

![alt text](image-2.png)

A pipe dupla junta colunas de uma tabela, adiciona palavras que você quiser, e retorna tudo junto em uma coluna nova.

Em nosso exemplo, ela retornou tudo na coluna 'informação'.