# Visão geral da API

A API contem um conjunto de rotas que permitirá segregar clientes em diferentes grupos de taxas. Dessa forma, é possível criar grupos novos  e / ou grupos de preços específicos com taxas exclusivas (com datas validade ou não).

Todos os usuários tem um grupo associado a ele no processo de criação e durante o seu ciclo de vida, pode ser associado a novos grupos de taxas ( que tem validade ou padrão que não possuem).
As configurações de grupos  associadas a um usuário só são validas se o grupo está dentro dentro de sua validade e não foi deletado. 

Todas as alterações serão feitas somente de forma lógica. Desta forma será possível a realizações de auditorias e controle de alterações pelo broker.

As configurações são separadas pro broker.


