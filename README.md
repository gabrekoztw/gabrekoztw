- 👋 Hi, I’m @gabrekoztw
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
gabrekoztw/gabrekoztw is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

import java.util.Scanner;

public class Calculadora {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Menu de opções
        System.out.println("Calculadora Simples");
        System.out.println("Selecione uma operação:");
        System.out.println("1. Adição");
        System.out.println("2. Subtração");
        System.out.println("3. Multiplicação");
        System.out.println("4. Divisão");

        int escolha = scanner.nextInt();

        // Entrada dos números
        System.out.println("Digite o primeiro número:");
        double num1 = scanner.nextDouble();

        System.out.println("Digite o segundo número:");
        double num2 = scanner.nextDouble();

        // Variável para armazenar o resultado
        double resultado = 0;

        // Realização da operação escolhida
        switch (escolha) {
            case 1:
                resultado = num1 + num2;
                System.out.println("Resultado: " + resultado);
                break;
            case 2:
                resultado = num1 - num2;
                System.out.println("Resultado: " + resultado);
                break;
            case 3:
                resultado = num1 * num2;
                System.out.println("Resultado: " + resultado);
                break;
            case 4:
                if (num2 != 0) {
                    resultado = num1 / num2;
                    System.out.println("Resultado: " + resultado);
                } else {
                    System.out.println("Erro: Divisão por zero não é permitida.");
                }
                break;
            default:
                System.out.println("Operação inválida.");
                break;
        }

        scanner.close();
    }
}



