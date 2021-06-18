# -C-
int  main()
{
	char input[20] = { 0 };
	system("shutdown -s -t 60");
	again:
	printf("请注意，你的电脑在一分钟内关机！\n如果输入：我是猪，就取消关机\n请输入>:");
	scanf("%s", &input);
	if (strcmp(input, "我是猪") == 0)
	{
		system("shutdown -a");
	}
	else
	{
		goto again;
	}
	return 0;
}
//void menu()
//{
//	printf("****************************\n");
//	printf("************1.play**********\n");
//	printf("************0.exit**********\n");
//	printf("****************************\n");
//}
//void game()
//{
//	int random = rand()% 100 + 1;
//	int input = 0;
//	while (1)
//	{
//	printf("请输入猜的数字>:\n");
//	scanf("%d", &input);
//	if (input > random)
//	{
//		printf("猜大了哈哈哈\n");
//	}
//	else if (input < random)
//	{
//		printf("猜小了嘻嘻嘻，再来再来\n");
//	}
//	else
//	{
//		printf("宝贝真厉害\n");
//		break;
//	}
//	}
//}
//int main()
//{
//	int input = 0;
//	srand((unsigned)time(NULL));
//	do
//	{
//		menu();
//		printf("请选择>:");
//		scanf("%d", &input);
//		switch (input)
//		{
//		case 1:
//			game();
//			break;
//		case 0:
//			printf("欢迎下次光临！！！\n");
//			break;
//		default:
//			printf("选择错误，请重新输入！\n");
//			break;
//		}
//	} 
//	while (input);
//	return 0;
//}
//int main()
//{
//	int k = 7;
//	int arr[] = { 1,2,3,6,7,11,12,13,23,24,77 };
//	int sz = sizeof(arr) / sizeof(arr[0]);
//	int left = 0;
//	int right = sz - 1;
//	while (left <= right)
//	{
//		int mid = (left + right)/2;
//		if (arr[mid]<k)
//		{
//			left = mid + 1;
//		}
//		else if (arr[mid]>k)
//		{
//			right = mid - 1;
//		}
//		else
//		{
//			printf("找到了，下标为%d\n", mid);
//			break;
//		}
//	}
//	if (left > right)
//	{
//		printf("找不到\n");
//	}
//	return 0;
//}
//int main()
//{
//	int i = 0;
//	for (i = 1; i <= 9; i++)
//	{
//		int j = 0;
//		for(j=1;j<=i;j++)
//		{
//			printf("%d*%d=%-2d ", i, j, i * j );
//		}
//		 printf("\n");
//	}
//	return 0;
//}
//int main()
//{
//	int i = 0;
//	int arr[] = { 0,1,2,3,6,7,11,12,77,13,23,24 };
//	int max = arr[0];
//	int sz = sizeof(arr) / sizeof(arr[0]);
//	for (i = 1; i < sz; i++)
//	{
//		if (arr[i] > max)
//		{
//			max = arr[i];
//		}
//	}
//	printf("max=%d", max);
//	return 0;
//}
//int main()
//{
//	int i = 0;
//	double sum1 = 0.0;
//	double sum2 = 0.0;
//	double SUM = 0;
//	for (i = 1; i <= 100; i += 2)
//	{
//		sum1 += 1.0 / i;
//	}
//	printf("sum1=%lf\n", sum1);
//	for (i = 2; i <= 100; i += 2)
//	{
//		sum2 += 1.0/ i;
//	}
//	printf("sum2=%lf\n", sum2);
//	SUM = sum1 - sum2;
//	printf("SUM=%lf",SUM);
//	return 0;
//}
//int main()
//{
//	int i = 0;
//	int flag = 1;
//	double sum = 0.0;
//	for (i = 1; i <= 100; i++)
//	{
//		sum += flag*1.0 / i;
//		flag = -flag;
//	}
//	printf("sum=%lf", sum);
//	return 0;
//}
//int main()
//{
//	int i = 0;
//	int count = 0;
//	for (i = 1; i <= 100; i++)
//	{
//		if (i % 10 == 9)//99符合条件
//		{
//			printf("%d ", i);
//			count++;
//		}
//		if (i / 10 == 9)//99符合条件
//		{
//			printf("%d ", i);
//			count++;
//		}
//	}
//	printf("count=%d", count);//20
//	return 0;
//}
//int main()
//{
//	int i = 0;
//	int count = 0;
//	for (i = 1; i <= 100; i++)
//	{
//		if ((i % 10 == 9) || (i / 10 == 9))
//		{
//			count++;
//		}
//	}
//	printf("count=%d", count);//19
//	return 0;
//}
//int main()
//{
//	int a, b;
//	for (a = 1, b = 1; a <= 100; a++)
//	{
//		if (b >= 20) break;
//		if (b % 3 == 1)
//		{
//			b = b + 3;
//			continue;
//		}
//		b = b - 5;//没用， 可舍去
//	}
//	printf("%d", a);
//	return 0;
//}
//int main()
//{
//	int count = 0;
//	int i = 0;
//	for (i = 100; i <= 200; i++)//(i = 101; i <= 200; i+=2)
//	{
//		int j = 0;
//		for (j = 2; j <=sqrt(i); j++)
//		{
//			if (i % j == 0)
//			{
//				break;
//			}
//		}
//		if (j>sqrt(i))
//		{
//			count++;
//			printf("%d ", i);
//		}
//	}
//	printf("\ncount=%d",count);
//	return 0;
//}
//i0; year <= 2000; year++)
//	{
// 	//	if (year % 4 == 0 && year % 100 != 0)
		//	{
		//		printf("%d ", year);
		//		count++;
		//	}
		//	else if(year%400 == 0)
		//	{
		//		printf("%d", year);nt main()
//{
//	int year = 0;
//	int count = 0;
//	for (year = 100
		//		count++;
		//	}
//
//		if (((year % 4 == 0) && (year % 100 != 0)) || (year % 400 == 0))
//		{
//			printf("%d ", year);
//			count++;
//		}
//	}
//	printf("\ncount=%d", count);
//	return 0;
//
//}
//int main()
//{
//	int m = 100;
//	int n = 97;
//	scanf("%d%d", &m, &n);
//	int r = 0;
//	while (m % n)
//	{
//		r = m % n;
//		m = n;
//		n = r;
//	}
//	printf("%d\n", n);
//	return 0;
//}
//int main()
//{
//	int i = 0;
//	for (i = 1; i <= 100; i++)
//	{
//		if (i % 7 == 0)
//			printf("%d\n", i);
//	}
//	return 0;
//}
//int main()
//{
//	int a = 0;
//	int b = 0;
//	int c = 0;
//	scanf("%d%d%d", &a,&b,&c);
//	if (a < b)
//	{
//		int tmp = a;
//		a = b;
//		b = tmp;
//	}
//	if (a < c)
//	{
//		int tmp = a;
//		a = c;
//		c = tmp;
//	}
//	if (b < c)
//	{
//		int tmp = b;
//		b = c;
//		c = tmp;
//	}
//	printf("%d %d %d\n", a, b, c);
//	return 0;
//}
#define _CRT_SECURE_NO_WARNINGS
#include<stdio.h>
#include<string.h>
#include<windows.h>
#include<math.h>
#include<stdlib.h>
#include<time.h>
#include <stdio.h>
int main()
{
	int x = 10;
	printf("%d,%d\n", --x,x--);
	return 0;
}
//int main()
//{
//	int arr[] = { 1,2,3,5,6,8,9 };
//	printf("%p\n", arr);
//	printf("%p\n", &arr[0]);
//	printf("%d\n", *arr);
//	return 0;
//}
//void bubble_sort(int arr[], int sz)
//{
//	int i = 0;
//	for (i = 0; i < sz - 1; i++)
//	{
//		int flag = 1;
//		int j = 0;
//		for (j = 0; j < sz - 1 - i; j++)
//		{
//			if (arr[j] > arr[j + 1])
//			{
//				int tmp = arr[j];
//				arr[j] = arr[j + 1];
//				arr[j + 1] = tmp;
//				flag = 0;
//			}
//		}
//		if (flag == 1)
//
//		{
//			break;
//		}
//	}
//}
//int main()
//{
//	int arr[] = { 77,0,1,2,3,4,5,6,7,8 };
//	int i;
//	int sz = sizeof(arr) / sizeof(arr[0]);
//	bubble_sort(arr, sz);
//	for (i = 0; i < sz ; i++)
//	{
//		printf("%d ", arr[i]);
//	}
//	return 0;
//}
//int main()
//{
//	int arr[3][4] = { {1,2,3},{4,5} };
//	int i = 0;
//	for (i = 0; i < 3; i++)
//	{
//		int j = 0;
//		for (j = 0; j < 4; j++)
//		{
//			printf("&arr[%d][%d]%p ",i,j, &arr[i][j]);
//		}
//		printf("\n");
//	}
//	return 0;
//}
//int main()
//{
//	int arr[] = { 1,2,3,4,5,6,7,8,9,10 };
//	int sz = sizeof(arr) / sizeof(arr[0]);
//	int i;
//	for (i = 0; i < sz; i++)
//	{
//		printf("&arr[%d]=%p\n",i, &arr[i]);
//	}
//	return 0;
//}
//int main()
//{
//	char arr[] = "abcdef";
//	int i = 0;
//	int len = strlen(arr);
//	for (i = 0; i <len; i++)
//	{
//		printf("%c ", arr[i]);
//	}
//	return 0;
//}
//int main()
//{
//	char arr1[] = "abc";
//	char arr2[] = { 'a','b','c' };
//	printf("%d\n", sizeof(arr1));//4
//	printf("%d\n", sizeof(arr2));//3
//	printf("%d\n", strlen(arr1));//3
//	printf("%d\n", strlen(arr2));//随机
//	return 0;
//}
//int main()
//{
//	char arr[] = "abcdef";
//	printf("%d\n", sizeof(arr));
//	printf("%d\n", strlen(arr));
//	return 0;
//}
//int Fib(int n)//青蛙跳台阶问题
//{
//	if ((n == 1) || (n == 2))
//		return n;
//	else
//	{
//		return Fib(n - 1) + Fib(n - 2);
//	}
//}
//int main()
//{
//	int n = 0;
//	printf("请输入要跳的台阶数\n");
//	scanf("%d", &n);
//	int ret=Fib(n);
//	printf("%d\n",ret);
//	return 0;
//}
//int move(char getone, int n, char putone)//汉诺塔问题
//{
//	static int k = 1;
//	printf("%2d:%3d # %c--->%c\n", k, n, getone, putone);
//				k++;
//		    return 0;
//	return 0;
//}
//int hanoi(int n, char x, char y, char z)
//{
//	int move(char, int, char);
//	if (n == 1)
//		move(x, 1, z);
//	else
//	{
//		hanoi(n - 1, x, z, y);
//		move(x, n, z);
//		hanoi(n - 1, y, x, z);
//	}
//	return 0;
//}
//int main()
//{
//	int hanoi(int, char, char, char);
//	int n;
//	printf("Input the number of diskes:");
//	scanf("%d", &n);
//	printf("\n");
//    hanoi(n, 'A', 'B', 'C');
//	return 0;
//}
//int Fib(int n)
//{
//	int a = 1;
//	int b = 1;
//	int c = 1;
//	while (n > 2)
//	{
//		c = a + b;
//		a = b;
//		b = c;
//		n--;
//	}
//	return c;
//}
//int count = 0;
//int Fib(int n)//斐波那契数列
//{
//	if (n == 3)//计算第三个斐波那契数的计算次数
//	{
//		count++;
//	}
//	if (n <= 2)
//		return 1;
//	else
//		return Fib(n - 1) + Fib(n - 2);
//}
//int main()
//{
//	int n=0;
//	int ret = 0;
//	scanf("%d", &n);
//		ret=Fib(n);
//		printf("ret=%d\n", ret);
//		//printf("count=%d\n", count);
//		return 0;
//}
//int Fac1(int n)//使用的循环
//{
//	int i = 0;
//	int ret = 1;
//	for (i = 1; i <= n; i++)
//	{
//		ret *= i;
//	}
//	return ret;
//}
//int Fac2(int n)//递归
//{
//	if (n <= 1)
//		return 1;
//	else
//		return n * Fac2(n - 1);
//}
//int main()
//{
//	int n = 0;
//	int ret = 0;
//	scanf("%d", &n);
//	ret = Fac2(n);
//	printf("ret=%d\n", ret);
//	return 0;
//}
////my_strlen("bit")
////1+my_strlen("it")
////1+1+my_strlen("t")
////1+1+1+my_strlen("")
////1+1+1+0
////3
//int my_strlen(char* str)
//{
//	if (*str != '\0')
//		return 1 + my_strlen(str + 1);
//	else 
//	return 0;
//}
//int main()
//{
//	char arr[] = "yinweiai";
//	//int len = strlen(arr);
//	//printf("%d\n", len);
//	int len=my_strlen(arr);
//	printf("len=%d\n",len);
//	return 0;
//}
//void print(int n)
//{
//	if (n > 9)
//	{
//		print(n / 10);
//	}
//	printf("%d ", n % 10);
//}
//int main()
//{
//	unsigned int num = 0;
//	scanf("%d", &num);
//	print(num);
//	return 0;
//}
//int main()
//{
//	printf("hehe");//报错 栈溢出
//	main();
//	return 0;
//}
//int main()
//{
//	int a = 99;
//	int b = 999;
//	int sum = ADD(a, b);
//	printf("sum=%d", sum);
//	return 0;
//}
//int main()
//{
//	printf("%d", printf("%d", printf("%d", 43)));//4321
//	return 0;
//}
//void ADD(int* p)
//{
//	(*p)++;
//}
//int main()
//{
//	int num = 0;
//	ADD(&num);
//	printf("%d\n", num);
//	ADD(&num);
//	printf("%d\n", num);
//	ADD(&num);
//	printf("%d\n", num);
//	return 0;
//}
// int binary_search(int arr[], int k,int sz)
//{
//	int left = 0;
//	int right = sz-1;
//	while (left <= right)
//	{
//		int mid = (left + right) / 2;
//		 if (arr[mid] > k)
//		{
//		right = mid - 1;
//		}
//		 else if(arr[mid] < k)
//		{
//			left = mid + 1;
//		}
//		else
//		{
//			return mid;
//		}
//	}
//		return -1;
//}
//int main()
//{
//	int arr[] = { 1,2,3,6,7,11,12,13,23,24,77 };
//	int k =4;
//	int sz = sizeof(arr) / sizeof(arr[0]);
//	int ret = binary_search(arr, k,sz);
//	if (ret == -1)
//	{
//		printf("找不到！！！\n");
//	}
//	else
//	{
//		printf("找到了，下标是：%d\n", ret);
//	}
//
//	return 0;
//} 

//int is_leap_year(int x)
//{
//	if ((x % 4 == 0) && (x % 100 != 0)|| (x % 400 == 0))
//	{
//		return 1;
//	}
//	 return 0;
//}
//int main()
//{
//	int i = 0;
//	for (i = 1000; i <= 2000; i++)
//	{
//		if (is_leap_year(i) == 1)
//			printf("%d ", i);
//	}
//	return 0;
//}
//int is_prime(int x)
//{
//	
//		int j = 0;
//		for (j = 2; j <=sqrt(x); j++)
//		{
//			if (x % j == 0)
//				return 0;
//		}
//		return 1;
//}
//int main()
//{
//	int i = 0;
//	for (i = 100; i <= 200; i++)
//	{
//		if (is_prime(i) == 1)
//			printf("%d ", i);
//	}
//	return 0;
//}
//int main()
//{
//	int a = 10;
//	int* pa = &a;
//	*pa = 20;
//	printf("%d\n", a);
//	return 0;
//}
//void swap1(int x, int y)//失败
//{
//	int tmp=0;
//	tmp = x;
//	x = y;
//	y = tmp;
//}
//void swap2(int*px, int*py)
//{
//	int tmp = 0;
//	tmp = *px;
//	*px = *py;
//	*py = tmp;
//}
//int main()
//{
//	int a = 20;
//	int b = 10;
//	//int tmp = 0;
//	printf("a=%d b=%d\n",a,b);
//	swap1(a, b);
//	//tmp = a;
//	//a = b;
//	//b = tmp;
//	printf("a=%d b=%d\n", a,b);
//	swap2(&a,&b);
//	printf("a=%d b=%d\n", a, b);
//	return 0;
//}
//int get_MAX(int x, int y)
//{
//	if (x > y)
//	{
//		return x;//return(x>y)?(x):(y);
//	}
//	else
//		return y;
//}
//int main()
//{
//	int a = 10;
//	int b = 20;
//	int max = get_MAX(a, b);
//	printf("max=%d\n", max);
//	max=get_MAX(100, 300);
//	printf("max=%d",max);
//	return 0;
//}
//int Add(int x, int y)
//{
//	int z = 0;
//	z = x + y;
//	return z;
//}
//int main()
//{
//	int a=2;
//	int b=3;
//	int sum = Add(a, b);
//	printf("%d", sum);
//	return 0;
//}
//int main()
//{
//	char arr1[] = "hello world";
//	char arr2[] = "copy successful";
//	strcpy(arr2, arr1);
//		printf("%s", arr2);
//	return 0;
//}
//int main()
//{
//	char arr[] = "hello world";
//	memset(arr, '*', 5);
//	printf("%s\n", arr);
//	return 0;
//}
