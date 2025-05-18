# bmi.c
include <stdio.h>

int main() {
	float peso;
	float altura;
	float bmi;
	
	printf("Ingrese su peso: ");
	scanf("%d", &peso);
	printf("Ingrese su altura: ");
	scanf("%f", &altura);
	
	bmi=peso/(altura*altura);
	
	printf("Su indice de masa corporal es: %2.f\n ",bmi);
	
	if(bmi<18.5){
		printf("Usted tiene Bajo peso");
	}else if(bmi>=18.5 && bmi<24.9){
		printf("Usted esta Normal\n");
	}else if(bmi>=25 && bmi<29.9){
		printf("Usted tiene Sobrepeso\n");
	}else{
		printf("Usted tiene Obesidad\n");
	}
	
	printf("Indice | Condición\n");
	printf("------------------------------\n");
	printf("<18.5  | Bajo peso\n");
	printf("18.5 - 24.9 | Normal\n");
	printf("25.0 - 29.9 | Sobrepeso\n");
	printf(">=30 | Obesidad\n");
	
	
	
	

	
	return 0;
}
