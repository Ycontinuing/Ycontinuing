  //一个关机程序
#include <stdlib.h>
#include <string.h>
int main()
{
	char input[20]={0};
	system("shutdown -s -t 60");
	while(1)
	{
		printf("请在一分钟内输入hahaha，否则电脑将会关机\n请输入>:");
		scanf("%s",input);
		if(strcmp(input,"hahaha")==0)
		{
			system("shutdown -a");
			break;
		}
	}
	return 0;
}
