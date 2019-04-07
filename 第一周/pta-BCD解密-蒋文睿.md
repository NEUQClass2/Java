 
# JAVA菜鸟入门

## BCD解密学习初心得：从C到JAVA

###第一次尝试：
- 先读题，发现题意是要把16进制转化成十进制输出；
-  而且碰到了java这种未接触过的语言
 - 第一反应就是先用c先写出来咯
-  /*#include <stdio.h>

- int main()

- {

 -	int x;

-	int n, a;

-	scanf("%d", &x);

-	a = x % 16;

-	n = x / 16 * 10 + a;

-	printf("%d", n);

-	return 0;

- }*/
- 我试着转换为JAVA的格式：
- /*import java.util.*;
- class Main
- {
- 	void printArea(int x)
- 	{
 -   int n,a;
 -   a=x%16;
 -   n=x/16*10+a;
 -   
-		System.out.println(n);
-	}
- }*/
- 然而交上去却是错的
- 在调试过程中我发现没办法输入十六进制的ABCDEF字符部分
- 就想着用字符串输入试试
##  2000years later

- 在看了网上的代码和书以后，同时发现函数十六进制（HEX）转十进制的函数也是基于字符串
- 不过由于输入的问题
- 就照着网上的来了：
- import java.util.*;
- public class Main {
-	public static void main(String[] args) {
-		Scanner in=new Scanner(System.in);
-		int n=in.nextInt();
-		System.out.println(Integer.toHexString(n));
-	}
- }
- 完美通过
-  不过我又做了以下两组实验：
- 将Scanner in=new Scanner(System.in);
-		int n=in.nextInt();
- 这两句删除
- 还是发现输不入英文
- 所以单用字符串还是不行
- 查询了这两句的作用，发现其作用是读取输入信息，不过还是没有发现有其他必要的意义，希望我在今后的学习中可以弄明白原理究竟是为何；