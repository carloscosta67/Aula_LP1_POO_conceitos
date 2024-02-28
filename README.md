"#Estudos-casa"  
1. Altere seu programa para imprimir uma mensagem diferente.

2. public class MyFirstJavaProgram {

   /* This is my first java program.
    * This will print 'Hello estou aprendendo Java' as the output
    */

   public static void main(String []args) {
      System.out.println("Hello estou aprendendo Java"); // prints Hello estou aprendendo Java      
      
   }
}
2. Altere seu programa para imprimir duas linhas de texto usando 
duas linhas de código System.out.
public class DuasLinhas {

    public static void main(String[] args) {
        System.out.println("Hello!");
        System.out.println("Estou aprendendo Java!");
    }
}

3. Sabendo que os caracteres \n representam uma quebra de linhas, 
imprima duas linhas de texto usando uma única linha de código 
System.out

public class MyFirstJavaProgram {

   /* Este é meu primeiro programa Java.
    * Este irá imprimir 'Hello , estou aprendendo Java'
    * em duas linhas
    */

   public static void main(String []args) {
      System.out.println("Hello, estou aprendendo Java\n" + "Estou progredindo!"); 
                                                                           
   }
}

1. Na empresa em que trabalhamos, há tabelas com o gasto de cada 
mês. Para fechar o balanço do primeiro trimestre, precisamos 
somar o gasto total. Sabendo que, em janeiro, foram gastos 15 mil 
reais, em fevereiro, 23 mil reais e, em março, 17 mil reais, faça um 
programa que calcule e imprima a despesa total no trimestre e a 
média mensal de gastos.

public class DespesaTrimestral {

    public static void main(String[] args) {
        // Despesas mensais
        int janeiro = 15000;
        int fevereiro = 23000;
        int marco = 17000;

        // Cálculo da despesa total
        int despesaTotal = janeiro + fevereiro + marco;

        // Cálculo da média mensal de gastos
        double mediaMensal = despesaTotal / 3.0;

        // Impressão dos resultados
        System.out.println("Despesa total no trimestre: R$" + despesaTotal);
        System.out.printf("Media mensal de gastos: R$%.2f\n", mediaMensal);
    }
}

2. Programa que leia as notas e calcule a média de LP1 deste 
semestre, referente a um determinado aluno
(P1*0.6+((E1+E2)/2)*0.4)*0.5+(max(((P1*0.6+((E1+E2)/2)*0.4)-5.9),0)/((P1*0.6+((E1+E2)/2)*0.4)-5.9))*(API*0.5)+X+(SUB*0.2)

import java.util.Scanner;

public class MediaLP1 {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Leitura das notas
        System.out.print("Digite a nota da P1: ");
        double p1 = scanner.nextDouble();
        System.out.print("Digite a nota da E1: ");
        double e1 = scanner.nextDouble();
        System.out.print("Digite a nota da E2: ");
        double e2 = scanner.nextDouble();
        System.out.print("Digite a nota da API: ");
        double api = scanner.nextDouble();
        System.out.print("Digite a nota da X: ");
        double x = scanner.nextDouble();
        System.out.print("Digite a nota da SUB: ");
        double sub = scanner.nextDouble();

        // Cálculo da média
         double mediaFinal = (prova1*0.6+((ex1+ex2)/2)*0.4)*0.5+(Math.max(((prova1*0.6+((ex1+ex2)/2)*0.4)-5.9),0)/((prova1*0.6+((ex1+ex2)/2)*0.4)-5.9))*(notaApi*0.5)+exExtra+(provaSub*0.2);

        // Exibição da média
       System.out.printf("A média final do aluno é: %.2f\n", mediaFinal);
       scanner.close();
    }
}
