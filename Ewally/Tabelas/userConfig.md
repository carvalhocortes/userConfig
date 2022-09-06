# A tabela userConfig



configHolder = Portador da configuração. Pode ser um grupo ou um usuário
uuid = id único da configuração
parent = id da relação entre grupo e grupo e usuário grupo
config = configurações relativas ao grupo
type = tipo de configuração
deletedAt = data que o grupo foi deletado logicamente
start = inicio da data de vigencia
end = fim da data de vigencia
createdAt = data de criação da configuração


configHolder | uuid | parent | config | type | deletedAt | start | end | createdAt
--- | --- | --- | --- | --- | --- | --- | --- | ---
string | uuid | string | object | string | timestamp | timestamp | timestamp | timestamp
Default | 1 | | {} | system
Norte | 2 | 1 | {} | CSF 
Sul | 3 | 1 | {} | CSF 
Leste | 4 | 1 | {} | CSF 
Oeste | 5 | 1 | {} | CSF
Maquininha free | 6 | | {} | CSF 
csf_joao | 7 | 2 | {} | relationship | | | 2022-07-01 23:59 | 2022-01-30 11:18
csf_joao | 8 | 6 | {} | relationship 
Festa Junina | 9 | | {} | CSF | | 2022-06-01 00:00 | 22-07-31 23:59
csf_joao | 10 | 3 | {} | relationship | | 2022-07-02 00:00 | | 2022-06-30 12:49
csf_joao | 11 | 9 | {} | relationship


