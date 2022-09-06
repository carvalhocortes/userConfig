# Os usuários

## Descrição

Dentro do contexto configurações de usuário um USUÁRIO é um conjunto de um ou mais GRUPOS que se sobrepõe formando a configuração total válida de um cliente do broker.

A API permite a associação, troca ou desassociação de um grupo a um usuário, além de guardar informações históricas sobre cada ação para fins de auditoria.

## Regras

Todos os usuários devem estar associados a um grupo padrão.

Não é permitido associar duas vezes o mesmo grupo a um usuário.

As associações podem, mas não precisam, ter uma data de validade.

É possível definir dia e hora que a associação começa ou deixa de valer.

É possível trocar o grupo associado por outro grupo do mesmo tipo.

A troca de grupo associado pode ser agendada para um dia e hora específico ou feita imediatamente.

Não é possível desassociar um grupo que seja do tipo padrão.

## Erros

Em caso de duplicidade ou inconsistência de algum dado enviado a API retorna erro conforme tabela.

Campo | Descrição | Formato
--------- | --------- | --------- 
userName | Nome do usuáro | broker_cliente
groupName | Nome do grupo a ser associado | string
config | configurações do grupo | objeto 
start | data de início da validade do grupo | YYYY-MM-DD HH:MM
end | data de fim da validade do grupo | YYYY-MM-DD HH:MM


