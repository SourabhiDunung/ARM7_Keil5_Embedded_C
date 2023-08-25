#include<lpc214x.h>
void delay(unsigned int a)
{
unsigned int i,j;
for(i=0;i<=a;i++){
for(j=0;j<=i;j++);
}
}

int main()
{
PINSEL0 &=0x00FFFFFF;
PINSEL1 &=0xFFFFFF00;
IODIR0 |=0x000FF000;
while(1)
{
unsigned int x,y;
IOSET0 |= 0x00080000;

for(y=0;y<=7;y++){
x=IOSET0;
IOSET0=x>>1;
delay(4000);
}
IOCLR0 |= 0x000FF000;
delay(4000);
}
}
