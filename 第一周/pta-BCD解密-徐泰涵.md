# 泰神的作业

标签（空格分隔）： Java代码

---

###**代码：**
`import java.util.Scanner;
  public class Main{
    public static void main(String args[]){
      Scanner reader=new Scanner(System.in);
      int x = reader.nextInt();
      int a = 0;
      int b = 0;
      int c = 0;
      a=x%16;
      b=x/16;
      c=b*10+a;
      System.out.printf("%d",c);
    }
}`
###**心得体会：**
1、学会了Java语言的基本书写格式：
public class{
    public static void main(String args[]){
    ...
    ...
    }
}
2、学会了Java语言的输入：
import java.util.Scanner;
int x = reader.nextInt();
**注：输入类型要相匹配**
3、学会了Java语言的输出格式：
System.out.printf("%d等",变量);
System.out.println（a+"字符串"+b）;
4、学会了基本数据类型的声明。