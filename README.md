# MULTIPLOS


#include <stdio.h>
#include <stdlib.h>

int main (void)
{
    int i, multiplos_de_2, multiplos_de_5, n, un_numero;
    multiplos_de_2 = 0;
    multiplos_de_5 = 0;
    printf ("Ingresa el valor de n: ");
    scanf ("%d", &n);
    (void) getchar ();
    for (i=1; i<=n; i++)
    {
        printf ("PROCESO %d\n", i);
        printf ("Ingresa el valor de un numero: ");
        scanf ("%d", &un_numero);
        (void) getchar ();
        if(un_numero%2==0)
            multiplos_de_2=multiplos_de_2+1;
        if(un_numero%5==0)
            multiplos_de_5=multiplos_de_5+1;
        putchar ('\n');
    }
    printf ("Valor de multiplos de 2: %d\n", multiplos_de_2);
    printf ("Valor de multiplos de 5: %d\n", multiplos_de_5);
    system ("pause");
    return EXIT_SUCCESS;
}

