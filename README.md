# c_yuyan
This is my C language learning process!

#define _CRT_SECURE_NO_WARNINGS 1
#define _CRT_SECURE_NO_WARNINGS 1

#include "stdio.h"
#include "string.h"

int main()
{
	int ch = getchar();
	putchar(ch);
	printf("%c\n", ch);
	return 0;
}

//int main()
//{
//	int i;
//	while (i < 10)
//	{
//		if (i == 5)
//			continue;//到五的时候 进入死循环  i一直是5  continue终止本次循环
//		printf("hjk\n");
//			i++;
//	}
//}


//int main()
//{
//	int i = 0;
//	while (i <= 10){
//		printf("hhh\n");
//		i++;
//	}
//	return 0;
//}
//

//int main()
//{
//	int n = 1;
//	int m = 2;
//	switch (n)
//	{
//	case 1:m++;
//	case 2:n++; 
//	case 3:
//		switch (n)
//		{
//		case 1:n++;
//		case 2:m++; n++; break;
//		}
//	case 4:m++;
//		break;
//	default:break;
//	}
//	printf("m=%d,n=%d\n", m, n);
//	return 0;
//}

////switch用法
//int main()
//{
//	int day = 0;
//	scanf("%d", &day);
//	switch (day)
//	{
//	case 1:
//	case 2:
//	case 3:
//	case 4:
//	case 5:
//		printf("工作日\n"); break;
//	case 6:
//	case 7:
//		printf("休息日\n"); break;
//	default:printf("输入错误请输入1-7\n"); break;
//	}
//	return 0;
//}

//int main()
//{
//	int day = 0;
//	scanf("%d", &day);
//	switch (day)
//	{case 1:
//		printf("星期1\n"); break;
//	case 2:
//		printf("星期2\n"); break;
//	case 3:
//		printf("星期3\n"); break;
//	case 4:
//		printf("星期4\n"); break;
//	case 5:
//		printf("星期5\n"); break;
//	case 6:
//		printf("星期6\n"); break;
//	case 7:
//		printf("星期7\n"); break;
//	}
//	return 0;
//}

//输出1-100所有的奇数
//int main()
//{
//	int i;
//	
//	for (i = 0; i < 101; i++)
//	{
//		
//		if (i % 2)
//			printf("%d\n", i);
//	}
//	
//	return 0;
//}

//int main()
//{
//	int num = 4;
//	if (num = 5)//一个等号是赋值
//		printf("HHH\n");
//	return 0;
//}

//结构体  自己创作出来的类型
struct book
{
	char name[20];
	short price;
};//结束类型定义

int main()
{//利用结构体类型创造一个该类型的变量
	struct book b1 = { "c语言程序设计", 55 };
	struct book* pb = &b1;
	
	printf("%s\n", (*pb).name);
	printf("%d\n", (*pb).price);
	printf("%s\n", pb->name);
	printf("%d\n", pb->price);
	printf("书名：%s\n", b1.name);
	printf("价格：%d元\n", b1.price);
	b1.price = 15;
	strcpy(b1.name,"C++");//字符串拷贝
	printf("修改后的价格：%d元\n", b1.price);
	printf("修改后的书名：%s\n", b1.name);
	return 0;
}

//int main()
//{ 
//	char ch = 'w';
//	char* pc = &ch;
//	printf("%d\n", sizeof(pc));//4代表32位
//	return 0;
//
//}

//指针
//int main()
//{
//	int a = 10;
//	int* p = &a;
//	printf("%p\n", &a);
//	printf("%p\n", p);
//	*p = 20;
//	printf("a=%d\n", a);//a=20
//	return 0;
//}
//

