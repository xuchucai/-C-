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
