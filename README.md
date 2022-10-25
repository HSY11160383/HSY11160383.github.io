# HSY11160383.github.io
HI

![image](https://user-images.githubusercontent.com/112918655/196331216-116006c2-e03f-40b1-b275-89fc5d4ff648.png)

week08-1
#include <stdio.h>
int main()
{
    int n;
    scanf("%n", &n);
    int bad=0;
    for(int i=2; i<n; i++){
        if(n%i==0) bad=1;
    }
    if(bad==0)printf("%d 是質數", n);
    else printf("%d 不好, 不是質數", n);
}
計算質數

week08-2
#include <stdio.h>
int main()
{
    int a;
    scanf("%d", &a);
    for(int n=2; n<=a; n++){
        int bad=0;
        for(int i=2; i<n; i++){
            if(n%i==0 ) bad=1;
        }
        if(bad==0) printf("%d ", n);
    }
}
換一種方式寫質數

week08-3
#include <stdio.h>
int main()
{
    printf("請輸入 5個數字(要加起來): ");
    int n;
    int sum=0;
    for(int i=0; i<5; i++){
        scanf("%d", &n);
        sum+= n;
    }
    printf("總和是:%d", sum);
}
計算數字總和

week08-4
#include <stdio.h>
int main()
{
	int n;
	scanf("%d", &n);
	for(int i=1; i<=n; i++){
		for(int k=1; k<=n-i; k++) printf(" ");
		for(int k=1; k<=i; k++) printf("*");
		printf("\n");
	}
}
換一種方式畫三角形(for版本)

week08-5
#include <stdio.h>
int main()
{
	int n;
	scanf("%d", &n);
	for(int i=1; i<=n; i++){
		for(int k=1; k<=n; k++){
			if(k<=n-i)printf(" ");
			else printf("*");
		}
	printf("\n");
	}
}
換一種方式畫三角形(for版本)

week08-6
#include <stdio.h>
int main()
{
	int n;
	scanf("%d", &n);
	int i=1;
	while(i<=n){

		int k=1;
		while(k<=n){
			if(k<=n-i)printf(" ");
			else printf("*");

			k++;
		}
		printf("\n");
		i++;
	}
}
換一種方式畫三角形(while版本)

![image](https://user-images.githubusercontent.com/112918655/197678985-669eaf42-4267-4a97-80e7-63ae8f6616f2.png)
