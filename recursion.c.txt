#include<stdio.h>
#include<conio.h>
int fact(int);
main()
{
int n,f;
//program to find factorial by recursion
printf("Enter any number");//enter any number whose factorial you want to find.
scanf("%d",&n);
//calling our user defined function
f= fact(n);
printf("factorial is %d",f); //displaying factorial of input number
getch();
}
 int fact(int n)
{
 if(n==0)
  return(1);
  else
  //function calling itself: recursion
  return(n*fact(n-1));
 }

