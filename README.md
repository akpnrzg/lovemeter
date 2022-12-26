/*# lovemeter
lovemeter/*
#include <stdio.h>
#include <stdlib.h>
#include<string.h>
int main(){
char name1[10],name2[10];
int love;
printf("Enter your name: ");
scanf("%s",&name1);
printf("Enter your lover's name: ");
scanf("%s",&name2);
love=strlen(name1)+strlen(name2);
if(strlen(name1)>strlen(name2))
{
love-=5;
}
else
{
love+=3;
}
love*=52;
love=love/(2+strlen(name2));
printf("\n\nThe love percent for %s and %s equals %d\n",name1,name2,love);
}
