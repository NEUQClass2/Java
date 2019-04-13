- 第一次接触java，一脸懵
- 只会照猫画虎写，但总之神奇的过了
- 其实和c主要区别就是一个输入输出
```
import java.util.Scanner; 
public class Main{
	public static void main(String[] args) {
		Scanner input=new Scanner(System.in);
        int a=input.nextInt(); // 接收键盘输入数据
        int x=a%16;
        int ans=a/16*10+x;
        System.out.println(ans);
        
	}
}
```
- 去网上查了一下，PTA上提交(可能）都是这种格式，总之先留个底
```
public class Main{
    public static void main(String[] args){
           //其他代码
    }
}
```
# 关于scanner输入
- 程序开头必须```import java.util.Scanner``` 导入Scanner类。
- 使用```Scanner sc = new Scanner(System.in);```生成scanner对象。  
该Scanner对象sc可以处理标准输入。所谓的标准输入，在你的电脑上就是你从键盘通过控制台进行的输入。

参考：https://www.cnblogs.com/zhrb/p/6347738.html?utm_source=itdadao&utm_medium=referral  
（还有很多其他关于scanner的东西，留着以后看）
