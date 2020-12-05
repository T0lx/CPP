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
    cout<<"Name:Toin"<<endl<<"Address：beijing";
    return 0;
}
2.编写一个C++程序，它要求用户输入一个已long为单位的距离，然后将他转换为码(一long等于200码)
#include <iostream>
using namespace std;
int long(int n);
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