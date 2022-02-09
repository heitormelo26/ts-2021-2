**NOME: Heitor Melo  MATRÍCULA:** 201802767 

Conjunto de classes de equivalência para avaliação universitária 



|Id |Descrição |V/I |
| - | - | - |
|CE01|nota1 < 0 |I |
|CE02|nota1 >= 0 e nota1 <= 100 |V |
|CE03|nota1 > 100 |I |
|CE04|nota2 < 0 |I |
|CE05|nota2 >= 0 e nota2 <= 100 |V |
|CE06|nota2 > 100 |I |
|CE07|cargaHoraria < 0 |I |
|CE08|cargaHoraria >= 0 |V |
|CE09|faltas < 0 |I |
|CE10|faltas >= 0 |V |


|CT |Valor de Entrada (nota1,nota2,cargaHoraria,faltas) |Resultado Esperado |Classe de Equivalência|
| - | :- | - | :- |
|CT01 |-2.0;20.0;60;10 |Valor Inválido |CE01 |
|CT02 |70.0;60.0;60;40 |Reprovado por Falta |CE02,CE05, CE08,CE10 |
|CT03 |Reprovado por Média |CE02,CE05, CE08,CE10 |
|||||
|CT05 |50.0;30.0;60;5 |Recuperação |CE02,CE05, CE08,CE10 |
|||||
|CT06 |20.0;-20.0;60;10 |Valor Inválido |CE04 |
|CT07 |70.0;0.0;60;40 |Reprovado por Falta |CE02,CE05, CE08,CE10 |
|CT08 |120.0;0.0;60;40 |Valor Inválido |CE03 |
|CT09 |50.0;130.0;60;40 |Valor Inválido |CE06 |
|CT10 |50.0;30.0;-2;5 |Valor Inválido |CE07 |
|CT11 |50.0;30.0;70;-10 |Valor Inválido |CE09 |
|CT12 |-2.0;-20.0;60;10 |Valor Inválido |CE01,CE04 |
|CT13 |-2.0;20.0;-30;10 |Valor Inválido |CE01,CE07 |
|CT14 |-2.0;20.0;30;-4 |Valor Inválido |CE01,CE09 |
|CT15 |30.0;-20.0;-30;10 |Valor Inválido |CE04,CE07 |
|CT16 |30.0;-20.0;30;-10 |Valor Inválido |CE04,CE09 |
|CT17 |30.0;20.0;-30;-10 |Valor Inválido |CE07,CE09 |
|CT18 |-2.0;-20.0;-60;10 |Valor Inválido |CE01,CE04, CE07 |


|CT19 |-2.0;-20.0;60;-10 |Valor Inválido |CE01,CE04, CE09 |
| - | - | - | :- |
|CT20 |-2.0;20.0;-60;-10 |Valor Inválido |CE01,CE07, CE09 |
|CT21 |20.0;-20.0;-60;-10 |Valor Inválido |CE04,CE07, CE09 |
|CT22 |-20.0;-20.0;-60; -10 |Valor Inválido |CE01,CE04, CE07,CE09 |
|CT23 |120.0;200.0;30;10 |Valor Inválido |CE03,CE06 |
|CT24 |120.0;-200.0;30;10 |Valor Inválido |CE03,CE04 |
|CT25 |120.0;20.0; -3;10 |Valor Inválido |CE03,CE07 |
|CT26 |120.0;20.0; 3;-10 |Valor Inválido |CE03,CE09 |
|CT27 |12.0;200.0;-30;10 |Valor Inválido |CE06,CE07 |
|CT28 |12.0;200.0;30;-10 |Valor Inválido |CE06,CE09 |
|CT29 |12.0;20.0;-30;-10 |Valor Inválido |CE07,CE09 |
|CT30 |120.0;200.0;-30;10 |Valor Inválido |CE03, CE06 ,CE07 |
|CT31 |120.0;200.0;30; -10 |Valor Inválido |CE03, CE06, CE09 |
|CT32 |120.0;20.0;-30;-10 |Valor Inválido |CE03, CE07, CE09 |
|CT33 |12.0;200.0;-30;  -10 |Valor Inválido |CE06, CE07, CE09 |
|CT34 |120.0;200.0;-30;-10 |Valor Inválido |CE03,CE06, CE07, CE09 |
|CT35 |Aprovado |CE02,CE05, CE08,CE10 |
|||||

