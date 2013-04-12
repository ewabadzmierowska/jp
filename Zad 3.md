```c
#include <stdio.h>
int main (){
    double a,z=1;
   int n, i;
   printf("Podaj liczbe: ");
   scanf("%lf",&a);
   printf("Podaj wykladnik (liczba naturalna): ");
   scanf("%d",&n);
   for(i=1;i<=n;i++){
   z=z*a;
}
   printf("\n\n Wartosc %lf do potegi %d wynosi %lf ", a, n, z);
   getchar();
   getchar();
   return 0;
       }
```
