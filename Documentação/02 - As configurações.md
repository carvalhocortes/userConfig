# As configurações

Serão permitido alterações nas seguintes configurações:

## Taxas
advanceDelay = contem o plano de recebimento dividido entre credito e debito. O valor informado corresponde  a quantidade de dias.
advanceTax = contem o valor da taxa a ser cobrada do cliente tanto para credito quanto para debito. 
Para o credito deve ser informada o valor para compras divididas em até 12 vezes. sendo permitido quebrar em intervalos menores.
from = quantidade inicial de meses. 
to = quantidade final de meses.
value = valor da taxa
Para o campo debito informar somente o valor da taxa.

Abaixo exemplo com plano de recebimento D+1 para credito e debito e taxa de credito de 1,99% para compras em 1 vez no credito, 7,5% de 2 à 6 vezes e 13,5% de 7 à 12 vezes no credito. Para compras no debito taxa de 1,19%

```JSON
"config": {
  "advanceDelay": {
    "credit": 1,
    "debit": 1
  },
  "advanceTax": {
    "CREDIT": [
      {"from": 1,"to": 1,"value": 0.0199},
      {"from": 2,"to": 6,"value": 0.075},
      {"from": 7,"to": 12,"value": 0.135}
    ],
    "DEBIT": 0.0119
  }
}
```


## Limites

sdf

```JSON
"config": {

}
```



## Notificações

asfd

```JSON
"config": {

}
```


## Grupos padrão

Os grupos padrão devem ter todas as configurações citadas.