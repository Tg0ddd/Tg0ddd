# include <stdio.h>
# include <stdlib.h>
# include <conio.h>
# include <math.h>
void niilber_too(void )
{
   double a, b, c = 0;
    printf("\nEne 2 toog oruulna \nEhnii too : ");
    scanf("%lf", &a);
    printf("2 too: ");
    scanf("%lf", &b);
    c = a + b;
    printf("\n%.4lf + %.4lf = %.4lf\n", a, b, c);
}
void yalgawar_too( void )
{
    double a, b, c = 0;
    printf("\nEne 2 toog oruulna \nEhnii too : ");
    scanf("%lf", &a);
    printf("2 too: ");
    scanf("%lf", &b);
    c = a - b;
    printf("\n%.4lf - %.4lf = %.4lf\n", a, b, c);
}
void urjwer_too(void ){
 double a, b, c = 0;
    printf("\nEne 2 toog oruulna \nEhnii too : ");
    scanf("%lf", &a);
    printf("2 too: ");
    scanf("%lf", &b);
    c = a * b;
    printf("\n%.4lf * %.4lf = %.4lf\n", a, b, c);
}
void noogdwor_too( void ){
 double a, b, c = 0;
    printf("\nEne 2 toog oruulna \nEhnii too : ");
    scanf("%lf", &a);
    printf("2 too: ");
    scanf("%lf", &b);
    c = a / b;
    printf("\n%.4lf / %.4lf = %.4lf\n", a, b, c);
}
void pactoral_too(void){
  int i,n,pac=1,count=1;
     void clrscr();
     printf("\n N=");
     scanf("%i", &n);
     for(i=n;i>=0;i--){      
     if(i==1) continue;
     if(i==0) continue;
     pac=pac*i;
 }
   printf("%d iin Pactaral=%d", n, pac);
}
void yazguur_too(void){
 int n, pac;
 printf("\nN=");
     scanf("%i", &n);
     pac=sqrt(n);
   printf("%d", pac);
}
void zereg_too(void){
  int n,m, pac;
   printf("\nN=");
     scanf("%i", &n);
     printf("zereg ni=");
     scanf("%d", &m);
     pac=pow(n,m);
   printf("Hariu=%d", pac);
}
void log_too(void){
  double n, pac;
   printf("\nN=");
     scanf("%lf", &n);
     pac=log(n);
   printf("%.4lf", pac);
}
#include<stdio.h>
#include<conio.h>
#include<math.h>
#include<stdlib.h>
#define KEY "Ta uuriin songoltoo oruul nuu?:"
// Function prototype declaration
void addition();
void subtraction();
void multiplication();
void division();
void modulus();
void power();
int factorial();
void calculator_operations();
// Start of Main Program
int main()
{
    int X=1;
    char Calc_oprn;
    // Function call
    calculator_operations();
    while(X)
    {
        printf("\n");
        printf("%s : ", KEY);
        Calc_oprn=getche();
        switch(Calc_oprn)
        {
            case '+': niilber_too();
                      break;
            case '-': yalgawar_too();
                      break;
            case '*': urjwer_too();
                      break;
            case '/': noogdwor_too();
                      break;
            case '?': yazguur_too();
                      break;
            case '!': pactoral_too();
                      break;
            case '^': zereg_too();
                      break;
            case '#': log_too();
    break;
            case 'H':
            case 'h': calculator_operations();
                      break;
            case 'Q':
            case 'q': exit(0);
                      break;
            default : system("cls");
                      calculator_operations();
        }
    }
}
//Function Definitions
void calculator_operations()
{
    //system("cls");  use system function to clear
    //screen instead of clrscr();
    printf("\nEnhuu tooni  mashin 2 ba 1 toon dr yawagdag\n\n");
    printf("Enter + symbol for Niilber \n");
    printf("Enter - symbol for yalgawar \n");
    printf("Enter * symbol for urjwer \n\n");
    printf("Enter / symbol for noogdwor \n");
    printf("Enter ? symbol for yazguur\n");
    printf("Enter ^ symbol for zereg \n\n");
    printf("Enter ! symbol for Factoral \n");
    printf("Enter # symbol for log10\n");
}
