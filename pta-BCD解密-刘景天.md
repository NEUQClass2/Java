# 7-4 BCD解密 （10 分)
BCD数是用一个字节来表达两位十进制的数，每四个比特表示一位。所以如果一个BCD数的十六进制是0x12，它表达的就是十进制的12。但是小明没学过BCD，把所有的BCD数都当作二进制数转换成十进制输出了。于是BCD的0x12被输出成了十进制的18了！

现在，你的程序要读入这个错误的十进制数，然后输出正确的十进制数。提示：你可以把18转换回0x12，然后再转换回12。
### 输入格式：
输入在一行中给出一个[0, 153]范围内的正整数，保证能转换回有效的BCD数，也就是说这个整数转换成十六进制时不会出现A-F的数字。
### 输出格式：
输出对应的十进制数。
### 输入样例：
```
18
```
### 输出样例：
```
12
```
## AC代码
```java
import java.util.*;
class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        Integer a = sc.nextInt();
        System.out.println(Integer.toHexString(a));
    }
}
```
## 感想
hhh去年王和兴的作业题，直接把输入以16进制输出就好了
## 知识点
Integer类提供的进制转换方法
|方法|参数解释|返回值|
|-|-|-|
|Integer.toBinaryString(n);|n是int或Integer数|把n转为2进制的字符串|
|Integer.toOctalString(n);|n是int或Integer数|把n转为8进制的字符串|
|Integer.toHexString(n);|n是int或Integer数|把n转为16进制的字符串|
|Integer.toString(n, d);|n是int或Integer数，d是底数|把n转换为d进制后的字符串|