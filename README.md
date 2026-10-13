# Raise-to-the-power-by-recrsive-logarithmic-
#include<stdio.h>
#include<stdlib.h>
int recpow (int x , int y){
     if (y==0) {return 1;}
     int a = recpow(x,y/2);
     if (y%2 == 0) return a*a;
     if (y%2 != 0) return a*a*x;
}
int main()
{
    int a , b;
    printf("enter value of base & power \n");
    scanf("%d %d",&a ,&b);
     int c = recpow( a , b);
     printf(" %d raise to the power %d is %d ",a,b,c);
    return 0;
}