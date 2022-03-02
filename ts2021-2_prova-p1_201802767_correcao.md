<div align=center>

  ![](https://i.imgur.com/Jl4jpwI.png)

</div>

#### <p style="text-align: center;">Universidade Federal de Goiás</p>
#### <p style="text-align: center;">Instituto de Informática</p>
#### <p style="text-align: center;">Bacharelado em Engenharia de Software</p>
#### <p style="text-align: center;">Teste de Software - 2021/2</p>
#### <p style="text-align: center;">Gilmar Ferreira Arantes</p>
####  <p style="text-align: center;"> Prova P1 - 16/02/2022</p>

**Matrícula**: Heitor Melo de Lucas Brandão
**Nome**: 201802767

<p><font color=green>Nota: 9.0</font></p>

1. Quanto ao objetivo do Teste de Software, responda as duas questões seguintes:
   1. (**0,5 ponto**) Qual o objetivo primário da atividade de teste de software?

   O objetivo primário da atividade de teste de software é revelar a presença de defeitos. <font color=green>Certo.</font>

   2. (**0,5 ponto**) O que acontece, quando não se atinge este objetivo primário?

    Quando a atividade de teste de software não atinge este objetivo primário, o software estará sujeito a apresentar defeitos e consequentemente a produção de erros os quais vão levar a falha do software. <font color=red>Errado.</font>

2. (**1,0 ponto**) Explique o que é o teste exaustivo e porque sua execução não é possível.

    Teste exaustivo consiste na busca de eliminar e satisfazer todas as possibilidade de teste para determinado software ou parte deste, isto é, trazer todo o conjunto infinito de valores para cada chamada, execução, rotina do software a ser testado. Então, por exemplo, em situação de teste de cadastro onde há uma senha, para se testar todas as combinações de senha possíveis beira-se ao impossível devido a um conjunto praticamente infinito de combinação de caracteres. Portanto, é inviável se realizar um teste exaustivo, pois necessita-se de muitos recursos (como o tempo), apresentando pouca vantagem em relação a outros tipos de testes. <font color=green>Certo.</font>

3. (**1,0 ponto**) Cite pelo menos duas limitações da Técnica de Teste Funcional e duas da Técnica de Teste Estrutural.

    O teste funcional apesar de ser extremamente necessário apresenta limitações como o fato de ser altamente dependente de uma boa documentação na especificação de requisitos, ja que seu teste é diretamente oriundo deste documento, além disso, o teste funcional não garante que todas as partes essenciais do software seram testadas, requerendo para isso a utilização de teste exaustivo, o qual não é vantajoso para a ativida de teste em geral. Enquanto isso, o teste estrutural mesmo sendo essencial para a atividade de teste, se limita no fato de que o número de caminhos em uma execução de código pode ser infinito ou muito grande e mesmo que todos os caminhos estejam especificados pode-se haver problemas no fluxo de execução visto como correto, alem disso, nesse teste determinado módulo pode ser executado corretamente para alguns teste e para outros não. <font color=green>Certo.</font>

4. (**1,0 ponto**) Descreva pelo menos um dos quatro níveis de teste constantes da literatura especializada.

    Um dos níveis de teste constantes consiste no Teste de Sistema o qual consiste em um teste puramente de usuário, isto é, testar o software atuando como um usuário, buscando assim, se contextualizar no ambiente operacional do usuário, ou seja, executar o teste no mesmo ambiente, com mesmos dados e mesma visão sobre o software que um usuário teria. <font color=green>Certo.</font>

5. (**1.0 ponto**)Descreva qual o propósito do critério de teste funcional Particionamento por Classes de Equivlência.

    O proprósito do teste funcional de Particionamento por Classes de Equivalência é minimizar o número de casos testes mediante a separação do conjunto de entradas possíveis em classes que mostram equivalencia entre todos os valores que estão contidos nela. Dessa maneira, para testar determinada funcionalidade que poderia requerer teste exaustivo (testar todas as possibilidades), executa-se o teste por classe de equivalencia que separa tao conjunto de entradas em N classes sobre as quais é necessário testar um valor que pertence a esta, visto que teoricamente um elemento de uma classe de equivalencia se comporta da mesma maneira que os outros da mesma classe. <font color=green>Certo.</font>

6. (**1.00 ponto**) Existe algum tipo de hierarquia em relação aos critérios de teste estrutural, todos os nós, todos os arcos e todos os caminhos? Se sim, explique-a, considerando a perspectiva dos níveis de cobertura desejados.

    Sim, existe um tipo de hierarquia em relação aos critérios de teste estrutural (todos nós, todos arcos e todos caminhos), visto que nos 8 níveis de cobertura definidos por Copeland (2004), o nível 1 oferece cobertura sobre todos os nós (para situações excepcionais como falta de memória), enquanto que o nível 2 apresenta cobertura para todos os arcos (para situação de analisar as tomadas de decisões de TRUE e FALSE) e por fim, o nível 7 o qual  estende para todos os caminhos de execução de um procedimento. <font color=green>Certo.</font>

7. Considere a especificação, a seguir, de um hipotético programa que objtiva a classificação de um triângulo, a partir dos valores informados para os seus três lados.

   a) Dado um triângulo cujos segmentos medem A, B e C, que são números inteiros positivos na faixa de 0 a 100. Esse triângulo somente existirá se: (A + B < C) ou (A + C < B) ou (B + C < A).
   b) Quanto às medidas dos seus lados o triângulo, poderá ser classicado em:
         • Isósceles = quando possui dois lados com a mesma medida;
         • Escaleno = quando todos os seus lados têm medidas diferentes;
         • Equilátero = quando todos os lados tem a mesma medida;
         • Acutângulo = quando o quadrado de um dos seus lados é menor que a soma do quadrado dois outros dois. (A<sup>2</sup> < B<sup>2</sup> + C<sup>2</sup>).
         • Retângulo: quando o quadrado de um dos seus lados é igual à soma do quadrado dois outros dois. (A<sup>2</sup> = B<sup>2</sup> + C<sup>2</sup>).
         • Obtusângulo: quando o quadrado de um dos seus lados é maior que a soma do quadrado dois outros dois. A<sup>2</sup> > B<sup>2</sup> + C<sup>2</sup>.

7.1 (**2.0 pontos**) Definir uma tabela de decisão para o teste tanto da existência do triângulo, quanto para a definição do seu tipo. Consulte exemplo de tabela de decisão na tarefa 005.

    Considerando que a causa: "<a,b,c> é triangulo?" consiste no conjunto de regras (A + B > C) ou (A + C > B) ou (B + C > A)

| CAUSAS               | Regra - 1  | Regra - 2  | Regra - 3  | Regra - 4  | Regra -5  | Regra - 6  | Regra -7  | Regra - 8  | Regra - 9  |
| -------------------- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| <a,b,c> é triangulo? | F   | T   | T   | T   | T   | T   | T   | T   | T   |
| a = b                | -   | F   | F   | F   | F   | T   | T   | T   | T   |
| b = c                | -   | F   | F   | T    | T    | F   | F   | T    |T     |
| a = c                | -   | F   | T    | F   | T    | F   | T    |F     | T    |
| **Efeitos**          |     |     |     |     |     |     |     |     |     |
| Não existe           | X   |     |     |     |     |     |     |     |     |
| Isósceles            |     |     |  X   | X    |     | X    |     |     |     |
| Escaleno             |     | X    |     |     |     |     |     |     |     |
| Equilátero           |     |     |     |     |     |     |     |     |  X   |
| Impossível           |     |     |     |     | X    |     |  X   |  X   |     |

<font color=green>Certo.</font>

7.2 (**2.0 pontos**) Criar os conjunto de casos de teste necessários para a cobertura das combinações constantes da tabela de decisão, seguindo o seguinte padrão:

| CT1 | Lado A | Lado B | Lado C | Resultado |
| --- | ------ | ------ | ------ | --------- |
| CT1 | 2       |  3      | 4       | Não existe          |
| CT2 | 5      | 5      | 6      | Isósceles |
| CT3 | 9      | 7       | 14       | Escaleno          |
| CT4 | 2       | 2       | 2       |  Equilátero         |

<font color=orange>Parcialmente correto. O CT01 Falhou. Nota 1,5.</font>

# OBSERVAÇÃO:

    A regra mencionada anteriormente para existencia de um triangulo "(A + B < C) ou (A + C < B) ou (B + C < A)", está  equivocada, o correto é: (A + B > C) ou (A + C > B) ou (B + C > A)
