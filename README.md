#include<reg51.h>
sbit led=P2^0;
void delay(unsigned int );
void main()
{
	while(1)
	{
		led=1;
		delay(500);
		led=0;
		delay(200);
	}
}
void delay(unsigned int dly)
{
	int i,j;
	for(i=0;i<dly;i++)
	for(j=0;j<1000;j++);
}
