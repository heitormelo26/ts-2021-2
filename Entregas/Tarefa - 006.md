## Tarefa 006 - 15/02/2022 - Grafo de Fluxo de Controle

1. Heitor Melo De Lucas Brandão || 201802767

~~~java

public class Avaliacao {


1    public String avalia(double nota1, double nota2, int faltas, int cargaHoraria) throws ValoresInvalidosException{
2        String result;
3        double percentualFaltas = (faltas*100/cargaHoraria);
4        double media = (nota1 + nota2)/2;
5        if((nota1 < 0.0 || nota1 > 10) || (nota2 < 0.0 || nota2 > 10) || (faltas < 0 || faltas > cargaHoraria) || cargaHoraria < 0){
6            throw new ValoresInvalidosException();//result = "Valores Inválidos.";
7        }else if(percentualFaltas > 25.0){
8            result = "Reprovado por Falta.";
9        }else if(media < 3.0){
10            result = "Reprovado por Média.";
11        }else if(media >= 3.0 && media < 6.0){
12            result = "Prova Extra.";
13        }else{
14            result = "Aprovado.";
15        }
16        return result;
17    }
18 }
~~~

2. **Pede-se:**
   1. Desenhar o **Grafo do Fluxo de Controle**. Pode-se anexar a imagem, aqui neste arquivo.

    Arquivo gerado pelo aluno:
    
    ![](https://i.imgur.com/a4sjFHX.png)


    
    Arquivo gerado pelo plug-in do eclipse:

    ![](https://i.imgur.com/prLmPL8.png)



  
   **2. Calcular a complexidade ciclomática do código. Exemplo de coo calcular pode ser obtido no [link](https://www.treinaweb.com.br/blog/complexidade-ciclomatica-analise-estatica-e-refatoracao)**

    Utilizando a fórmula:  V(G) = 16 – 13 + 2, em que onde E é o número de arestas (setas) e N é o número de nós do grafo G.
    
    Temos que para o grafo acima V(G) = 5 
    
    Considerando a tabela abaixo, temos que o código é de complexidade **BAIXA**

| Complexidade | Avaliação                                      |
| ------------ | ---------------------------------------------- |
| 1-10         | Método simples. Baixo risco.                   |
| 11-20        | Método razoavelmente complexo. Moderado risco. |
| 21-50        | Método muito complexo. Elevado risco.          |
| 51-N         | Método de altíssimo risco e bastante instável. |


   3. **Definir quantos caminhos de execução existem;**
   
       Quantidade de Caminhos: 5
       
       Caminhos: 
*        ABCK;
*        ABDEK;
*        ABDFGK;
*        ABDFHI;
*        ABDFHJK;
       
   
   4. **Definir os casos de teste necessários para se percorrer todos estes caminhos. Cada caso de teste deve ter o valor correspondente para cada variável de entrada e o valor esperado**.

    Variáveis:   **nota1**,  **nota2**,  **faltas**,  **cargaHoraria**

| Caso de Teste | nota1 | nota2 | faltas | cargaHoraria | Saída    |
| ------------- | ----- | ----- | ------ | ------------ | --- |
| CT1           | -5    | 20    | 20     | 40           | "Valores inválidos"    |
| CT2           |  20     | 20      | 40       |   40           | "Reprovado por falta"    |
| CT3           |   10    | 10      |  0      | 40             | "Reprovado por Medio"    |
| CT4           |   40    | 40      |   0     |   40           |  "Prova extra"   |
| CT5           | 80  | 80      |  0      |  40            | "Aprovado"    |
