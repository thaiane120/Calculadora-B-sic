# Calculadora-B-sic
Calculadora simples em C para realizar as 4 operações básicas da matemática
#include<stdio.h>
main(){
	float operacao, y,x, resultado;
	printf("insira um numero: ");
	scanf("%f", &x);
	printf("escolha outro numero que deseja fazer a operação: ");
	scanf("%f", &y);
	printf("se deseja multiplicar, digite 1\n se deseja somar, digite 2\n se deseja subtrair digite 3\n se deseja dividir, digite 4\n");
	scanf("%f", &operacao);
	if(operacao==1){
		resultado=x*y;
	}else{
		if(operacao==2){
			resultado=x+y;
			printf("%f", resultado);
		}else{
			if(operacao==3){
				resultado=x-y;
				printf("%f", resultado);
			}else{
				if(operacao==4){
					resultado=x/y;
					printf("%f", resultado);
				}else{
					printf("operacao invalida");
				}
			}
		}
	}
}
