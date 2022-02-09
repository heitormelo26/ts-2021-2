

# GRAFICO DE CAUSA E EFEITO:

![](https://i.imgur.com/oIqIpZe.png)

# TABELA DE DECISAO

| CAUSA OU EFEITO | CONDIÇÕES/REGRAS | R1     | R2  | R3  | R4  | R5  | R6  | R7  | R8  |
| --------------- | ---------------- | ------ | --- | --- | --- | --- | --- | --- | --- |
| CAUSA           | Masculino        |    V   | V   |   V |  V  |   F |  F  |   F |  F  |
| CAUSA           | Idade > 25       |    F   | F   |   V |   V |   F |  F  |   V |  V  |
| CAUSA           | Casado(a)        |    F   | V   |   F |  V  |   F |  V  |   F |   V |
| XXXXXX          | XXXXXX           | XXXXXX |     |     |     |     |     |     |     |
| EFEITO          | 0% de desconto   |   X    |     |     |     |     |     |     |     |
| EFEITO          | 5% de desconto   |        |   X |     |     |  X  |     |     |     |
| EFEITO          | 10% de desconto  |        |     |  X  |     |     |  X  |     |     |
| EFEITO          | 15% de desconto  |        |     |     |  X  |     |     |  X  |     |
| EFEITO          | 20% de desconto  |        |     |     |     |     |     |     |  X  |

# CASOS DE TESTE

| CASO DE TESTE   | MASCULINO| IDADE > 25 | CASADO(A) | VALOR     |
| --------------- | ---------| ---------- | --------- | --------- |
| Caso de Teste 1 | TRUE     | FALSE      | FALSE     | R$2000,00 |
| Caso de Teste 2 | TRUE     | FALSE      | TRUE      | R$1900,00 |
| Caso de Teste 3 | TRUE     | TRUE       | FALSE     | R$1800,00 |
| Caso de Teste 4 | TRUE     | TRUE       | TRUE      | R$1700,00 |
| Caso de Teste 5 | FALSE    | FALSE      | FALSE     | R$1900,00 |
| Caso de Teste 6 | FALSE    | FALSE      | TRUE      | R$1800,00 |
| Caso de Teste 7 | FALSE    | TRUE       | FALSE     | R$1700,00 |
| Caso de Teste 8 | FALSE    | TRUE       | TRUE      | R$1600,00 |






					


---
