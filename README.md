// Proyecto
//primera parte
#include "stdio.h"
#include "stdlib.h"
#define MAXIMO 10
#define SALTO printf ("\n")

void main() {
	double x, R, coefi[MAXIMO];
	long li;
	char a[15], * p;
	int j;

	a[0] = 13;
	printf("Por favor, informe el grado del polinomio..\n");
	cgets(a);
	li = strtol(a + 2, &p, 10);
	while (*p != '\0' || li < -32768L || li > 32767L) {
		printf("%c", 7);  		/* Aviso de error */
		printf("Cifra incorrecta. Favor rectifique...\n");
		cgets(a);
		li = strtol(a + 2, &p, 10);
	}
