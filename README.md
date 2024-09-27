# ME-1-LABORATORIO-DE-PROGRAMACAO
Repositório da primeira ME de Laboratório de Programação da UNIMA(Universidade de Maceió) por Antônio Santiago
-------------------------------------------------------------------------------------------------------------------------
1-
public static void main(String[] Args) {  
	        Scanner scanner = new Scanner(System.in);
	        System.out.print("Digite o nome do funcionário: ");
	        String nome = scanner.nextLine();
	        System.out.print("Digite o salário atual do funcionário: ");
	        double salario = scanner.nextDouble();
	        System.out.print("Digite quantos anos ele trabalha na empresa: ");
	        int anosTrabalho = scanner.nextInt();
	        double novoSalario;
	        if (anosTrabalho < 3) {
	            novoSalario = salario + (salario * 0.03); 
	        } else if (anosTrabalho >= 3 && anosTrabalho < 10) {
	            novoSalario = salario + (salario * 0.125); 
	        } else {
	            novoSalario = salario + (salario * 0.20);
	        }
	        System.out.printf("O novo salário de %s é: R$ %.2f\n", nome, novoSalario);
	        scanner.close();
	}	 
-------------------------------------------------------------------------------------------------------------------------
2-
public static void main(String[] Args) {
    Scanner sc = new Scanner(System.in);
		Random rand = new Random();
		System.out.println("SORTEIO DE NÚMEROS: Digite um número entre 1 e 5");
	  int num = sc.nextInt();
	  int num1 = rand.nextInt(5) + 1;
	  System.out.println("Número gerado: " + num1);
	}
-------------------------------------------------------------------------------------------------------------------------
3-
public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Digite o valor da casa: ");
        double valorCasa = scanner.nextDouble();
        System.out.print("Digite o salário do comprador: ");
        double salario = scanner.nextDouble();
        System.out.print("Digite em quantos anos será feito o pagamento: ");
        int anos = scanner.nextInt();
        int meses = anos * 12;
        double prestacaoMensal = valorCasa / meses;
        double limitePrestacao = salario * 0.30;
        System.out.printf("A prestação mensal será de: R$ %.2f\n", prestacaoMensal);
        if (prestacaoMensal <= limitePrestacao) {
            System.out.println("Empréstimo aprovado!");
        } else {
            System.out.println("Empréstimo negado. A prestação excede 30% do salário.");
        }
        scanner.close();
    }
------------------------------------------------------------------------------------------------------------------------------
4-
	public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Digite seu peso (em kg): ");
        double peso = scanner.nextDouble();
        System.out.print("Digite sua altura (em metros): ");
        double altura = scanner.nextDouble();
        double imc = peso / (altura * altura);
        System.out.printf("Seu IMC é: %.2f\n", imc);
        if (imc < 18.5) {
            System.out.println("Abaixo do peso");
        } else if (imc >= 18.5 && imc < 25) {
            System.out.println("Peso ideal");
        } else if (imc >= 25 && imc < 30) {
            System.out.println("Sobrepeso");
        } else if (imc >= 30 && imc < 40) {
            System.out.println("Obesidade");
        } else {
            System.out.println("Obesidade mórbida");
        }
        scanner.close();
    }
------------------------------------------------------------------------------------------------------------------------------
5-
public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Digite o comprimento do primeiro segmento de reta: ");
        double lado1 = scanner.nextDouble();
        System.out.print("Digite o comprimento do segundo segmento de reta: ");
        double lado2 = scanner.nextDouble();
        System.out.print("Digite o comprimento do terceiro segmento de reta: ");
        double lado3 = scanner.nextDouble();
        if ((lado1 < lado2 + lado3) && (lado2 < lado1 + lado3) && (lado3 < lado1 + lado2)) {
            System.out.println("Os segmentos podem formar um triângulo.");
            if (lado1 == lado2 && lado2 == lado3) {
                System.out.println("Tipo de triângulo: Equilátero (todos os lados iguais)");
            } else if (lado1 == lado2 || lado1 == lado3 || lado2 == lado3) {
                System.out.println("Tipo de triângulo: Isósceles (dois lados iguais)");
            } else {
                System.out.println("Tipo de triângulo: Escaleno (todos os lados diferentes)");
            }
        } else {
            System.out.println("Os segmentos não podem formar um triângulo.");
        }
        scanner.close();
    }
------------------------------------------------------------------------------------------------------------------------------
6-
public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Digite um ano: ");
        int ano = scanner.nextInt();
        if ((ano % 4 == 0 && ano % 100 != 0) || (ano % 400 == 0)) {
            System.out.println(ano + " é um ano bissexto.");
        } else {
            System.out.println(ano + " não é um ano bissexto.");
        }
        scanner.close();
    }
------------------------------------------------------------------------------------------------------------------------------
7-
	public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Digite o preço do produto: R$ ");
        double preco = scanner.nextDouble();
        if (preco > 100) {
            preco *= 0.90;
        } else if (preco >= 50 && preco <= 100) {
            preco *= 0.95;
        } else {
            preco = preco; 
        }
        System.out.printf("O preço final do produto é: R$ %.2f%n", preco);
        scanner.close();
    }
------------------------------------------------------------------------------------------------------------------------------
8-
public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Digite um número inteiro: ");
        int n = scanner.nextInt();
        if (n >= 10 && n <= 20) {
            System.out.println("Dentro do intervalo");
        } else {
            System.out.println("Fora do intervalo");
        }
        scanner.close();
    }
------------------------------------------------------------------------------------------------------------------------------
