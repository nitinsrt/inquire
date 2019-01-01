#include<stdio.h>
main()
{
	int n,i,q,ar[100000]={0},a,b;
	scanf("%d",&n);
	for(i=0;i<n;i++)
	{
		scanf("%d",&ar[i]);
	}	
	scanf("%d",&q);
	while(q--)
	{
		scanf("%d %d",&a,&b);
		int sum=0;
		a--;
		b--;
		for(i=a;i<=b;i++)
		{
			sum=sum+ar[i];
		}
		printf("%d",sum);
	}
	return 0;
}
