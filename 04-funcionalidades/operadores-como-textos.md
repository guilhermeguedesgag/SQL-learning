## ' : Como inserir apóstrofos ou outros caracteres especiais como textos


Se você quiser inserir a palavras 'Departament's' você terá que inserir uma tratativa para que seja inserido essa palavra com o apostrofo:

```sql
select nome || q'[ estudo no caic's ]' || cidade as informacao from alunos;
```

![](image-2.png)

Ficando dessa forma acima.