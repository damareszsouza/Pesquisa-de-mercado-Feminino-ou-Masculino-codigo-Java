# Pesquisa-de-mercado-Feminino-ou-Masculino-codigo-Java


Damares Costa de Souza 
Moodle - IFRS

Programação Básica com Java III - Turma 2022B
Painel Meus cursos  PBJIII2022B 1. Integrando Estruturas de Controle  Teste seus conhecimentos 1
Iniciado em	segunda, 25 jul 2022, 17:47
Estado	Finalizada
Concluída em	segunda, 25 jul 2022, 18:43
Tempo empregado	55 minutos 48 segundos
Avaliar	8,56 de um máximo de 10,00(86%)
Questão 1
Parcialmente correto
Atingiu 0,75 de 1,00
Não marcadaMarcar questão
Texto da questão
Considere o seguinte enunciado de problema:

Um aluno realizou três provas de uma disciplina. Considerando o critério abaixo, faça um programa que mostre se ele ficou para exame. Em caso positivo, leia a nota do exame e verifique se conseguiu a aprovação ou não.

Imagem mostra a fórmula: média igual a prova 1 mais prova 2 mais prova 3 dividido por 3.

A média deve ser maior ou igual a 7,0. Se não conseguir, a nova média deve ser:

Imagem mostra a seguinte fórmula: final igual a média mais exame dividido por 2

Nesse caso, a média final deve ser maior ou igual a 5,0.

Complete o programa abaixo, arrastando e soltando os trechos de código nos lugares corretos, de forma que implemente corretamente uma solução para o problema acima.



public class ExameEstudante {
	public static void main(String[] args) {
		System.out.print("Nota na prova 1: ");
		double prova1 = Double.parseDouble(System.console().readLine());
		System.out.print("Nota na prova 2: ");
		double prova2 = Double.parseDouble(System.console().readLine());
		System.out.print("Nota na prova 3: ");
		double prova3 = Double.parseDouble(System.console().readLine());
		
		double media = (prova1 + prova2 + prova3) / 3; 
		System.out.printf("\nMEDIA = %.1f\n", media); 
		
		System.out.printf("MEDIA FINAL = %.1f\n", mediaFinal);  {
			System.out.println("O estudante nao ficou em exame.");
		} else  {
			System.out.println("O estudante ficou em exame.");
			System.out.print("Informe a nota dele no exame: ");
			double exame = Double.parseDouble(System.console().readLine());
			
			double mediaFinal = (media + exame) / 2; 
			if(media >= 7) 
			
			if(mediaFinal >= 5) 
				System.out.println("O estudante foi aprovado!"); 
			else
				System.out.println("O estudante foi reprovado :(");
		}
	}
}

       
Feedback
Sua resposta está parcialmente correta.
Você selecionou corretamente 6.
A resposta correta é:
Considere o seguinte enunciado de problema:

Um aluno realizou três provas de uma disciplina. Considerando o critério abaixo, faça um programa que mostre se ele ficou para exame. Em caso positivo, leia a nota do exame e verifique se conseguiu a aprovação ou não.

Imagem mostra a fórmula: média igual a prova 1 mais prova 2 mais prova 3 dividido por 3.

A média deve ser maior ou igual a 7,0. Se não conseguir, a nova média deve ser:

Imagem mostra a seguinte fórmula: final igual a média mais exame dividido por 2

Nesse caso, a média final deve ser maior ou igual a 5,0.

Complete o programa abaixo, arrastando e soltando os trechos de código nos lugares corretos, de forma que implemente corretamente uma solução para o problema acima.



public class ExameEstudante {
	public static void main(String[] args) {
		System.out.print("Nota na prova 1: ");
		double prova1 = Double.parseDouble(System.console().readLine());
		System.out.print("Nota na prova 2: ");
		double prova2 = Double.parseDouble(System.console().readLine());
		System.out.print("Nota na prova 3: ");
		double prova3 = Double.parseDouble(System.console().readLine());
		
		[double media = (prova1 + prova2 + prova3) / 3;]
		[System.out.printf("\nMEDIA = %.1f\n", media);]
		
		[if(media >= 7)] {
			System.out.println("O estudante nao ficou em exame.");
		} [else] {
			System.out.println("O estudante ficou em exame.");
			System.out.print("Informe a nota dele no exame: ");
			double exame = Double.parseDouble(System.console().readLine());
			
			[double mediaFinal = (media + exame) / 2;]
			[System.out.printf("MEDIA FINAL = %.1f\n", mediaFinal);]
			
			[if(mediaFinal >= 5)]
				[System.out.println("O estudante foi aprovado!");]
			else
				System.out.println("O estudante foi reprovado :(");
		}
	}
}

Questão 2
Correto
Atingiu 1,00 de 1,00
Não marcadaMarcar questão
Texto da questão
Considere o seguinte problema:

Foi feita uma estatística em 20 cidades brasileiras para coletar dados sobre acidentes de trânsito. Para cada cidade, foram obtidos os seguintes dados:

código da cidade;
número de veículos de passeio (em 2017);
número de acidentes de trânsito com vítimas (em 2017).
Faça um programa que calcule e mostre:

o código da cidade com o maior número de acidentes de trânsito;
o código da cidade com o menor número de acidentes de trânsito;
a média de veículos entre as 20 cidades;
a média de acidentes de trânsito nas cidades com menos de 2.000 veículos de passeio.
Complete o programa abaixo, arrastando e soltando os trechos de código, de forma que o problema cima seja corretamente implementado.



public class AnalisaTransitoCidades {
	public static void main(String[] args) {
		int maiorNumAcidentes = -1, codCidadeMaiorNumAcid = 0, menorNumAcidentes = -1, codCidadeMenorNumAcid = 0, 
			somaVeiculos = 0, numCidInf2000Veic = 0, somaAcidCidInf2000Veic = 0;
		
		for(int cont = 1; cont <= 20; cont++)  {
			System.out.printf("------------------------ CIDADE %02d ------------------------\n", cont);
			System.out.print("Codigo: ");
			int codigo = Integer.parseInt(System.console().readLine());
			System.out.print("Numero de veiculos de passeio em 2017: ");
			int veiculosPasseio = Integer.parseInt(System.console().readLine());
			System.out.print("Numero de acidentes de transito com vitimas em 2017: ");
			int numAcidentes = Integer.parseInt(System.console().readLine());
			
			if(numAcidentes > maiorNumAcidentes)  {
				maiorNumAcidentes = numAcidentes;
				codCidadeMaiorNumAcid = codigo;
			}
			if(numAcidentes < menorNumAcidentes || menorNumAcidentes == ‑1)  {
				menorNumAcidentes = numAcidentes;
				codCidadeMenorNumAcid = codigo;
			}
			somaVeiculos += veiculosPasseio;
			if(veiculosPasseio < 2000)  {
				numCidInf2000Veic++;
				somaAcidCidInf2000Veic += numAcidentes;
			}
		}
		
		double mediaVeiculos = somaVeiculos / 20.0;
		double mediaAcidCidInf2000Veic = somaAcidCidInf2000Veic / (double) numCidInf2000Veic;
		
		System.out.printf("\nCODIGO DA CIDADE COM O MAIOR NUMERO DE ACIDENTES = %d\n", codCidadeMaiorNumAcid);
		System.out.printf("CODIGO DA CIDADE COM O MENOR NUMERO DE ACIDENTES = %d\n", codCidadeMenorNumAcid);
		System.out.printf("MEDIA DE VEICULOS DE PASSEIO = %.1f\n", mediaVeiculos);
		System.out.printf("MEDIA DE ACIDENTES NAS CIDADES COM MENOS DE 2000 VEICULOS DE PASSEIO = %.1f\n", mediaAcidCidInf2000Veic);
	}
}

   
Feedback
Sua resposta está correta.
A resposta correta é:
Considere o seguinte problema:

Foi feita uma estatística em 20 cidades brasileiras para coletar dados sobre acidentes de trânsito. Para cada cidade, foram obtidos os seguintes dados:

código da cidade;
número de veículos de passeio (em 2017);
número de acidentes de trânsito com vítimas (em 2017).
Faça um programa que calcule e mostre:

o código da cidade com o maior número de acidentes de trânsito;
o código da cidade com o menor número de acidentes de trânsito;
a média de veículos entre as 20 cidades;
a média de acidentes de trânsito nas cidades com menos de 2.000 veículos de passeio.
Complete o programa abaixo, arrastando e soltando os trechos de código, de forma que o problema cima seja corretamente implementado.



public class AnalisaTransitoCidades {
	public static void main(String[] args) {
		int maiorNumAcidentes = -1, codCidadeMaiorNumAcid = 0, menorNumAcidentes = -1, codCidadeMenorNumAcid = 0, 
			somaVeiculos = 0, numCidInf2000Veic = 0, somaAcidCidInf2000Veic = 0;
		
		[for(int cont = 1; cont <= 20; cont++)] {
			System.out.printf("------------------------ CIDADE %02d ------------------------\n", cont);
			System.out.print("Codigo: ");
			int codigo = Integer.parseInt(System.console().readLine());
			System.out.print("Numero de veiculos de passeio em 2017: ");
			int veiculosPasseio = Integer.parseInt(System.console().readLine());
			System.out.print("Numero de acidentes de transito com vitimas em 2017: ");
			int numAcidentes = Integer.parseInt(System.console().readLine());
			
			[if(numAcidentes > maiorNumAcidentes)] {
				maiorNumAcidentes = numAcidentes;
				codCidadeMaiorNumAcid = codigo;
			}
			[if(numAcidentes < menorNumAcidentes || menorNumAcidentes == ‑1)] {
				menorNumAcidentes = numAcidentes;
				codCidadeMenorNumAcid = codigo;
			}
			somaVeiculos += veiculosPasseio;
			[if(veiculosPasseio < 2000)] {
				numCidInf2000Veic++;
				somaAcidCidInf2000Veic += numAcidentes;
			}
		}
		
		double mediaVeiculos = somaVeiculos / 20.0;
		double mediaAcidCidInf2000Veic = somaAcidCidInf2000Veic / (double) numCidInf2000Veic;
		
		System.out.printf("\nCODIGO DA CIDADE COM O MAIOR NUMERO DE ACIDENTES = %d\n", codCidadeMaiorNumAcid);
		System.out.printf("CODIGO DA CIDADE COM O MENOR NUMERO DE ACIDENTES = %d\n", codCidadeMenorNumAcid);
		System.out.printf("MEDIA DE VEICULOS DE PASSEIO = %.1f\n", mediaVeiculos);
		System.out.printf("MEDIA DE ACIDENTES NAS CIDADES COM MENOS DE 2000 VEICULOS DE PASSEIO = %.1f\n", mediaAcidCidInf2000Veic);
	}
}

Questão 3
Correto
Atingiu 1,00 de 1,00
Não marcadaMarcar questão
Texto da questão
Considere o seguinte problema:

Faça um programa que receba a idade, a altura e o peso de 25 pessoas, calcule e mostre:

a quantidade de pessoas com idade superior a 50 anos;
a média das alturas das pessoas com idade entre 10 e 20 anos;
a percentagem de pessoas com peso inferior a 40 quilos entre todas as pessoas analisadas.
Complete o programa abaixo, arrastando e soltando os trechos de código nos espaços vazios de forma que o problema acima seja implementado de forma correta.



public class AnalisePessoas {
	public static void main(String[] args) {
		int quantMaior50 = 0, quantEntre10e20 = 0, quantInf40Kg = 0;
		double somaAlturas = 0; 
		
		for(int cont = 1; cont <= 25; cont++)  {
			System.out.printf("------------------------ PESSOA %02d ------------------------\n", cont);
			System.out.print("Idade: ");
			int idade = Integer.parseInt(System.console().readLine());
			System.out.print("Altura: ");
			double altura = Double.parseDouble(System.console().readLine());
			System.out.print("Peso: ");
			double peso = Double.parseDouble(System.console().readLine());
			
			if(idade > 50) 
				quantMaior50++; 
			else if(idade >= 10 && idade <= 20)  {
				somaAlturas += altura;
				quantEntre10e20++; 
			}
			
			if(peso < 40)
				quantInf40Kg++;
		}
		
		double mediaAlturas = somaAlturas / quantEntre10e20;
		double percInf40Kg = quantInf40Kg * 100.0 / 25;
		
		System.out.printf("\nQUANTIDADE DE PESSOAS COM MAIS DE 50 ANOS = %d\n", quantMaior50);
		System.out.printf("MEDIA DAS ALTURAS DAS PESSOAS ENTRE 10 E 20 ANOS = %.2f metros\n", mediaAlturas);
		System.out.printf("PERCENTAGEM DE PESSOAS COM MENOS DE 40 KG = %.1f%%\n", percInf40Kg);
	}
}

     
Feedback
Sua resposta está correta.
A resposta correta é:
Considere o seguinte problema:

Faça um programa que receba a idade, a altura e o peso de 25 pessoas, calcule e mostre:

a quantidade de pessoas com idade superior a 50 anos;
a média das alturas das pessoas com idade entre 10 e 20 anos;
a percentagem de pessoas com peso inferior a 40 quilos entre todas as pessoas analisadas.
Complete o programa abaixo, arrastando e soltando os trechos de código nos espaços vazios de forma que o problema acima seja implementado de forma correta.



public class AnalisePessoas {
	public static void main(String[] args) {
		int quantMaior50 = 0, quantEntre10e20 = 0, quantInf40Kg = 0;
		[double somaAlturas = 0;]
		
		[for(int cont = 1; cont <= 25; cont++)] {
			System.out.printf("------------------------ PESSOA %02d ------------------------\n", cont);
			System.out.print("Idade: ");
			int idade = Integer.parseInt(System.console().readLine());
			System.out.print("Altura: ");
			double altura = Double.parseDouble(System.console().readLine());
			System.out.print("Peso: ");
			double peso = Double.parseDouble(System.console().readLine());
			
			[if(idade > 50)]
				[quantMaior50++;]
			else [if(idade >= 10 && idade <= 20)] {
				somaAlturas += altura;
				[quantEntre10e20++;]
			}
			
			if(peso < 40)
				quantInf40Kg++;
		}
		
		double mediaAlturas = somaAlturas / quantEntre10e20;
		double percInf40Kg = quantInf40Kg * 100.0 / 25;
		
		System.out.printf("\nQUANTIDADE DE PESSOAS COM MAIS DE 50 ANOS = %d\n", quantMaior50);
		System.out.printf("MEDIA DAS ALTURAS DAS PESSOAS ENTRE 10 E 20 ANOS = %.2f metros\n", mediaAlturas);
		System.out.printf("PERCENTAGEM DE PESSOAS COM MENOS DE 40 KG = %.1f%%\n", percInf40Kg);
	}
}

Questão 4
Correto
Atingiu 1,00 de 1,00
Não marcadaMarcar questão
Texto da questão
Considere o enunciado do problema abaixo:

Faça um programa que receba a idade de 15 pessoas, calcule e mostre quantidade de pessoas em cada faixa etária, conforme os critérios abaixo:

Faixa 1: até 15 anos
Faixa 2: de 16 a 30 anos
Faixa 3: de 31 a 45 anos
Faixa 4: de 46 a 60 anos
Faixa 5: acima de 60 anos
Complete o programa abaixo, arrastando e soltando os trechos de código nos espaços vazios, de forma que o programa implemente corretamente uma solução para o problema acima.



public class VerificaFaixaEtaria {
	public static void main(String[] args) {
		int faixa1 = 0, faixa2 = 0, faixa3 = 0, faixa4 = 0, faixa5 = 0;
		
		for(int cont = 1; cont <= 15; cont++)  {
			System.out.printf("Informe a idade da %da pessoa: ", cont); 
			int idade = Integer.parseInt(System.console().readLine()); 
			
			if(idade <= 15) 
				faixa1++; 
			else if(idade <= 30) 
				faixa2++; 
			else if(idade <= 45) 
				faixa3++; 
			else if(idade <= 60) 
				faixa4++; 
			else
				faixa5++;
		}
		
		System.out.printf("\nPESSOAS NA FAIXA 1 = %d\n", faixa1);
		System.out.printf("PESSOAS NA FAIXA 2 = %d\n", faixa2);
		System.out.printf("PESSOAS NA FAIXA 3 = %d\n", faixa3);
		System.out.printf("PESSOAS NA FAIXA 4 = %d\n", faixa4);
		System.out.printf("PESSOAS NA FAIXA 5 = %d\n", faixa5);
	}
}

          
Feedback
Sua resposta está correta.
A resposta correta é:
Considere o enunciado do problema abaixo:

Faça um programa que receba a idade de 15 pessoas, calcule e mostre quantidade de pessoas em cada faixa etária, conforme os critérios abaixo:

Faixa 1: até 15 anos
Faixa 2: de 16 a 30 anos
Faixa 3: de 31 a 45 anos
Faixa 4: de 46 a 60 anos
Faixa 5: acima de 60 anos
Complete o programa abaixo, arrastando e soltando os trechos de código nos espaços vazios, de forma que o programa implemente corretamente uma solução para o problema acima.



public class VerificaFaixaEtaria {
	public static void main(String[] args) {
		int faixa1 = 0, faixa2 = 0, faixa3 = 0, faixa4 = 0, faixa5 = 0;
		
		[for(int cont = 1; cont <= 15; cont++)] {
			[System.out.printf("Informe a idade da %da pessoa: ", cont);]
			[int idade = Integer.parseInt(System.console().readLine());]
			
			[if(idade <= 15)]
				[faixa1++;]
			else [if(idade <= 30)]
				[faixa2++;]
			else [if(idade <= 45)]
				[faixa3++;]
			else [if(idade <= 60)]
				[faixa4++;]
			else
				faixa5++;
		}
		
		System.out.printf("\nPESSOAS NA FAIXA 1 = %d\n", faixa1);
		System.out.printf("PESSOAS NA FAIXA 2 = %d\n", faixa2);
		System.out.printf("PESSOAS NA FAIXA 3 = %d\n", faixa3);
		System.out.printf("PESSOAS NA FAIXA 4 = %d\n", faixa4);
		System.out.printf("PESSOAS NA FAIXA 5 = %d\n", faixa5);
	}
}

Questão 5
Parcialmente correto
Atingiu 0,71 de 1,00
Não marcadaMarcar questão
Texto da questão
Considere o seguinte problema:

Faça um programa que receba dez idades, pesos e alturas, calcule e mostre:

a média de idades das dez pessoas;
a quantidade de pessoas com peso superior a 90 quilos e altura inferior a 1,50 metro;
a percentagem de pessoas com idade entre 10 e 30 anos entre as pessoas que medem mais de 1,90 metros.
Complete o programa abaixo, arrastando e soltando os trechos de código nos espaços em branco, de forma que a solução para o problema acima seja implementada corretamente.



public class CalculosPessoas {
	public static void main(String[] args) {
		 em branco 
		
		for(int cont = 1; cont <= 10; cont++)  {
			System.out.printf("------------------------ PESSOA %02d ------------------------\n", cont);
			System.out.print("Idade: ");
			int idade = Integer.parseInt(System.console().readLine());
			System.out.print("Altura: ");
			double altura = Double.parseDouble(System.console().readLine());
			System.out.print("Peso: "); 
			double peso = Double.parseDouble(System.console().readLine()); 
			
			somaIdades += idade;
			if(idade >= 10 && idade <= 30) 
				quantSup90Inf150++;
			if(altura > 1.90)  {
				quantSup190++;
				if(peso > 90 && altura < 1.50) 
					quantSup190Entre10E30++;
			}
		}
		
		double mediaIdades = somaIdades / 10.0;
		double percSup190Entre10E30 = quantSup190Entre10E30 * 100.0 / quantSup190;
		
		System.out.printf("\nMEDIA DE IDADE DAS PESSOAS = %d\n", mediaIdades);
		System.out.printf("QUANTIDADE DE PESSOAS COM PESO SUPERIOR A 90 KG e ALTURA INFERIOR A 1,50M = %d\n", quantSup90Inf150);
		System.out.printf("PERCENTAGEM DE PESSOAS COM MAIS DE 1,90M DE ALTURA COM IDADE ENTRE 10 E 30 ANOS = %.1f%%\n", percSup190Entre10E30);
	}
}

      int somaIdades = 0, quantSup90Inf150 = 0, quantSup190 = 0, quantSup190Entre10E30 = 0;
Feedback
Sua resposta está parcialmente correta.
Você selecionou corretamente 5.
A resposta correta é:
Considere o seguinte problema:

Faça um programa que receba dez idades, pesos e alturas, calcule e mostre:

a média de idades das dez pessoas;
a quantidade de pessoas com peso superior a 90 quilos e altura inferior a 1,50 metro;
a percentagem de pessoas com idade entre 10 e 30 anos entre as pessoas que medem mais de 1,90 metros.
Complete o programa abaixo, arrastando e soltando os trechos de código nos espaços em branco, de forma que a solução para o problema acima seja implementada corretamente.



public class CalculosPessoas {
	public static void main(String[] args) {
		[int somaIdades = 0, quantSup90Inf150 = 0, quantSup190 = 0, quantSup190Entre10E30 = 0;]
		
		[for(int cont = 1; cont <= 10; cont++)] {
			System.out.printf("------------------------ PESSOA %02d ------------------------\n", cont);
			System.out.print("Idade: ");
			int idade = Integer.parseInt(System.console().readLine());
			System.out.print("Altura: ");
			double altura = Double.parseDouble(System.console().readLine());
			[System.out.print("Peso: ");]
			[double peso = Double.parseDouble(System.console().readLine());]
			
			somaIdades += idade;
			[if(peso > 90 && altura < 1.50)]
				quantSup90Inf150++;
			[if(altura > 1.90)] {
				quantSup190++;
				[if(idade >= 10 && idade <= 30)]
					quantSup190Entre10E30++;
			}
		}
		
		double mediaIdades = somaIdades / 10.0;
		double percSup190Entre10E30 = quantSup190Entre10E30 * 100.0 / quantSup190;
		
		System.out.printf("\nMEDIA DE IDADE DAS PESSOAS = %d\n", mediaIdades);
		System.out.printf("QUANTIDADE DE PESSOAS COM PESO SUPERIOR A 90 KG e ALTURA INFERIOR A 1,50M = %d\n", quantSup90Inf150);
		System.out.printf("PERCENTAGEM DE PESSOAS COM MAIS DE 1,90M DE ALTURA COM IDADE ENTRE 10 E 30 ANOS = %.1f%%\n", percSup190Entre10E30);
	}
}

Questão 6
Parcialmente correto
Atingiu 0,67 de 1,00
Não marcadaMarcar questão
Texto da questão
Complete o programa abaixo, arrastando e soltando os trechos de código nos espaços vazios, de forma que receba dez números inteiros e mostre a soma dos números pares dentre eles.



public class SomaPares {
	public static void main(String[] args) {
		int numero = Integer.parseInt(System.console().readLine()); 
		
		 em branco  {
			System.out.printf("Informe o %do numero: ", cont); 
			int soma = 0; 
			
			if(numero % 2 == 0) 
				soma += numero; 
		}
		
		System.out.printf("\nSOMA DOS NUMEROS PARES = %d\n", soma);
	}
}

  for(int cont = 1; cont <= 10; cont++)   
Feedback
Sua resposta está parcialmente correta.
Você selecionou corretamente 4.
A resposta correta é:
Complete o programa abaixo, arrastando e soltando os trechos de código nos espaços vazios, de forma que receba dez números inteiros e mostre a soma dos números pares dentre eles.



public class SomaPares {
	public static void main(String[] args) {
		[int soma = 0;]
		
		[for(int cont = 1; cont <= 10; cont++)] {
			[System.out.printf("Informe o %do numero: ", cont);]
			[int numero = Integer.parseInt(System.console().readLine());]
			
			[if(numero % 2 == 0)]
				[soma += numero;]
		}
		
		System.out.printf("\nSOMA DOS NUMEROS PARES = %d\n", soma);
	}
}

Questão 7
Correto
Atingiu 1,00 de 1,00
Não marcadaMarcar questão
Texto da questão
Considere o seguinte enunciado de um problema:

Um banco concederá um crédito especial aos seus clientes, de acordo com o saldo médio no último ano. Faça um programa que receba o saldo médio de um cliente e calcule o valor do crédito, de acordo com os seguintes critérios:

Caso o saldo médio seja maior que R$ 1000,00, o percentual de crédito será de 30% do saldo médio.
Caso o saldo médio seja maior que R$ 800,00 e menor ou igual a R$ 1000,00, o percentual de crédito será de 25% do saldo médio.
Caso o saldo médio seja maior que R$ 600,00 e menor ou igual a R$ 800,00, o percentual de crédito será de 20% do saldo médio.
Caso o saldo médio seja menor ou igual a R$ 600,00, o percentual de crédito será de 10% do saldo médio.
Mostre o saldo médio e o valor do crédito.

Complete o programa em Java abaixo, arrastando e soltando os códigos nos lugares corretos, de forma que implemente corretamente uma solução para o problema acima.



public class CalculaCredito {
	public static void main(String[] args) {
		double saldoMedio, valorCredito = 0; 
		
		System.out.print("Saldo medio no ano anterior: ");
		saldoMedio = Double.parseDouble(System.console().readLine());
				
		if(saldoMedio > 1000) 
			valorCredito = saldoMedio * 30 / 100;
		else if(saldoMedio > 800) 
			valorCredito = saldoMedio * 25 / 100;
		else  em branco 
			valorCredito = saldoMedio * 20 / 100;
		else  
			valorCredito = saldoMedio * 10 / 100;
		
		System.out.printf("\nSALDO MEDIO = R$ %.2f\n", saldoMedio);
		System.out.printf("VALOR DO CREDITO = R$ %.2f\n", valorCredito); 
	}
}

  if(saldoMedio > 600)   
Feedback
Sua resposta está correta.
A resposta correta é:
Considere o seguinte enunciado de um problema:

Um banco concederá um crédito especial aos seus clientes, de acordo com o saldo médio no último ano. Faça um programa que receba o saldo médio de um cliente e calcule o valor do crédito, de acordo com os seguintes critérios:

Caso o saldo médio seja maior que R$ 1000,00, o percentual de crédito será de 30% do saldo médio.
Caso o saldo médio seja maior que R$ 800,00 e menor ou igual a R$ 1000,00, o percentual de crédito será de 25% do saldo médio.
Caso o saldo médio seja maior que R$ 600,00 e menor ou igual a R$ 800,00, o percentual de crédito será de 20% do saldo médio.
Caso o saldo médio seja menor ou igual a R$ 600,00, o percentual de crédito será de 10% do saldo médio.
Mostre o saldo médio e o valor do crédito.

Complete o programa em Java abaixo, arrastando e soltando os códigos nos lugares corretos, de forma que implemente corretamente uma solução para o problema acima.



public class CalculaCredito {
	public static void main(String[] args) {
		[double saldoMedio, valorCredito = 0;]
		
		System.out.print("Saldo medio no ano anterior: ");
		saldoMedio = Double.parseDouble(System.console().readLine());
				
		[if(saldoMedio > 1000)]
			valorCredito = saldoMedio * 30 / 100;
		else [if(saldoMedio > 800)]
			valorCredito = saldoMedio * 25 / 100;
		else [if(saldoMedio > 600)]
			valorCredito = saldoMedio * 20 / 100;
		[else] 
			valorCredito = saldoMedio * 10 / 100;
		
		System.out.printf("\nSALDO MEDIO = R$ %.2f\n", saldoMedio);
		[System.out.printf("VALOR DO CREDITO = R$ %.2f\n", valorCredito);]
	}
}

Questão 8
Parcialmente correto
Atingiu 0,43 de 1,00
Não marcadaMarcar questão
Texto da questão
Considere o seguinte problema:

Foi feita uma pesquisa sobre a audiência de canal de TV em várias casas de uma cidade, em determinado dia. Para cada casa consultada foi fornecido o número do canal (4, 5, 7, 12) e o número de pessoas que estavam assistindo àquele canal. Se a televisão estivesse desligada, nada era anotado, ou seja, essa casa não entrava na pesquisa. Faça um programa que:

leia um número indeterminado de dados (número do canal e número de pessoas que estavam assistindo);
calcule e mostre a percentagem de audiência de cada canal.
Para encerrar a entrada de dados, digite o número do canal ZERO.

Complete o programa abaixo de forma que implemente corretamente o problema acima.



public class PesquisaAudiencia {
	public static void main(String[] args) {
		int canal, cont = 1, canal4 = 0, canal5 = 0, canal7 = 0, canal12 = 0, totalPessoas = 0; 
		do  {
			System.out.printf("------------------------ CASA %02d ------------------------\n", cont);
			 em branco 
			 em branco 
			if(canal != 0) {
				System.out.print("Numero de pessoas assistindo o canal: ");
				int numPessoas = Integer.parseInt(System.console().readLine());
				totalPessoas += numPessoas;  {
					case 4: canal4 += numPessoas; break;
					case 5: canal5 += numPessoas; break;
					case 7: canal7 += numPessoas; break;
					case 12: canal12 += numPessoas; break;
				}
				cont++;
				switch(canal) 
			}
		} while(canal != 0) ;
		
		double percCanal4 = canal4 * 100.0 / totalPessoas;
		double percCanal5 = canal5 * 100.0 / totalPessoas;
		double percCanal7 = canal7 * 100.0 / totalPessoas;
		double percCanal12 = canal12 * 100.0 / totalPessoas;
		
		System.out.printf("\nPERCENTUAL DE AUDIENCIA DO CANAL 4 = %.1f%%\n", percCanal4);
		System.out.printf("\nPERCENTUAL DE AUDIENCIA DO CANAL 5 = %.1f%%\n", percCanal5);
		System.out.printf("\nPERCENTUAL DE AUDIENCIA DO CANAL 7 = %.1f%%\n", percCanal7);
		System.out.printf("\nPERCENTUAL DE AUDIENCIA DO CANAL 12 = %.1f%%\n", percCanal12);
	}
}

 System.out.print("Canal que estavam assistindo (4, 5, 7 ou 12): ");    canal = Integer.parseInt(System.console().readLine()); 
Feedback
Sua resposta está parcialmente correta.
Você selecionou corretamente 3.
A resposta correta é:
Considere o seguinte problema:

Foi feita uma pesquisa sobre a audiência de canal de TV em várias casas de uma cidade, em determinado dia. Para cada casa consultada foi fornecido o número do canal (4, 5, 7, 12) e o número de pessoas que estavam assistindo àquele canal. Se a televisão estivesse desligada, nada era anotado, ou seja, essa casa não entrava na pesquisa. Faça um programa que:

leia um número indeterminado de dados (número do canal e número de pessoas que estavam assistindo);
calcule e mostre a percentagem de audiência de cada canal.
Para encerrar a entrada de dados, digite o número do canal ZERO.

Complete o programa abaixo de forma que implemente corretamente o problema acima.



public class PesquisaAudiencia {
	public static void main(String[] args) {
		[int canal, cont = 1, canal4 = 0, canal5 = 0, canal7 = 0, canal12 = 0, totalPessoas = 0;]
		[do] {
			System.out.printf("------------------------ CASA %02d ------------------------\n", cont);
			[System.out.print("Canal que estavam assistindo (4, 5, 7 ou 12): ");]
			[canal = Integer.parseInt(System.console().readLine());]
			if(canal != 0) {
				System.out.print("Numero de pessoas assistindo o canal: ");
				int numPessoas = Integer.parseInt(System.console().readLine());
				[switch(canal)] {
					case 4: canal4 += numPessoas; break;
					case 5: canal5 += numPessoas; break;
					case 7: canal7 += numPessoas; break;
					case 12: canal12 += numPessoas; break;
				}
				cont++;
				[totalPessoas += numPessoas;]
			}
		} [while(canal != 0)];
		
		double percCanal4 = canal4 * 100.0 / totalPessoas;
		double percCanal5 = canal5 * 100.0 / totalPessoas;
		double percCanal7 = canal7 * 100.0 / totalPessoas;
		double percCanal12 = canal12 * 100.0 / totalPessoas;
		
		System.out.printf("\nPERCENTUAL DE AUDIENCIA DO CANAL 4 = %.1f%%\n", percCanal4);
		System.out.printf("\nPERCENTUAL DE AUDIENCIA DO CANAL 5 = %.1f%%\n", percCanal5);
		System.out.printf("\nPERCENTUAL DE AUDIENCIA DO CANAL 7 = %.1f%%\n", percCanal7);
		System.out.printf("\nPERCENTUAL DE AUDIENCIA DO CANAL 12 = %.1f%%\n", percCanal12);
	}
}

Questão 9
Correto
Atingiu 1,00 de 1,00
Não marcadaMarcar questão
Texto da questão
Considere o problema abaixo:

Uma empresa fez uma pesquisa de mercado para saber se as pessoas gostaram ou não de um novo produto lançado no mercado. Para isso, forneceu o sexo do entrevistado e sua resposta (S – sim ou N – não). Sabe-se que foram entrevistadas dez pessoas. Faça um programa que leia essas informações para cada pessoa, calcule e mostre:

o número de pessoas que responderam sim;
o número de pessoas que responderam não;
o número de mulheres que responderam sim;
a porcentagem de homens que responderam não, entre todos os homens analisados.
Complete o programa abaixo, arrastando e soltando os trechos de código nos espaços em branco, de forma que o problema acima seja corretamente implementado.



public class Pesquisa {
	public static void main(String[] args) {
		int numSim = 0, numNao = 0, numMulheresSim = 0, numHomensNao = 0, numHomens = 0; 
		
		 em branco  {
			System.out.printf("------------------------ PESSOA %02d ------------------------\n", cont);
			System.out.print("Sexo (M ou F): ");
			char sexo = System.console().readLine().charAt(0);
			System.out.print("Resposta (S - sim ou N - nao): ");
			char resposta = System.console().readLine().charAt(0);
			
			if(resposta == 'S' || resposta == 's')  {
				numSim++;
				if(sexo == 'F' || sexo == 'f') 
					numMulheresSim++;
			} else {
				numNao++; 
				if(sexo == 'M' || sexo == 'm') 
					numHomensNao++;
			}
			if(sexo == 'M' || sexo == 'm')
				numHomens++; 
		}
		
		double percHomensNao = numHomensNao * 100.0 / numHomens; 
		
		System.out.printf("\nNUMERO DE PESSOAS QUE RESPONDERAM SIM = %d\n", numSim);
		System.out.printf("NUMERO DE PESSOAS QUE RESPONDERAM NAO = %d\n", numNao);
		System.out.printf("NUMERO DE MULHERES QUE RESPONDERAM SIM = %d\n", numMulheresSim);
		System.out.printf("PORCENTAGEM DE HOMENS QUE RESPONDERAM NAO = %.1f%%\n", percHomensNao);
	}
}

      for(int cont = 1; cont <= 10; cont++) 
Feedback
Sua resposta está correta.
A resposta correta é:
Considere o problema abaixo:

Uma empresa fez uma pesquisa de mercado para saber se as pessoas gostaram ou não de um novo produto lançado no mercado. Para isso, forneceu o sexo do entrevistado e sua resposta (S – sim ou N – não). Sabe-se que foram entrevistadas dez pessoas. Faça um programa que leia essas informações para cada pessoa, calcule e mostre:

o número de pessoas que responderam sim;
o número de pessoas que responderam não;
o número de mulheres que responderam sim;
a porcentagem de homens que responderam não, entre todos os homens analisados.
Complete o programa abaixo, arrastando e soltando os trechos de código nos espaços em branco, de forma que o problema acima seja corretamente implementado.



public class Pesquisa {
	public static void main(String[] args) {
		[int numSim = 0, numNao = 0, numMulheresSim = 0, numHomensNao = 0, numHomens = 0;]
		
		[for(int cont = 1; cont <= 10; cont++)] {
			System.out.printf("------------------------ PESSOA %02d ------------------------\n", cont);
			System.out.print("Sexo (M ou F): ");
			char sexo = System.console().readLine().charAt(0);
			System.out.print("Resposta (S - sim ou N - nao): ");
			char resposta = System.console().readLine().charAt(0);
			
			[if(resposta == 'S' || resposta == 's')] {
				numSim++;
				[if(sexo == 'F' || sexo == 'f')]
					numMulheresSim++;
			} else {
				[numNao++;]
				[if(sexo == 'M' || sexo == 'm')]
					numHomensNao++;
			}
			if(sexo == 'M' || sexo == 'm')
				[numHomens++;]
		}
		
		[double percHomensNao = numHomensNao * 100.0 / numHomens;]
		
		System.out.printf("\nNUMERO DE PESSOAS QUE RESPONDERAM SIM = %d\n", numSim);
		System.out.printf("NUMERO DE PESSOAS QUE RESPONDERAM NAO = %d\n", numNao);
		System.out.printf("NUMERO DE MULHERES QUE RESPONDERAM SIM = %d\n", numMulheresSim);
		System.out.printf("PORCENTAGEM DE HOMENS QUE RESPONDERAM NAO = %.1f%%\n", percHomensNao);
	}
}
