#include<stdio.h>
int main()
{
	int num,count,c9,c89,c78,c67,c6;
	float sum=0.0,avg=0.0;
	num=count=c9=c89=c78=c67=c6=0;
	
	scanf("%d",&num);
	while(num>0 && num<101)
	{
		sum += num;
		count+= 1;
		if(num>=90)
		  c9=c9+1;
		else
			{
				if(num>=80&&num<90)
				c89 += 1;
				else
				{
					if(num>=70&&num<80)
					c78+= 1;
					else
					{
						if(num>=60&&num<70)
						c67 =c67+ 1;
							else 
							c6+= 1;
					}
				
				}
				
			}
	 
		scanf("%d",&num);
	} 
		avg = sum/count;
		printf("90分以上%d\n",c9);
		printf("八十到九十%d\n",c89);
		printf("七十到八十%d\n",c78);
		printf("六十到七十%d\n",c67);
		printf("六十以下%d\n",c6);
		printf("平均数%f\n",avg);
		printf("总和%f\n",sum);
	 return 0;
}
 
