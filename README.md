# Data-Maneger-2

#include <stdio.h>
#include <math.h>
#include <string.h>

typedef struct students {
   char name[100];
   char class[100];
   char division[100];
   int rollNo[100];
}s;

typedef struct teachers {
char name[100];
char classTeacher[100];
}t;

typedef struct class {
char Class[100];
char division[100];
int pat[100];
int boys[100];
int girls[100];
}c;

int main(){

s s1;
s1.name[1000];
s1.class[1000];
s1.division[1000];
s1.rollNo[1000];

t t1;
t1.classTeacher[1000];
t1.name[1000];

c c1;
c1.boys[10000];
c1.Class[1000];
c1.division[1000];
c1.girls[10000];
c1.pat[1000];

char sname[100];
char tname[100];

for(int i = 0; i < 1; i++){
   printf("Enter Details of Student %d\n",i +1);
   printf("\n");
   printf("Enter Name : ");
   fgets(sname,100,stdin);

   printf("Enter Class : ");
   scanf("%s",&s1.class[i]);
 
   printf("Enter Division : ");
   scanf("%s",&s1.division[i]);

   printf("Enter Roll No. : ");
   scanf("%d",&s1.rollNo[i]);

   s1.name[i] = sname[i];    
}

for(int i = 0; i < 1; i++){
   printf("Enter Details of Teacher %d\n",i + 1);
   printf("\n");
   printf("Enter Name : ");
   fgets(tname,100,stdin);

   printf("Enter Class of which they are Classteacher : ");
   scanf("%s",&t1.classTeacher[i]);

   t1.name[i] = tname[i];
}

for(int i = 0; i < 1; i++){
   printf("Enter Details of Class  %d\n",i + 1);
  printf("\n");
  printf("Enter Class Name : ");
  scanf("%s",&c1.Class[i]);

  printf("Enter Division : ");
  scanf("%c",&c1.division[i]);

  printf("Enter Total No of Students : ");
  scanf("%d",&c1.pat[i]);

  printf("Enter No of Boys : ");
  scanf("%d",&c1.boys[i]);

  printf("Enter No of Girls : ");
  scanf("%d",&c1.girls[i]);  
}

return 0;

}

