#include<lpc214x.h>
void delay(unsigned int a)
{
unsigned int i,j;
for(i=0;i<=a;i++);
for(j=0;j<=i;j++);
}

int main()
{
PINSEL0 &=0x00FFFFFF;
PINSEL1 &=0xFFFFFF00;
IODIR0 |=0x000FF000;
while(1)
{
IOSET0 |= 0x000FF000;
delay(700000);
IOCLR0 |= 0x000FF000;
delay(700000);
}
}
