```c
#include <stdio.h>
#include <math.h>
double pierwiastek (double a){
       double x=1, eps=1e-15;
       do {
           x=(x+a/x)/2;
           } while (fabs(x-a/x)>eps*x);
           return x;
           }
           int main(){
               double z;
               for (z=1e-5;z<=1e5; z=z*10){
                   printf("pierw(%lf)=%.15lf\n",z,pierwiastek(z));
                   printf(" sqrt(%lf)=%.15lf\t",z,sqrt(z));
                   printf("blad wzgledny=%e\n",(pierwiastek(z)-sqrt(z))/sqrt(z));
                   }
                   getchar();
                   getchar();
                   return 0;
                   }
```
