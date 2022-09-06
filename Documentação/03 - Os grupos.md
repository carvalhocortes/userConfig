# Os grupos

## Descrição

Dentro do contexto configurações de usuário um GRUPO é um conjunto de configurações que será associado a um USUÁRIO.

A API permite a criação, edição, consulta e exclusão (lógica) de grupos, além de guardar informações históricas sobre cada ação para fins de auditoria.

## Regras

Não é permitido criar grupos com o mesmo nome de um grupo existente e valido.

Os grupos podem, mas não precisam, ter datas início e fim de validade.

## Tipos de Grupos

Existem três tipos de grupos, o **padrão**, **complementar**, **promocional**.

O **grupo padrão** são aqueles que são associados a um usuário quando ele é criado. Não podem ter validade.

**Grupo complementar** adiciona configurações especificas para um usuário. Podem ou não ter validade.

**Grupo promocional adiciona** configurações especificas para um usuário por determinado tempo. Devem ter validade.

## Erros

Em caso de duplicidade ou inconsistência de algum dado enviado a API retorna erro conforme tabela.

Campo | Descrição | Formato
--------- | --------- | --------- 
groupName | Nome do grupo | string 
config | configurações do grupo | objeto 
start | data de início da validade do grupo | YYYY-MM-DD HH:MM
end | data de fim da validade do grupo | YYYY-MM-DD HH:MM


