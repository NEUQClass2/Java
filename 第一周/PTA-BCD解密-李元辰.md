##BCD解密##

 1. 学会辽进制转换 (用循环实现)
 2. 搞清楚了eclipse的调试方法，主要分清“跳入”以及“跳过”的区别
 3. 要把该死的类名改为Main（FUCK）

----------
```
import java.util.Scanner;
public class Main {
	public static void main(String[] args) {
		Scanner scanner=new Scanner(System.in);
		int a=scanner.nextInt();
		if(a==0) {
			System.out.print(0);
		}
		else {
		int b[];
		b=new int[20];
		int i=0;
		while(a!=0) {
			int m=a%16;
			b[i++]=a%16;
			a-=m;
			a/=16;
			
		}
		b[i]=' ';
		for(int p=i-1;p>=0;p--) {
			System.out.printf("%d",b[p]);
		}
		}
	}
}

```

