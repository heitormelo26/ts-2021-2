<div align=center>
  <img src="brasaooficialcolorido.png">
</div>

#### <p style="text-align: center;">Universidade Federal de Goiás</p>
#### <p style="text-align: center;">Instituto de Informática</p>
#### <p style="text-align: center;">Bacharelado em Engenharia de Software</p>
#### <p style="text-align: center;">Teste de Software - 2021/2</p>
#### <p style="text-align: center;">Gilmar Ferreira Arantes</p>
####  <p style="text-align: center;"> Prova P2 - 12/04/2022</p>

Matrícula: 201802767

Nome: Heitor Melo de Lucas Brandão

<font color="green">Nota 6,95</font>


1. Quanto ao Processo de Teste de Software, responda as duas questões seguintes:
   1.1 (**0,5 ponto**) Defina os seguintes conceitos Processo de Teste de Software, Projeto de Teste de Software e Plano de Teste de Sofware.

    Processo de teste consiste na ação continuada, realização contínua e prolongada de atividades realacionadas e voltadas para a elaboração e execução de testes. Enquanto que o plano de teste consiste no documento elaborado que registra as decisões a serem feitas durante o processo de teste. Por fim, o projeto de Teste de Software consiste na maneira como o processo de teste será executado, isto é, as métricas, boas práticas e práticas usuais a serem adotadas. <font color="red">Nota 0,5</font>

   1.2 (**0,5 ponto**) Descreva o relacionamento existente entre estes conceitos.

   A relação existente entre esses conceitos é que o plano de teste demonstra o que será feito, isto é, é o documento que reflete o que está planejado para os testes mostrando o que deve ser alcançado e isto será feito mediante uma sequencia de processos/atividades definidas no processo de teste sobre as quais métricas e gerenciamento do projeto de teste irão reger conforme esperado. <font color="red">Nota 0,4</font>

2. (**1,0 pontos**) Descreva as vantagens para a equipe de desenvolvimento ao se adotar um processo de teste ágil.

    A vantagem para a equipe de desenvolvimento adotar um processo de teste agil é que esta passará a entender e identificar com mais precisão defeitos durante o próprio desenvolvimento, posto que em teste ágil busca-se evitar defeitos ao invés de apenas procurá-los no final do desenvolvimento. Logo, com a metodologia ágil toda a equipe de desenvolvimento trabalha em conjunto com os testers para agir de modo a desenvolver pensando em evitar erros, o que, consequentemente, evita retrabalho em códigos. Além disso, como busca-se evitar erros, o código elaborado é de maior qualidade, há maior proximidade com stakeholders (pois precisam entender o que seria um defeito a nível de soluçao) e promovem entregas rápidas. <font color="red">Nota 1,0</font>

3. (**1,0 ponto**) Cite pelo menos três características do Teste Exploratório.

    Testes explorátórios são caracterizados por não adotar scripts, tornado a atividade mais flexível e livre, permitindo ao testador explorar a aplicação livremente e diretamente. Além disso, nos testes exploratórios, a documentação de casos de testes e resultados de testes são realizados à medida que os testes são realizados, seguindo uma abordagem de metodologia ágil.Por fim, o teste exploratório pode ser divido em duas diretrizes: Teste exploratório de escopo reduzido (testa funcionalidades/telas especificas) e teste de escopo abrangente (navega pela aplicação toda). <font color="red">Nota 1,0</font>

4. Considere os arquivos .java (Banco.java, Agencia.java, Conta.java e BankValidator.java). Nos próprios arquivos .java estão definidas as regras para cadastramento de cada um deles (Banco, Agencia e Conta). Desta forma, pede-se:
   4.1. (**2.0 Pontos**) Definir os cenários de teste suficientes para testar o cadastro e movimentações financeiras envolvendo bancos, agências e contas, conforme especificado. Para cada cenário definir os critérios de teste adequados à definição dos seus casos de teste.

        Agência

            Número
                CE1 - Numero com 2 dígitos - Erro
                CE2 - Número com 4 dígitos - Certo
                CE3 - Número com 6 dígitos - Erro
                CE4 - Número com letra - Erro

            Nome
                CE5 - Nome com 4 letras - Erro
                CE6 - Nome com 6 letras - Certo
                CE7 - Nome com 101 dígitos - Erro
                CE8 - Nome com número - Erro

            Cidade
                CE9 - Cidade com 4 letras - Erro
                CE10 - Cidade com 6 letras - Certo
                CE11 - Cidade com 101 dígitos - Erro
                CE12 - Cidade com número - Erro

       Banco

            Número
                CE13 - Numero com 2 dígitos inteiros - Erro
                CE14 - Número com 3 dígitos inteiros - Certo
                CE15 - Número com 6 dígitos inteiros - Erro
                CE16 - Número com letra - Erro
                CE16 - Número com 3 dígitos decimais - Erro
                CE17 - Número com 3 dígitos inteiros negativos - Erro

            Nome
                CE18 - Nome com 4 letras - Erro
                CE19 - Nome com 6 letras - Certo
                CE20 - Nome com 101 dígitos - Erro
                CE21 - Nome com número - Erro
        Conta

            Número
                CE22 - Numero com 5 dígitos inteiros - Erro
                CE23 - Número com 6 dígitos inteiros - Certo
                CE24 - Número com 7 dígitos inteiros - Erro
                CE25 - Número com letra - Erro

            Tipo
                CE26 - Corrente - Certo
                CE27 - Poupanca - Certo

            Limite
                CE28 - (Conta) = Corrente - Cheque - Certo
                CE29 - (Conta) = Poupanca - Cheque - Erro

            Saldo
                CE30 - Saldo < 0.0 - Erro
                CE31 - Saldo > 0.0 - Certo

            depositar()
                CE32 - Valor < 0.0 - Erro
                CE33 - Valor > 0.0 - Certo

            transferir()
                CE34 - Valor < 0.0 - Erro
                CE35 - Valor > 0.0 - Certo
                CE36 - ContaOrigem == null - Erro
                CE37 - ContaDestino == null - Erro

             creditarRendimentos()
                CE38 - Valor < 0.0 - Erro
                CE39 - Valor > 0.0 - Certo
                CE40 - Conta.tipo == Poupanca - Certo
                CE41 - Conta.tipo == Corrente - Erro

            debitarJurosChequeEspecial()
                CE38 - Valor < 0.0 - Erro
                CE39 - Valor > 0.0 - Certo
                CE40 - Conta.tipo == Poupanca - Certo
                CE41 - Conta.tipo == Corrente - Erro

            validaTipo()
                CE42 - tipo == Poupanca - Certo
                CE43 - tipo == Corrente - Certo
                CE44 - tipo == Salario - Errado

            validaSaldo()
                CE45 - Valor < 0.0 - Erro
                CE46 - Valor > 0.0 - Certo
    <font color="red">Nota 1,9</font>

   4.2. (**2.0 Pontos**) Definir os casos de teste suficientes para a cobertura do teste de cada um dos cenários definidos. Documentar os casos de teste no seguinte padrão:

           O CEn refere-se ao CTn sendo n >= 1 e n <= 46

         |  CT  | Valores de Entrada | Resultado esperado |
         |:----:|:------------------:|:------------------:|
         | CT01 |         23         |       False        |
         | CT02 |        2146        |        True        |
         | CT03 |       123567       |       False        |
         | CT04 |      1234Aaa       |       False        |
         | CT05 |        nome        |       False        |
         | CT06 |       heitor       |        True        |
         | CT07 |  asdnjod...(100x)  |       False        |
         | CT08 |       hei21        |       False        |
         | CT09 |    asfe            |    False           |
         | CT10 |    asfeaa          |    True            |
         | CT11 | asdnjod...(100x)   |    False                |
         |CT12      | cir6                   |      False              |
         | CT13 |         23         |       False        |
         | CT14 |        214        |        True        |
         | CT15 |       123567       |       False        |
         | CT16 |      1234Aaa       |       False        |
         | CT16 |        33.2        |       False        |
         | CT17 |       -222       |        True        |
         | CT18 |  asdnjod...(100x)  |       False        |
         | CT19 |       hei21        |       False        |
         | CT20 |    asfe            |    False           |
         | CT21 |    asfeaa          |    True            |
         | CT22 |        21422        |        False        |
         | CT23 |       123567       |       True        |
         | CT24 |      1234222       |       False        |
         | CT25 |        22a        |       False        |
         | CT26 |       Corrente       |        True        |
         | CT27 |  Poupanca  |       True        |
         | CT28 |       (Conta) = Corrente - Cheque        |       True        |
         | CT29 |    (Conta) = Poupanca - Cheque            |    False           |
         | CT30 |    -0.2          |    False            |
         | CT31 |     2.2          |    True            |
         | CT32 |    -0.2          |    False            |
         | CT33 |    2.2          |    True            |
         | CT34 |    -0.2          |    False            |
         | CT35 |    2.2          |    True            |
         | CT36 |    null          |    False            |
         | CT37 |    null          |    False            |
         | CT38 |    -0.2          |    False            |
         | CT39 |    2.2          |    True            |
         | CT40 |    Poupanca          |    True            |
         | CT41 |    Corrente          |    False            |
         | CT42 |    Poupanca           |    True            |
         | CT43 |    Corrente          |    True            |
         | CT44 |    Salario          |    False            |
         | CT45 |    -0.2          |    False            |
         | CT46 |    2.2          |    True

    <font color="red">Nota 1,0</font>
    <font color="red">Os valores de entrada não correspondem aos construtores implementados nas classes.</font>

   4.3. (**3.0 Pontos**) Implementar (na linguagem de programação java) as classes para o teste da criação dos objetos e das movimentações financeiras envolvendo bancos e agências e contas.

   <font color="red">Nota 1,15</font>


INSTRUÇÕES:
1. Tipo: Prova individual;
2. Local de Entrega: Plataforma Turing.
3. Forma de Entrega: arquivo compactado contendo:
   1. Este arquivo md, respondido.
   2. Classes de teste para (BancoTest, AgenciaTest e ContaTest);
   3. O arquivo compactado deverá ter o seguinte nome prova_p2<mat>.zip, onde mat é o número da matrícula do aluno(a).
5. Data da Entrega: 12/04/2022, as 22hs.
6. Critério de Aceitação: arquivo entregue, conforme solicitado.
7. Obs: segue no mesmo pacote o arquivo "org.apache.commons.lang.StringUtils", que é uma dependência do projeto. É deve ser inserida no _classpath_ do projeto de implementação da questão 4, caso não esteja utilizando o _maven_.
