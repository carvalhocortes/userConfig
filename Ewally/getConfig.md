# getConfig

Lambda responsável pela busca e montagem das configurações de usuário

**Notas técnicas**  
1- Para montar a config do usuário, devemos buscar todos os grupos cujo configHolder é igual ao username do usuário

**Regras**  
1- configs individuais tem prioridade sobre todas outras configs  
2- config filho tem prioridade sobre a config pai  
3- config de grupo client tem prioridade sobre config de grupo sistêmico  
4- Se duas configs de grupo client der conflito vale o ultimo vinculado  
5- Para uma config de grupo client ser valida, o grupo deve ter uma data de vigência valida e o relacionamento entre o usuário e o grupo também e se não está deletado