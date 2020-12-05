<h1>复习题</h1>
<p>1.C++程序的模块叫什么？</p>
<p>函数</p>
<p>2.下面的预处理器编译指令是做什么用的？</p>
<p>#include <iostream></p>
<p>在最终编译前，将iostream中地内容替换为预处理指令</p>
<p>3.下面的语句是做什么用的？</p>
<p>using namespace std;</p>
<p>它使得程序可以使用std命名空间中的定义</p>
<p>4.什么语句可以用来打印短语"Hello,world",然后开始新的一行？</p>
<p>cout<<"Hello,world";或cout<<"Hello,world"<<endl;</p>
<p>5.什么语句可以用来创建名为cheeses的整数变量？</p>
<p>使用int可以创建一个名为cheeses的整数变量</p>
<p>6.什么语句可以用来将值32赋给变量cheeses？</p>
<p>使用=（赋值运算符），将值32放在变量声明右边 如:int cheeses=32;</p>
<p>7.什么语句可以用来将从键盘输入的值读入变量cheese中？</p>
<p>cin>>cheese</p>
<p>8.什么语句可以用来打印"We have X varieites of cheese",其中X为变量cheese</[]>
<p>cout<<"We have"<<cheese<<" varieites of cheese";</p>
<p>9.下面的函数原型指出了关于函数的哪些信息？</p>
<p>int froop(double t);</p>
<p>函数froop返回一个整数值，并接收一个double类型的参数</p>
void rattle(int n);
函数rattle不返回函数返回值，它接收一个int类型的参数
int prune(void);
函数prune返回一个整数值，它不接收任何参数
10.定义函数时，在什么情况下不必使用关键字return？
在定义函数原型时，如果将原型返回值声明为void或者函数不接受任何参数时不必使用关键字return
###编程练习
1.编写一个C++程序，它显示您的姓名和地址。
#include <iostream>
using namespace std;
int main()
{
    cout<<"Name:Toin"<<endl<<"Address：beijing"
    <<endl;
    return 0;
}
2.编写一个C++程序，它要求用户输入一个已long为单位的距离，然后将他转换为码(一long等于200码)
#include <iostream>
using namespace std;
int s_long(int n);
int main()
{
    cout<<"Enter you long number";
    int address;
    cin>>address;
    int result=long(address);
    cout<<result;
    return 0;
}
int long(int n)
{
    return n*220;
}
3.编写一个C++程序，它使用3个用户定义的函数(包括main())，并生成下面的输出:
Three blind mice
Three blind mice
See how they run
See how they run
Code:
#include <iostream>
using namespace std;
void show_message1(void);
void show_message2(void);
int main()
{
    show_message1();
    show_message1();
    show_message2();
    show_message2();
    return 0;
}
void show_message1(void)
{
    cout<<"Three blind mice"<<endl;
}
void show_message2(void)
{
    cout<<"See how they run"<<endl;
}
4.编写一个程序，让用户输入其年龄，然后现实该年龄包含多少个月，如下所示：
Enter you age:29
Code:
#include <iostream>
using namespace std;
int age(int);
int main(void)
{
    int month,ages;
    cout<<"Enter your age:"<<endl;
    cin>>ages;
    month=age(ages);
    cout<<month<<endl;
    return 0;
}
int age(int n)
{
    return n*12;
}
5.编写一个程序，其中的main()调用一个用户定义的函数(以摄氏温度值为参数，并返回相应的华氏温度)。该程序按下面的格式要求用户输入摄氏温度值，并显示结果。
Please enter a Celsius value:20
20 degrees Celsius is 68 degrees Fahrenheit.
下面是转换公示:
华氏温度=1.8*摄氏温度+32.0
#include <iostream>
using namespace std;
double Fahrenheit(double n);
int main()
{
    int celsius;
    cout<<"Please enter a Celsius value:";
    cin>>celsius;
    cout<<celsius<<" degrees Celsius is "<<Fahrenheit(celsius)<<" degrees Fahrenheit"
    <<endl;

    return 0;
}
double Fahrenheit(double n)
{
    return 1.8*n+32.0;
}
6.编写一个程序，其main()调用一个用户定义的函数(以光年值为参数，并返回对应天文单位的值)。该程序按下面的格式要求用户输入光年值，并显示结果:
Enter the number of light year:4.2
4.2 light years=265608 storonomical units.
天文单位是从地球到太阳的平均距离(约150000000公里或93000000英里),光年是光一年走的距离(约10万亿公里或6万亿公里英里)(除太阳外，最近的恒星大约离地球4.2光年)。请使用double类型，转换公式为:
1光年=63240天文单位
#include <iostream>
using namespace std;
double years(double n);
int main(void)
{
    double year,light_year;
    cout<<"Enter the number of light year:";
    cin>>year;
    light_year=years(year);
    cout<<year<<" light years="<<light_year<<" storonomical units."<<endl;
    return 0;
}
double years(double n)
{
    return n*63240;
}
7.编写一个程序，要求用户输入小时数和分钟数。在main()函数中，将这两个值传递给一个void函数，后者以下面这样的格式显示这两个值：
Enter the number of hours:9
Enter the number of minutes:28
Time:9:28
Code:
#include <iostream>
using namespace std;
void time_demo(int h,int m);
int main()
{
    int hours,minutes;
    cout<<"Enter the number of hours:";
    cin>>hours;
    cout<<"Enter the number of minutes:";
    cin>>minutes;
    time_demo(hours,minutes);
    return 0;
}
void time_demo(int h,int m)
{
    cout<<"Time:"<<h<<":"<<m<<endl;
}
