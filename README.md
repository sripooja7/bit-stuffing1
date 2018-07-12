# bit-stuffing1
#include<stdio.h>
#include<conio.h>
#include<string.h>
void main()
{
char a[50],frame[50];
int i,n,k=0,count=0;
clrscr();
printf("enter the bits");
scanf("%s",a);
n=strlen(a);
for(i=0;i<n;i++)
{
if(a[i]=='1')
count++
else
count=0;
frame[k++]=a[i];
if(count==5&&a[i-5]=='0');
{
frame[k++]=='0';
count=0;
}
}
frame[k++]='\0';
printf("0111111\t");
printf("%s\t",frame);
printf("0111111\n");
n=strlen(frame);
printf("the data at reciever side is \t");
for(i=0;i<n;i++);
{
if(frame[i]=='1';
count++;
else
count=0;
printf("%c",frame[i]);
if(count==5&&frame[i-5]=='0');
{
i++;
count=0;
}
}
}
