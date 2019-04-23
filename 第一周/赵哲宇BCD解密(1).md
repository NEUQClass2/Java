# zzy的BCD解密作业
### 题目：*基础编程题目集*  **7-4 BCD解密**

* **题目描述**  
BCD数是用一个字节来表达两位十进制的数，每四个比特表示一位。所以如果一个BCD数的十六进制是0x12，它表达的就是十进制的12。但是小明没学过BCD，把所有的BCD数都当作二进制数转换成十进制输出了。于是BCD的0x12被输出成了十进制的18了！
现在，你的程序要读入这个错误的十进制数，然后输出正确的十进制数。提示：你可以把18转换回0x12，然后再转换回12。
 * **输入样例**  
  18
  * **输出样例**  
  12


```java
import java.util.Scanner;//导入（import）java.util包下的Scanner类
public class Main {   //主类

	public static void main(String[] args) {  //java应用程序必须有一个类含有此条语句,这个类称为应用函数的主类
		                 //args 是main的参数，是一个字符类型的数组,使得程序能接受用户从键盘输入的字符串，java的运行程序总是从主类的main方法开始执行                    
		   //需要先进入字节码所在的目录，当文件具有多个类是执行的必须是主类的名字，运行时java虚拟机将字节码加载到内存里，然后解释执行
        
		Scanner reader=new Scanner(System.in);//赋值号左边声明一个Scanner类型的变量reader
		  //赋值号右边 new Scanner()是一个构造函数返回一个scanner类型的对象，System（系统类）.in(流变量，静态变量，可以直接通过system类调用）
		//控制台会一直等待输入，直到敲回车后，把输入内容传给Scanner
		int x=reader.nextInt();//??将reader类型的int型变量赋值给x
		int m=x/16;
		int n=x%16;
		int y=m*10+n;
		System.out.println(y);//System(系统类），out（静态数据成员），而out有是java.io.PrintStream类里的一个方法，println用来输出控制台信息
	}

}
```