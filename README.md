# Decimal-pra-bin-rio

#include <stdio.h>

int main(int argc, char **argv)
{
    int n;
    int total  = 0;
    int potenc = 1;
    int dec = 0;
    int recebe;

    printf("Leitura do numero binario: ");
    scanf("%d",&n);

    recebe = n;

     while(n > 0)
     {
        total += n % 10 * potenc;
        n = n / 10;
        potenc = potenc * 2;

     }

        dec = total;

        printf("Bin = %d - Dec = %d\n", recebe  , dec);

    return 0;
}

