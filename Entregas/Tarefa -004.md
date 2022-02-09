**NOME: Heitor Melo  MATRÍCULA:** 201802767 

Conjunto de classes de equivalência para avaliação universitária 



|Id |Descrição |V/I |
| - | - | - |
|CE01 |nota1 < 0 |I |
|CE02 |nota1 >= 0 e nota1 <= 100 |V |
|CE03 |nota1 > 100 |I |
|CE04 |nota2 < 0 |I |
|CE05 |nota2 >= 0 e nota2 <= 100 |V |
|CE06 |nota2 > 100 |I |
|CE07 |cargaHoraria < 0 |I |
|CE08 |cargaHoraria >= 0 |V |
|CE09 |faltas < 0 |I |
|CE10 |faltas >= 0 |V |


|CT |Valor de Entrada (nota1,nota2,cargaHoraria,faltas) |Resultado Esperado |Classe de Equivalência|
| - | :- | - | :- |
|CT01 |-0.1,20,20,20 |Valor Inválido |CE01, CE05, CE08, CE10 |
|CT02 |0,20,20,20 |Reprovado por Falta |CE02, CE05, CE08, CE10 |
|CT03 |0.1,20,20,20 |Reprovado por Falta |CE02, CE05, CE08, CE10 |
|CT05 |99.9,20,20,20 |Reprovado por Falta |CE02, CE05, CE08, CE10 |
|CT06 |100,20,20,20 |Reprovado por Falta |CE02, CE05, CE08, CE10 |
|CT07 |100.1,20,20,20 |Valor Inválido |CE03, CE05, CE08, CE10 |
|CT08 |20, -0.1,20,20 |Valor Inválido |CE04, CE02, CE08, CE10 |
|CT09 |20,0,20,20 |Reprovado por Falta |CE05, CE02, CE08, CE10 |
|CT10 |20,0.1,20,20 |Reprovado por Falta |CE05, CE02, CE08, CE10 |
|CT11 |20,99.9,20,20 |Reprovado por Falta |CE05, CE02, CE08, CE10 |
|CT12 |20,100,20,20 |Reprovado por Falta |CE05, CE02, CE08, CE10 |


|CT13 |20,100.1,20,20 |Valor Inválido |CE06, CE02, CE08, CE10 |
| - | - | - | - |
|CT14 |20,20,-1,20 |Valor Inválido |CE02,CE05, CEO7,CE10 |
|CT15 |20,20,0,20 |Reprovado por Falta |CE02,CE05, CEO8,CE10 |
|CT16 |20,20,1,20 |Reprovado por Falta |CE02,CE05, CEO8,CE10 |
|CT17 |20,20,20,-1 |Valor Inválido |CE02,CE05, CEO8,CE09 |
|CT18 |20,20,20,0 |Reprovado por Média |CE02,CE05, CEO8,CE10 |
|CT19 |20,20,20,1 |Reprovado por Média |CE02,CE05, CEO8,CE10 |
|CT20 |-0.1,-0.1,20,20 |Valor Inválido |CE01, CE04, CE08, CE10 |
|CT21 |0.1,-0.1,20,20 |Valor Inválido |CE02, CE04, CE08, CE10 |
|CT22 |99.9,-0.1,20,20 |Valor Inválido |CE02, CE04, CE08, CE10 |
|CT23 |100,-0.1,20,20 |Valor Inválido |CE02, CE04, CE08, CE10 |
|CT24 |100.1,-0.1,20,20 |Valor Inválido |CE03, CE04, CE08, CE10 |
|CT25 |-0.1,0,20,20 |Valor Inválido |CE01, CE05, CE08, CE10 |
|CT26 |0.1,0,20,20 |Reprovado por Falta |CE02, CE05, CE08, CE10 |
|CT27 |99.9,0,20,20 |Reprovado por Falta |CE02, CE05, CE08, CE10 |
|CT28 |100,0,20,20 |Reprovado por Falta |CE02, CE05, CE08, CE10 |
|CT29 |100.1,0,20,20 |Valor Inválido |CE03, CE05, CE08, CE10 |
|CT30 |30,30,20,0 |Recuperação |CE02, CE05, CE08, CE10 |
|CT31 |20,20,-1 ,-1 |Valor Inválido |CE02,CE05, CEO7,CE09 |
|CT32 |20,20,0 ,-1 |Valor Inválido |CE02,CE05, CEO7,CE09 |
|CT33 |20,20,1 ,-1 |Valor Inválido |CE02,CE05, CEO8,CE09 |
|CT34 |20,20,-1 ,0 |Valor Inválido |CE02,CE05, CEO7,CE10 |
|CT35 |20,20,0 ,0 |Reprovado por Falta |CE02,CE05, CEO8,CE10 |


|CT36 |20,20,1 ,0 |Reprovado por Falta |CE02,CE05, CEO8,CE10 |
| - | - | - | - |
|CT34 |20,20,-1 ,1 |Valor Inválido |CE02,CE05, CEO7,CE10 |
|CT35 |20,20,0 ,1 |Reprovado por Falta |CE02,CE05, CEO8,CE10 |
|CT36 |20,20,1 ,1 |Valor Inválido |CE02,CE05, CEO8,CE10 |

