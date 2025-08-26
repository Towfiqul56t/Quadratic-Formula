#include <stdio.h>
#include <math.h>
int main() {
    
double a, b, c;
double  r1,r2,x,y,z;

printf("Entar value of a: ");
scanf("%lf",&a);
printf("Entar value of b: ");
scanf("%lf",&b);
printf("Entar value of c: ");
scanf("%lf",&c);

x = b*b - 4*a*c;

if(x>0){
  r1 = (-b + sqrt(x))/(2*a);
  r2 = (-b - sqrt(x))/(2*a);
  printf("root1 %.3lf\n root2 %.3lf", r1,r2);
}
else if(x==0){
  r1=r2= -b/(2*a);
   printf("root1 %.3lf\n root2 %.3lf", r1,r2);
}
else{
  y = -b/(2*a);
  z = sqrt(x)/(2*a);
   printf("root1 %.2lf + %.2lfi\n root2 %.2lf - %.2lfi ", y, z);
}
   
}
