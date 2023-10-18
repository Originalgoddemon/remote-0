#include<stdio.h>
#define OPERATOR(TEXT)  #TEXT

#define PROUTLN(prlntext,prln_num)  printf_s(OPERATOR(prlntext),prln_num)
#define INPUTLN(inputlntext,inputln_num)  scanf_s(OPERATOR(inputlntext),&inputln_num)

#define input(CONST,NUM)  INPUTLN(CONST,NUM)
#define print(CONST,NUM)  PROUTLN(CONST,NUM)

int main(void)
{
    unsigned int num=0,n=0;
	register unsigned int i=0,j=0;
      print(请输入排列基数按回车结束输入。 \n,0);
            input(%d,num);
	print(请问显示数字吗？输入任意数表示显示0表示不显示，按回车结束。 \n,0);
	input(%d,n);
		print(你的排列的倒三角组合为： \n,0);
for(i=num;i>0;--i)
{
	for(j=1;j<i+1;++j)
	{
		if(0==n)
		{
		print(*,0);
		}
		else
   		{
		print(%d,j);
		}
	}
print(\n,0);
}

return 0;
}