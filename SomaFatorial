#include<stdio.h>
/*
Desenvolver uma função que, dado um número
inteiro N, *calcule o valor de S*:
S = N - (N-1)/2! + (N-2)/3! - (N-3)/4! + (N-4)/5! - ... 1/N!
*/

//sinalizando que existe uma função
float calculeS(int n);

//main
void main(){
	//declaração de variáveis
	int numero;
	float S;
	
	//comandos 
	printf("Insira um numero: ");
	scanf("%d", &numero);
	
	//chamando a função e retornando a soma 
	S=calculeS(numero);
	
	//mostrando o resultado da SOMA
	printf("A soma e: %.5f", S);
}

//função
float calculeS(int n){
	//declaração de variáveis
	int i, sub, j, fat=1;
	float div, soma, somaNegativo=0, somaPositivo=0;
	
	//varrendo do 'N' até o 1 
	i=1;
	while(sub>1)
	{
		//subtraindo o 'i' de 'n'
		sub=n-i;
		i++;
		//varrendo o fatorial de cada subtração
		fat=1;
		for(j=i; j>=1 ; j--) 
		{
			fat*=j;
		}
		
		//dividindo a subtração pelo fatorial correspondente
		div= (float)sub/fat;
		
		//atribuindo os valores a soma dos sinais correspondentes
		if(i%2==0)
		{
			somaNegativo+=div;
		}else
		{
			somaPositivo+=div;
		}
			
	}
	//somando os valores considerados 'negativos' com os 'positivos' e o 'N'
	soma= n-somaNegativo+somaPositivo;
	
	//retornando o valor para a MAIN
	return soma;
	


}
