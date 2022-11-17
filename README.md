# lista-Ponteiro
/*numero 1-faça um programa em C que armazene em um vetor 3 valores, e imprima os valores utilizando notação de ponteiro*/
#include <stdio.h>

int main(){
	int vetor[3];
	int *pVetor;
	int i;
	
	for(i=0; i<3; i++){
		printf("Informe um valor: ");
		scanf("%d", &vetor[i]);
	}
	
	for(i=0; i<3; i++){
		pVetor = &vetor[i];
		printf("%d\n", *pVetor);
	}
	
	return 0;
}


#include <stdio.h>
/*numero 2- Crie um programa em C que receba três números do usuário depois crie uma função que receba os 3 números como parâmetros: 
A, B e C. Ordene de tal forma que, ao final da função, A contenha o menor número e C o maior. 
Imprima os três números. Obs: Utilize ponteiro para solucionar o problema*/

void maior( int *a, int *b, int *c){
	if (*a<*b && *c>*b)
	{
		printf("a=%d\tb=%d\tc=%d", *a,*b,*c );
	}
}

int main (){
	
int  vetor[3];
	int *pVetor;
	int i;
	
	for (i=0;i<3;i++){
	printf 	("informe o valor: ");
	scanf ("%d", &vetor[i]);		
	}
	
   for (i=0;i<3; i++){
   pVetor= &vetor[i];
	}

maior(&vetor[0], &vetor[1], &vetor[2]);
}
