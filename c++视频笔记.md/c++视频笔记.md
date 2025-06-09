#### 1、c++的创建步骤
```c++
编写c++有四步骤

创建项目（进入vs开使创建新项目；项目名称选定后浏览加入内容让后创建}

创建文件（右侧源文件添加新建项目书写代码）

```C++
#include <iostream>
int main() {
    std::cout << "Hello, World!" << std::endl;
    return 0;
}
```


### 2、代码的2种注释
- 代码中两种注释 
- ` //`（单行注释；可以把一行的信息作为注释）
- /**/（多行注释；可以把多行信息进行注释)通常放在代码上方或者·结尾
```C++
#include <iostream>

int main()

 {
    //代码含义输出HELLOWORD到屏幕
    std::cout << "helloeword" << std::endl;
    return 0;   
}
```


#### 3、变量
- 变量（给一段指定内存空间起名方便操作这段内存）（方便管理内存空间）、（数据类型  变量名 = 变量初始值   ( int   1 = 000)
- 例如（1=000）可命名
- 变量创建语法：数据类型 变量名=变量初始值；（int  a=10）
```c++
#include <iostream>

int main() 
{
	int 1 1000）;
    std::cout << "H World!" << std::endl;
    return 0;ello
}
```


#### 4、常量
- 常量（作用于记录程序中不可改的数据）c++定义常量的方式分两种（#define  宏常量）：表示一个常量                         
- const修饰的变量：通常在变量定义前加cons
- 修饰该变量为常量格式为
```c++
#include <iostream>
using namespace std;

int main()
{

   // #define day 7
    cout << "一周总共有 " << day <<"天" << endl;
    const修饰的变量int mont = 12;
    
    cout <<"一年总共有” >>  << mont << “个月份 " << endl;
    system ("pause");
    }
```





#### 5、关键字
- 关键字：是c++中预先保留的单词（标识符）（在在定义变量或者常变量的时候，不用关键字取名）
- 标识符命名规则；
- 1：标识符不能是关键字（int int = 83是不允许的）
-  2；标识符只能由字母，数字，下划线组成（int 123abd = 12 是不允许的）（可以是 int -ada = 12）
-  3，第一个字符必须由由字母或者下划线组成
-  4，标识符中字母分大小写


### 6、数据类型
数据类型的意义；给变量分配合适的内存
				  
 - 整形；整形变量表示的是整数类型的数据数据类型（
 - short(短整形)占2字节
 - int（整形）占4字节
 - iong（长整形）windows为4字节 linux为4字节（32位） 8字节（64位）
 - longlong(长长整形)  
 ```c++               
#include <iostream>
using namespace std;

int main() {

	short num1 = 10;
	int num2 = 20;
	long num3 = 30;
	long long num4 = 40;

	cout << "num1 = " << num1 << endl;
	cout << "num2 = " << num2 << endl;
	cout << "num3 = " << num3 << endl;
	cout << "num4 = " << num4 << endl;

	// 用于暂停程序，以便查看输出
	cin.get();

	return 0;
}
```



### 7、sizeof关键字                  
- sizeof关键字 
- 用；利用sizeof关键字可以统计数据类型所占的大小
```c++

#include <iostream>
using  namespace std;

int main() {
	short num1 = 10;
	cout << "short占用内存空间为；" << sizeof(short) << endl;
                                （求出数据内存）
	int num2 = 24;
	cout << "int占用内存空间为；" << sizeof(int) << endl;
                              （求出数据内存）
	long num3 = 10;

	cout << "long占用内存空间为；" << sizeof(long) << endl;

	long long num4 = 10;
	cout << "long long占用内存空间为；" << sizeof(long long) << endl;
	system("pause");
}
```



### 8、实型
- 实型用于表示小数（浮点型）
- 1，单精度（flat) 双精度（double)占用4字节（7位有效数字） 用8字节（15~16位有效数字）
```c++
例如；#include <iostream>
using namespace std;

int main()
{
	//1,单精度 float  
	float f1 = 3.14f;
	//1,双精度 double  
	cout << "f1 =" << f1 << endl;
	double d2 = 3.14;
	cout << "d2=" << d2 << endl;
	cout << "float占用空间为" << sizeof(float) << endl;
	cout << "double占用空间为" << sizeof(double) << endl;
	//科学计数法
	float f2 = 3e2;//3*10^2
	double d3 = 3e-2;//3*0.1^2
	cout << "float = " << f2 << endl;
	cout << "doube =" << d3 << endl;
	return 0;
}
```


### 9、字符型
- 字符型用于显示单个字符。他的语法（chaed ch ='a';(不能用""符号)
- 1，c和c++中字符型变量只占用一个字节 2.字符型变量并不是把字符本身放到内存中存储，而是把相对应的ASCII编码放入存储单元
例如b=2；a=1 c =3
- ASCLL码由两部分组成的（
- 1，非打印控制字符（0——31分配给了控制字符，用于控制像打印机等一些外围设备）
-  2，打印字符（数字32—126分配给了能在电脑键盘上能找到的字符，当查看或者打印文档就会出现）
```c++

#include <iostream>
using namespace std;

int main() {
	//1,字符型变量创建方式
	char ch = 'a';//不能把单引号用错成双引号（单引号内只能有一个字符）（也不能在单引号里面写多个字符）
	cout << "a" << endl;
	//字符变量所占内存大小（sizeof)
	cout << "char所占内存大小" << sizeof(char) << endl;
	//字符型变量对应的ASCLL编码//a=97  A=65
	cout << (int)ch << endl;


	return 0;

	
}
```


### 10、转义字符
- 转义字符（用于一些不能显示的ASCLL字符
常用的转义字符；` \n`换行符）   ` \\`（反斜杠）；
- 输出一个杠到屏幕）  ` \t`（水平制表符）；可以整齐输出数据 
```c++

例如：
#include <iostream>
using namespace std;

int main() {
	cout <<"hello\t" << endl;
	cout << "hello worlde\t" << endl;
	cout << "hello 你好\t" << endl;
	cout << "hello\n" << endl;
	return 0;
}
```


### 11、字符串类型
- 字符串类型
- 1：c风格字符串（char 变量名【】="字符串值”)
- 2：c++风格字符串（string 变量名 ="字符串值")注意（用string之前需要包含头文件#include <string>)
```c++

 #include <iostream>
using namespace std;
#include <string>
int main()


{//c字符风格char 字符串后面得加【】字符不能使用单引号(因为单引号里面只能有一个字符）
	char str[] = "hello";
//c++字符风格string（用string时 需要包含头文件#include <string>
	string str3 = "hello";
	cout << str << endl;

	cout << str3 << endl;
	return 0;
}
```
/////////////////////////////////////////////////////////////////

### 12、布尔类型bool

- 布尔类型bool(只占用一个字节）只有两个值，true(真本质是1)false(假本质是0)

```c++
#include <iostream>
using namespace std;

int main() {
	//创建bool的数据类型
	bool flag = true;//true代表真（本质是1）
	cout << flag << endl;

	flag = false;//false代表假（本质是0）
	cout << flag << endl;
	//查看bool类型所占内存大小
	cout << "bool所占内存" << sizeof(bool) << endl;

	return 0;
}
```

### 13、数据输入
- 作用从键盘获取数据。关键词（cin)语法（cin>>变量）除数不能为零
例如；
```c++
#include <iostream>
using namespace std;
int main() {
	int a = 0;//整形量a
	//1、整形
	cout << "请给整形量a赋值" << endl;
	cin >> a;
	cout << "整形量a =" << a  << endl;
//2、浮点型
	float ste1 = 3.13f;//单精度
	cout << "请给整形量ste1赋值 " << ste1 << endl;
	cin >> ste1;
	cout << "ste1 =" << ste1 << endl;

	double f3 = 3.98;//双精度
	cout << "请给整型量f3赋值 " << f3 << endl;
	cin >> f3;
	cout << "f3 = " << f3 << endl;
//3、字符型
	char ch = 89;
	cout << "请给整形量ch赋值" << endl;
	cin >> ch;
	cout << "ch = " << ch << endl;
//4、字符串型
	char f5[] = "43";//c字符风格
	cout <<"请给字符串f5赋值" << endl;
	cin >> f5;
	cout << "字符串f5 =" << f5 << endl;
	string f6 = "45";//c++字符风格
	cout << "请给字符串f6赋值" << endl;
	cin >> f6;
	cout << "字符串6 =" << f6 << endl;
	//5、布尔类型(除了0代表假剩下都代表真)
	bool flog = true;//本性真
	cout << "请给flog赋值" <<flog << endl;
	cin >> flog;
	cout << "布尔flog =" << flog <<endl;
	bool f7 = false;//本性假
	cout << "请给f7赋值" <<f7 << endl;
	cin >> f7;
	cout << "布尔f7 =" <<f7 << endl;
    return o;
}
```

### 14、算数运算符
- 作用；用于执行代码运算
- 1、算数运算符（用于处理四则运算）
- 2、赋值运算符（用于将表达式的值赋给变量）
- 3、比较运算符（用于表达式的比较，并返回一个真值或者假值）
 - 4、逻辑运算符（用于根据表达式的值返回真值或假值）
	
例如；
```c++
include <iostream>
using namespace std;

int main() {
	//加减乘除运算
	int a1 = 30;
	int b2 = 60;
	cout << a1 + b2 << endl;
	cout << b2 - a1 << endl;
	cout << a1 * b2 << endl;
	cout << b2 / a1 << endl;//两整数相除，结果依然是整数，会将小数部分去除因为int是整形
	double d1 = 0.5;
	double f2 = 0.22;//两数相除，小数部分未被去除是因为double是双精度（浮点型)
	cout << d1 / f2 << endl;


	return 0;
}
```
### 15、取模运算
- 用于处理四则运算%（取模（取余））只有整数能取模小数不可以
```c++
#include <iostream>
using namespace std;

int main() {
	int a1 = 10;
	int b2 = 3;
	cout << a1 % b2 << endl;//取模运算的本质就是余数
	int a2 = 10;
	int e2 = 0;
	//cout << a1 % e2 << endl;//除数为零了所以无法运行
	
	return 0;
}
```
### 16、递增递减
- 用于四则运算++（前置递增或后置递减）--（前置递减或者后置递减）
例如；
```c++
#include<iostream>
using namespace std;
int main() {
	//1、前置递增
	int a = 10;
	++a;//让变量+1
	cout << "a =" << a << endl;

	//2、后置递增
	int b = 20;
	b++;//让变量+1
	cout << "b =" << b << endl;

	//3、前置和后置的区别
	//前置递增先让变量+1 后进行表达运算
	int a2 = 19;
	int b2 = ++a2 * 10;//（19+1）*10
	cout << "a2 =" << a2 << endl;
	cout <<"b2 ="<<b2 <<endl;

	//后置递增先进行表达运算 后让变量+1
	int w1 = 20;
	int e2 = w1++ * 30;//（先w1*30）后w1+1
	cout << "w1 =" << w1 << endl;
	cout << "e2 =" << e2 << endl;

	//4、前置递减和后置递减
	int a3 = 10;
	int b3 = --a3 * 10;//先让变量-1在运算*10;(10-1)*10
	cout << "--a3 =" << a3 << endl;
	cout << "--b3=" << b3 << endl;
	int a4 = 30;
	int b4 = a4-- * 50;//先运算*50 再让变量-1;(30*50)后30-1
	cout << "a4 =" << a4 << endl;
	cout << "b4 =" << b4 << endl;

    return o;
	//总结前后递增递减就是一个先加在乘 一个先乘再加  、递减同理
	
}
```




### 17、赋值运算符
- 用于将表达式的值赋给变量 =（赋值） +=（加等于）-=（减等于） %=（乘等于）···· 
例如
```c++
#include <iostream>
using namespace std;

int main() {
	//+=
	int a = 10;
	a += 2;//a=a+2
	cout << "a =" << a << endl;
	//-=
	int a1 = 10;
	a -= 2;//a=a1-2
	cout << "a =" << a << endl;
	//*=
	int a2 = 10;
	a2 *= 3;//a2=a2*3
	cout << "a 2=" << a2<< endl;
	// /=
	int a3 = 20;
	a3 /= 4;//a3=a3/4
	cout << "a3=" << a3 << endl;
	//%=
	int a4 = 12;
	a4 %= 6;
	cout << "a4 =" << a4 << endl;
	return 0;
}
```

#### 18、比较运算符
- 用于表达式的比较；并返回一个真值或者假值（==相等于），
- ！=（不等于），
- <（小于），>(大于
)，
- <=(小于等于),>=(大于等于)例如
```c++
#include <iostream>
using namespace std;

int main() {
	//==
	int a = 10;
	int b = 20;
	cout << (a == b) << endl;
	//!=
	cout << (a != b) << endl;
	//<
	cout << (a < b) << endl;
	//>
	cout << (a > b) << endl;
	//<=
	cout << (a <= b) << endl;
	//>=
	cout << (a >= b) << endl;




	return 0;
}
```
### 19、逻辑运算符 非、与、或、
- ！（非）：
- &&（与）
- ||(或)
```c++
#include <iostream>
using namespace std;

int main() {
	//逻辑非 ！
	int a = 10;//在c++中除了0，都为真
	cout << !a << endl;
	cout << !!a << endl;


	//逻辑 与 &&
	int a1 = 10;
	int a2 = 0;//一个为假结果就为假//同真为真，其于为假
	cout << (a1 && a2) << endl;

	//逻辑 或 ||
	int a3 = 10;
	int a4 = 0;//有一个是真的结果就为真//同假为假，同真为真
	cout << (a3 || a4) << endl;




	return 0;
}

```
###  程序流程结构分
- 1、顺序结构（程序按照顺序执行不发生跳转） 
- 2、选择结构（依据条件是否满足，有选择的执行相应功能）
-  3、循环结构（ 依据条件是否满足，循环多次执行某段代码)
### 20、程序流程结构-单行if语句
- 作用；执行满足条件的语句
- if的三种形式1、（单行格式if语句）
- 2、（多行格式if语句）
- 3、（多条件的if语句）
例如
```c++
int  main() {

	int score = 0;
	cout << "请输入一个分数" << endl;
	cin >> score; //cin(为一个量赋值）
	cout << "您输入的分数为" << score << endl;


	if (score > 600)//如果分数大于600、注意if（）后边不能加分号
		cout << "恭喜您考上一本大学" << endl;//视为恭喜你考上一本大学，输出到屏幕


}
```


### 21、多行格式if语句
- 多行格式if语法（if条件满足执行的语句）else()条件不满足执行的语句）
```c++
#include <iostream>
using namespace std;


int  main() {
	
	int score = 0;
	cout << "请输入你的分数" << endl;
	cin >> score;
	cout << "你输入的分数为" << score << endl;
	if(score > 600)
		cout << "恭喜你满足分数线要求" << endl;
	else//判断词汇
		cout << "很遗憾未能满足要求" << endl;
```


### 22、多条件的if语句
- 多条件的if语句；
- if（条件1满足执行的语句）else if（条件2）（条件2满足执行的语句） ····else（都不满足执行的语句）
例如；
```c++
#include <iostream>
using namespace std;


int  main() {
	
	int score = 0;
	cout << "请输入你的分数" << endl;
	cin >> score;//给变量赋值
		cout << "你输入的分数是" << score << endl;
		if (score > 600)
			cout << "恭喜你分数合格" << endl;
		else if (score > 500)
			cout << "抱歉你的分数只够二本" << endl;
		else if (score > 400)
			cout << "你只能上大专" << endl;
		else if (score > 300)
			cout << "差不多废了" << endl;
		else
			cout << "300都没有躺着呗" << endl;
	


	return 0;
}
```

### 23、嵌套if语句
- 在if语句中可以嵌套使用if语句，达到更精准的判断
例如
```c++
#include <iostream>
using namespace std;


int  main() {

	int score = 0;
	cout << "请输入分数" << endl;
	cin >> score;
	cout << "你输入的分数为" << score << endl;


	if (score > 600)
		cout << "恭喜分数合格" << endl;
	if (score > 700) {
		cout << "您能考入清华大学" << endl;
	}
	else if (score > 650) {
		cout << "你可以上人民大学" << endl;
	}
	else {
		cout << "你可以上川大" << endl;
	}
	if (score>600){}
	else if (score > 500) {
		cout << "恭喜进一本" << endl;
	}

	else if (score > 400)
		cout << "恭喜进二本" << endl;


	else if (score > 300) {
		cout << "恭喜进三本" << endl;
	}


	else
		cout << "很遗憾，再加油" << endl;


	return 0;
	}

```

### 24、三位选手称体重

```c++
#include <iostream>
using namespace std;

int main() {

	int num1 = 0;
	int num2 = 0;
	int num3 = 0;
	cout << "请输入选手1体重" << endl;
	cin >> num1;

	cout << "请输入选手2体重" << endl;
	cin >> num2;

	cout << "请输入选手3体重" << endl;
	cin >> num3;

	cout << "选手1的体重为" << num1 << endl;
	cout << "选手2的体重为" << num2 << endl;
	cout << "选手3的体重为" << num3 << endl;


	//判断那个最重
	//先判断1和2重量
	if (num1 > num2)//1比2重
	{
		if (num1 > num3)//1比3重
		{
			cout << "选手1最重" << endl;
	}
		else //3比1重
		{
			cout << "选手3最重" << endl;
		}
	}
	else//2比1重
	{
		if (num2 > num3) //2比3重
		{
			cout << "选手2最重" << endl;
	 }
		else//3比1重
		{
			cout << "选手3最重" << endl;
		}
     
	}
	

		return 0;

}

```

//////////////////////////////////////////////////////////////////////////////////////////////


### 25、三目运算符
- 作用；通过三目运算来进行简单的判断
- 语法；表达式1？表达式2：表达式3（如果表达式1的值为真，执行表达式2，并返回表达2的结果）（如果表达式1的值为假，执行表达式3，并返回表达式3的结果）
```c++
#include <iostream>
using namespace std;

int main() {
	//将a和b作比较，将变量大的赋值给c
	int a = 10;
	int b = 20;
	int c = 0;
	c = (a < b ? a: b);
	cout << "c =" << c << endl;
	//在c++中返回的是变量 可以继续赋值
	(a > b ? a : b) = 100;
	cout << "a=" << a << endl;
	cout << "b =" << b << endl;




	return 0;
}
```

### 26、switch语句
- 作用；执行多条件分支语句
- 语法；switch（表达式）、case()、break()、default()
- 注意1；switch语句中表达式类型只能是整型或者字符型
- 注意2；case里如果没有break程序会一直执行
- 总结；与if语句比，对于多条件判断时，switch语句结构清晰，执行效率高，缺点就是不可以像if语句一样判断区间
例如
```c++
#include <iostream>
using namespace std;

int main() {
	int score = 0;
	cout << "请你为这个节目打分" << endl;
	cin >> score;
	cout << "您打的分为" << score << endl;
	switch (score) {
	case 10:
		cout << "你觉得这个节目非常完美" << endl;
		break;
	case 9:
		cout << "你觉得这个节目完美" << endl;
		break;
	case 8:
		cout << "你觉得这个节目还不错" << endl;
		break;
	case 7:
		cout << "你觉得这个节一般" << endl;
		break;
	default:
		cout << "你认为这是烂片" << endl;

	}

	return 0;
}
```

#### 27、循环结构 while
- 作用；满足循环条件，执行循环语句
- 语法；while（循环条件）{循环语句}
- 解释；只要循环条件的结果为真，就执行循环语句
- 注意；在执行循环语句的时候，程序必须提供跳出循环的出口，否则出现死循环
例如
```c++
#include <iostream>
using namespace std;

int main() {
	int num = 0;
	//while(）填入循环条件；一定要避免死循环
	//注意事项
	while (num < 50)
	{
		cout << num << endl;
		num++;
	}
	return 0;
}
```
### 28、循环案例猜数字
```c++
#include <iostream>
using namespace std;
#include<ctime>//time系统时间头文件

int main()
{
	srand((unsigned int)time(NULL));//随机数种子
	//1、系统随机生成数字
	int num = rand() % 100 + 1;
	//2、玩家进行猜测
	int val = 0;
	while (1) {

		cin >> val;
		if (val > num)//3、判断玩家猜测
		{
			cout << "你猜测过大" << endl;
		}
		else if (val < num) {
			cout << "你猜测过小" << endl;
		}
		else {
			cout << "恭喜猜对了" << endl;//4、猜对退出游戏
			break;//break，可以利用该关键词来退出当前循环
		}


	}
	return 0;
}
```

### 29、dowhile语句
- 作用；满足循环条件，执行循环语句
- 语法；do{循环语句}while{循环条件}
- 注意；与while语句不同的是dowhile会先执行一次循环语句，在判断循环条件
```c++
#include <iostream>
using namespace std;

int main()
{
	int num = 0;
	do {
		cout << num << endl;
		num++;

	} while (num < 10);

	return 0;
}
```
### 30、案例练习（水仙花数）
```c++
#include <iostream>
using namespace std;

int  main() {
	int num = 100;
	do {

		
		
		int a = num % 10;
		int b = num / 10 % 10;
		int c = num / 100;

		if (a * a * a + b * b * b + c * c * c == num) {
			cout << num << endl;
		}
			num++;
		} while (num < 1000);


	
	      return 0;
	}

```

### 31、for循环
- 作用；满足循环条件，执行循环语句
- 语法；for（起始表达式；表达条件；末尾循环体）{循环语句;}
```c++
#include <iostream>
using namespace std;

int  main() {
	for (int i = 0; i < 10;i++)
		cout << i << endl;

	
	      return 0;
	}
```

### 32、案例练习（敲桌子）
```c++
#include <iostream>
using namespace std;

int  main() {
	for (int i = 1;i <= 100;i++) {
		if (i % 7 == 0 || i % 10 == 7 || i / 10 == 7) {
			cout << "敲桌子" << endl;
		}
		else {
			cout << i << endl;
		}
	}
	return 0;

}
```
### 33、嵌套循环
```c++

#include <iostream>
using namespace std;

int  main() {
	for (int i = 0;i < 10;i++)//外层执行一次
	{
		cout << "* ";

		for (int j = 0;j < 10;j++)//内层执行一周
		{
			cout << "* ";
		}cout << endl;
	
	}
	cout << endl;
	return 0;

}
```
### 34、用for循环打印乘法表
```c++
#include <iostream>
using namespace std;

int  main() {
	for (int i = 1;i <= 9;i++) {
		for (int j = 1;j <= i;j++) {
			cout << j << "*" << i << "=" << j * i << " ";
		}cout << endl;


	}cout << endl;
	return 0;

}
```
#### 35、跳转语句 break语句
- 作用；用于跳出选择结构或者循环结构
- break的使用时机；
- 1、出现在switch条件语句中，作用是终止case并跳出switch语句
- 2、出现在循环语句中，作用是跳出当前循环
- 3、出现在嵌套循环中，跳出内层循环



```c++
例如1switch语句
#include <iostream>
using namespace std;

int main() {
	cout << "请选择你的难度" << endl;
	cout << "1、普通难度" << endl;
	cout << "2、精英难度" << endl;
	cout << "3、地狱难度" << endl;
	int num = 0;
	cin >> num;
	switch (num) {

	case 1:
		cout << "你选择的是普通难度" << endl;
		break;
	case 2:
		cout << "你选择的是精英难度" << endl;
		break;
	case 3:
		cout << "你选择的是地狱难度难度" << endl;
		break;
	}

		return 0;

}
例如2  for(循环嵌套） 
```c++
#include <iostream>
using namespace std;

int main() {
	for (int i = 0;i < 10;i++) {

		for (int j = 0;j < 10;j++) {
			if (j == 6)
				break;
				
			cout << "* ";
		}cout << endl;


	}cout << endl;

		return 0;

}
```c++
例如3(for循环)
#include <iostream>
using namespace std;

int main() {
	for (int i = 0;i < 10;i++) {
		if (i == 7) {
			break;

		}
		cout << i << endl;

	}
		return 0;

}
```
## 36、跳转语句（continue)
- 作用；在循环语句中，跳过本次循环中尚未执行的语句，继续执行下一项
例如
```c++
#include <iostream>
using namespace std;

int main() {
	for (int i = 0;i <= 100;i++) {
		if (i % 2 == 0)//输出奇数，不输出偶数
		{
			continue;//1、与break的区别在于break会退出当前循环，continue会执行下一项
			           //2、continue会筛选条件，执行到此就不会向下执行，执行下一次循环

		}
		cout << i << endl;
}
		return 0;

}
```
## 37、跳转语句 goto
- 作用；可以无条件跳转语句
- 语法；goto标记;
例如
```c++
#include <iostream>
using namespace std;

int main()
{
	
	cout << "1、***" << endl;
	goto falg;//跳转到标记的地方
	cout << "2、***" << endl;
	
	cout << "3、***" << endl;
	falg://标记后面用冒号不能用分号
	cout << "4、***" << endl;

		return 0;

}
```

## 数组定义方式
- 所谓数组，就是一个集合，里面放了相同类型的数据元素
- 1、数组中的每个数据元素都是相同的数据类型
 - 2、数组是由连续的内存位置组成的



## 38、一维数组
一维数组定义的三种方式
- 1、数据类型  数组名【数组长度】
- 2、数据类型 数组名【数组长度】={值1、值2....}
- 3、数据类型 数组名【】={值1、值2....}
```c++
- 1、数据类型  数组名【数组长度】
#include <iostream>
using namespace std;

int main()
{
	int arr[5];
	arr[0] = 10;
	arr[1] = 20;
	arr[2] = 30;
	arr[3] = 40;
	arr[4] = 50;
	cout << arr[0] << endl;
	cout << arr[1] << endl;
	cout << arr[2] << endl;
	cout << arr[3] << endl;
	cout << arr[4] << endl;

		return 0;

}
```

- 2、数据类型 数组名【数组长度】={值1、值2....}
```c++
#include <iostream>
using namespace std;

int main()
{
	int arr[5] = { 10,20,30,40,50 };
	for (int i = 0;i < 5;i++) {
		cout << arr[i] << endl;

	}


		return 0;

}
```
- 3、数据类型 数组名【】={值1、值2....}
```c++
#include <iostream>
using namespace std;

int main()
{
	int arr[] = { 10,20,30,40,50,60,70,80,90, };
	for (int i = 0;i < 9;i++) {
		cout << arr[i] << endl;

	}


		return 0;

}
```
//////////////////////////////////////

## 39、一维数组数组名
- 用途；
- 1、可以统计整个数组在内存中的长度
-  2、可以获取数组在内存中的首地址
```c++
例如
#include<iostream>
using namespace std;

int main() {
    //数组的用图
    //1、可以通过数组名统计出数组所占内存
    int arr[9] = { 10,20,30,40,50,60,70,80,90, };
    cout << "数组占用内存" << sizeof(arr) << endl;
    cout << "数组的长度为" << sizeof(arr[0]) << endl;
    cout << "数组中元素的个数" << sizeof(arr) / sizeof(arr[0]) << endl;

    //2、可以通过数组名查看数组首个地址
    cout <<"数组的首地址为"<<(int) arr << endl;
    cout << "数组中第一个元素的地址" <<(int) & arr[0] << endl;
    cout << "数组第二个元素地址为" <<  (int)&arr[1] << endl;
    //数组名是常量，不可以进行赋值操作
    return 0;
}
```
### `五个小猪称体重`
```c++
#include<iostream>
using namespace std;

int main() {
    //创建五只小猪体重
    int arr[5] = {323,423,323,232,424, };
    int max = 0;//先认定最大值为0
    for (int i = 0;i < 5;i++) 
    {
        
        if (arr[i] > max)//如果访问数组中的元素比我认定的最大值还大，更新最大值
        {
            max = arr[i];
           
        }
       
    }
    cout << "最重的小猪体重为： "<<max << endl;
    


    return 0;
}
```
### `元素逆置`
```c++
using namespace std;

int main() {
    int arr[5] = { 1,3,5,3,6 };
    cout << "数据逆置前" << endl;
    for (int i = 0;i < 5;i++) {
        cout << arr[i] << endl;

    }cout << endl;


        int start = 0;//起始下标
        int end = sizeof(arr) / sizeof(arr[0]) - 1;//末尾元素下标
                 //数组的长度除以每个元素所占内存空间-1


        while(start<end)//satre<end就开始执行
        {
        //实现元素互换
        int temp = arr[start];//temp临时记录起始坐标
        arr[start] = arr[end];
        arr[end] = temp;

        start++;end--;//下标更新

    }
        //打印逆置后的数据
        cout << "数据逆置后" << endl;
        for (int i = 0;i < 5;i++) {

            cout << arr[i] << endl;
        }

    return 0;
}
```
## 40、冒泡排序
- 作用；最常用的排序手法，对组内元素进行排序
- 1、比较相邻元素，如果第一个比第二个大，就交换他们两个
- 2、对每一对相邻元素做同样的工作，执行完毕后，找到第一个最大值
- 3、重复以上步骤，每次比较数-1，直到不需要比较
```c++
#include<iostream>
using namespace std;

int main()
{
    //1、利用冒泡排序实现升序序列
    int arr[9] = { 1,3,2,6,7,5,4,9,8, };
    cout << "排序前： " << endl;

    for (int i = 0;i < 9;i++)
    {
        cout << arr[i] << "  ";
    }cout << endl;
    //2、开始冒泡排序
    //总共排序轮数为元素个数-1
    for (int i = 0;i < 9 - 1;i++)
    {    
        //内层循环对比 次数=元素个数-当前轮数-1
        for (int j = 0;j < 9 - i - 1;j++)
        {
            //如果第一个数字，比第二个大，交换两数字
            if (arr[j] > arr[j + 1]) 
            {
                int temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;

           }
        }
    }
    //排序后结果
    cout << "排序后： " << endl;
    for (int i = 0;i < 9;i++) {
        cout << arr[i] << "  ";
    }cout << endl;


    return 0;
}
```
## 41、二维数组的定义方式
- 1、数据类型 数组名【行数】【列数】；
- 2、数据类型 数组名【行数】【列数】={{数据1，数据2}，{数据3，数据4}}；
- 3、数据类型 数组名【行数】【列数】={数据1，数据2，数据3，数据4，}；
- 4、数据类型 数组名【】【列数】={数据1，数据2，数据3，数据4}；
- 建议；使用第二种更加直观，提高代码可读性。

```c++
1、第一种
#include<iostream>
using namespace std;

int main()
{
    int arr[2][3] = { 1,2,3,4,5,6, };
    for (int i = 0;i < 2;i++) {
        for (int j = -0;j < 3;j++) {
            cout << arr[i][j] <<" ";
        }
    }cout << endl;

    return 0;
}
```
2、第二种
```c++
#include<iostream>
using namespace std;

int main()
{
    int arr1[2][3] = 
    { 
      {1,2,3,},
      {4,5,6,}
    };
    for (int i = 0;i < 2;i++) {
        for (int j = 0;j < 3;j++) 
        {
            cout << arr1[i][j] <<" ";
        }
        cout << endl;
    }
    return 0;
}
```
3、第三种
```c++
#include<iostream>
using namespace std;

int main()
{
    int arr2[2][3] = { 1,2,3,4,5,6, };
    for (int i = 0;i < 2;i++) {
        for (int j = 0;j < 3;j++) {
            cout << arr2[i][j] << " ";

        }cout << endl;

    }
   
    return 0;
}
```
4、第四种
```c++
#include<iostream>
using namespace std;

int main()
{
    int arr2[][3] = { 1,2,3,4,5,6, };
    for (int i = 0;i < 2;i++) {
        for (int j = 0;j < 3;j++) {
            cout << arr2[i][j] << " ";

        }cout << endl;

    }
   
    return 0;
}
```
## 42、二维数组——数组名
- 1，查看二维数组所占内存空间
- 2，获取二维数组首地址
```c++
#include<iostream>
using namespace std;

int main()
{
    int arr[2][3] = { {1,2,3},{4,5,6,} };
    cout << "二维数组所占内存空间; " << sizeof(arr) << endl;
    cout << "二维数组第一行所占空间" << sizeof(arr[0]) << endl;
    cout << "二维数组第一个元素所占内存" << sizeof(arr[0][0]) << endl;

    cout << "二维数组行数为" << sizeof(arr) / sizeof(arr[0]) << endl;
    cout << "二维数组的列数为" << sizeof(arr[0]) / sizeof(arr[0][0]) << endl;

    cout << "二维数组首地址" << (int)arr << endl;
    cout << "二维数组第一行的首地址" << (int)arr[0] << endl;
    cout << "二维数组第二行的首地址" << (int)arr[1] << endl;

    cout << "二维数组第一个元素首地址" << (int)&arr[0][0] << endl;
    cout << "二维数组第二个元素首地址" << (int)&arr[0][1] << endl;


    return 0;
}
```
## 43、考试成绩统计
```c++
#include<iostream>
using namespace std;

int main()
{
    int score[3][3] = 
    {   
        {100,132.100},
        {21,31,32},
        {11,12,13}, 
    };
    string names[3] = { "张三","李四","王五", };
    //2、统计每个人的分数
    for (int i = 0;i < 3;i++)
    {
        int sum = 0;//统计分数总和变量
        for (int j = 0;j < 3;j++)
        {
            sum += score[i][j];
            //cout << score[i][j] << " ";
        }
        cout << names[i] <<"的总分； "<<sum<< endl;
    }

    return 0;
}
```
## 函数
- 作用；将一段经常使用的代码封装起来，减少代码重复，一个较大程序，一般分为若干
 个程序块，每个模块实现特定的功能


## 44、函数的定义
函数的定义分为五个步骤
- 1、返回值类型 
- 2、函数名 
- 3、参数表列
- 4、函数体语句
- 5、return表达式
- 语法；返回值类型 函数名（参数列表）{函数体语句 return表达式}
 ```c++
 #include<iostream>
using namespace std;

//返回值类型 函数名（参数列表）{函数体语句 return表达式}
int add(int num1,int  num2) {
    int sun = num1 + num2;
    return sun;
}


int main()
{
    
    
    return 0;
}
```
## 45、函数的调用
- 功能；使用定义好的函数
- 语法；函数名（参数）
```c++
#include<iostream>
using namespace std;

//返回值类型 函数名（参数列表）{函数体语句 return表达式}
//函数定义的时候，num1,num2并没有真是数据，他只是一个形式上的参数，简称型参
int add(int num1,int  num2)//add(a, b)的值会传递给num1,num2
{
    int sun = num1 + num2;
    return sun;
}

int main()
{
    //main函数中调用add函数
    int a = 10;
    int b = 23;
    //函数调用语法；函数名称（参数）
    //a和b称为实际参数 简称实参
    //当调用函数的时候，实参的值会传递给型参
    int c = add(a, b);
    cout << "c=" << c << endl;

    return 0;
}
```
## 46、值传递
- 所谓值传递，就是函数调用时实参将数据传递给形参
值传递时，如果形参发生变化不会影响实参
- 总结；值传递时，形参修饰不了实参
```c++
#include<iostream>
using namespace std;

//值传递
//定义函数，实现两个数字互换
//如果函数不需要返回值，声明的时候可以用void
void arr(int num1,int num2)
{
    cout << "交换前; " << endl;
    cout << "num1=" << num1 << endl;
    cout << "num2=" << num2 << endl;
    int temp = num1;
    num1 = num2;
    num2 = temp;

    cout << "交换后; " << endl;
    cout << "num1=" << num1 << endl;
    cout << "num2=" << num2 << endl;


    //return;返回值不需要的时候可以不写return
}

int main()
{
    int a = 21;
    int b = 42;
    cout << "a= " << a << endl;
    cout << "b= " << b << endl;
    //当我们做值传递的时候，函数形参发生变化并不会影响实参
    arr(a, b);
    cout << "a= " << a << endl;
    cout << "b= " << b << endl;

  
    return 0;
}
```
## 47、常见样式
常见的函数样式有四种
- 1、无参无返
-  2、有参无返 
- 3、无参有返
- 4、有参有返
```c++
#include<iostream>
using namespace std;
//1、无参无返
void arr01() {
    cout << "arr01" << endl;
}
// 2、有参无返
void arr2(int a) {
    cout << "arr2 a= " << a << endl;
}
// 3、无参有返 
 int arr3() {
    cout << "arr3" << endl;
    return 400;
}
// 4、有参有返

 int arr4(int a) {
     cout << "arr4"<< endl;
     return a;
 }
int main()
{
    //1、无参无返
    arr01();
    // 2、有参无返
    arr2(100);
    // 3、无参有返 
    int num1 = arr3();
    cout << "num1=" << num1 << endl;
    // 4、有参有返
    int num2 = arr4(10000);
    cout << "num2=" <<num2 << endl;

    return 0;
}
```
## 48、函数声明
 - 作用；告诉编译器函数名称及如何调用函数，函数的实际主题可以单独定义
- 函数的声明可以多次，但是函数的定义只有一次
```c++
#include<iostream>
using namespace std;
//函数的声明
int maxs(int a, int b);

//声明可以多次写，定义只能有一次
//定义
int maxs(int a, int b)
{
    return  a > b ? a:b;
}

int main()
{
    int a = 19;
    int b = 33;
    cout <<"最大值为"<< maxs(a, b) << endl;

    return 0;
```
## 49、函数的分文件编写
作用；让代码结构更加清晰
- 1、创建点缀名为.h的头文件
- 2、创建点缀名为.cpp的源文件
 - 3、在头文件中写函数声明
- 4、在源文件中写函数的定义




## 50、指针的基本概念
- 指针的作用；可以通过指针间接访问内存
- 1、内存编号是从0开始记录的一般用十六进制数字表示
- 2、可以利用指针变量保存地址


## 51、指针变量的定义和使用
- 语法；数据类型 *变量名
```c++
#include <iostream>
using namespace std;

int main()
{//1、定义指针
	int a = 10;
	//指针的语法：数据类型*指针变量名；
	int * p;
	//让指针记录变量a的地址；
	p = &a;
	cout << "a的地址是； " << &a << endl;
	cout << "*p的地址为； " << p << endl;
	//2、使用指针
	//可以通过解引用的方式来找到指针指向的内存
	//指针前面加*代表解引，找到指针指向的内存中的数据
	*p = 1000;
	cout << "a=  " << a << endl;
	cout << "*p=  " << *p << endl;



	return 0;
}
```
## 52、` 指针所占内存`
```c++

#include <iostream>
using namespace std;

int main() {
	//指针所占内存
	int a = 10;
	//int* p;
	//p = &a;
	//可以写成
	int* p = &a;
	//在32位操作系统下，指针占4字节大小，不管什么数据类型
	//在64位操作系统下，指针占8字节大小
	cout << "sizeof (int *)=" << sizeof(int *) << endl;
	cout << "sizeof (int *)=" << sizeof(float *) << endl;
	cout << "sizeof (int *)=" << sizeof(double *) << endl;
	cout << "sizeof (int *)=" << sizeof(char *) << endl;
	return 0;
}
```
## 53、空指针和野指针
- 空指针：指针变量指向内存中为0的空间
- 用途：初始化指针变量
- 空指针指向的内存是不可以访问的
- 例如
```c++
#include <iostream>
using namespace std;

int main() {
	//空指针用于指针变量初始化
	int* p = NULL;
	//空指针是不能访问的
	//0~~255之间的内存编号是系统占用的，因此不可访问
	*p = 100;
	return 0;
}
```
## ` 野指针 `
- 指变量指向非法的内存空间
- 在程序中，尽量避免野指针因为会报错
- 总结：空指针和野指针都不是我们申请的空间，因此不要访问
 ##  54、const修饰指针
 - const修饰指针有三种情况
 - 1、const修饰指针————常量指针（指针指向可以改，但指向的值不能改
 - 2、const修饰常量————指针常量（指针的指向不可以改，指针指向的值可以改）
 - 3、const即修饰指针，又修饰常量（指针的指向和指针指向的值都不能改）
```c++
#include <iostream>
using namespace std;

int main() {
	//常量指针 const修饰指针
	int a = 10;
	int b = 10;
	const int* p = &a;
	//指针指向的值不能改，指针的指向可以改
	p = &b;
	//const 修饰常量  指针常量
	//指针的指向不可以改，但指向的值可以改
	int * const p2 = &a;
	*p2 = 100;
	//p2=&b;//错误的
	//const修饰指针和常量
	int a = 10;
	const int* const p3 = &a;
	//指针的指向和指向的值都不能改
	//*p=100;//错误
	//*p3=&b;//错误

	return 0;
}
```
## 55、指针和数组
- 作用：利用指针访问数组中的元素
```c++
int arr[10] = { 1,2,3,4,5,6,7,8,9,10 };
cout << "第一个元素" << arr[0] << endl;

int* p = arr;//arr就是数组的首地址
cout << "利用指针访问第一个元素" << *p << endl;
p++;//利用指针向后偏移四个字节

cout << "利用指针访问第二个元素" << *p << endl;
cout << "用指针遍历数组" << endl;
int* p2 = arr;
for (int i = 0;i < 10;i++) {
	cout << *p2<< endl;
	p2++;
}
```
## 56、指针和函数
- 利用指针做函数参数，可以修改实参的值
- 总结：如果不想修改实参，就用值传递，如果想修改实参，就用地址传递
```c++
#include <iostream>
using namespace std;
//实现两个数字交换
//值传递
void arr(int a, int b) {
	int temp = a;
	a = b;
	b = temp;
	cout << "a=" << a << endl;
	cout << "b=" << b << endl;
}
//地址传递
void arr1(int* p1, int* p2) {
	int temp = *p1;
	*p1 = *p2;
	*p2 = temp;
}


int main() {
	//指针函数 
	// 值传递
	int a = 10;
	int b = 20;
	arr(a, b);//值传递不会修改实参
	//如果是地址传递，可以修饰实参
	arr1(&a, &b);
	cout << "a=" << a << endl;
	cout << "b=" << b << endl;
	return 0;
}
```
## 57、指针配合数组和函数
```c++
#include <iostream>
using namespace std;
//冒泡排序函数 参数1  数据首地址 参数2 数组长度
void max(int* arr, int len)
{
	for (int i = 0;i < len;i++)
	{
		for (int j = 0;j < len - i - 1;j++)
		{
			//如果j>j+1的值，交换数据
			if (arr[j] > arr[j + 1]) {
				int temp = arr[j];
				arr[j] = arr[j + 1];
				arr[j + 1] = temp;
			}
		}
	}
}
//打印数组
void hr(int* arr, int len)
{
	for (int i = 0;i < len;i++)
	{
		cout << arr[i] << endl;
	}
}

int main() {
	//创建数组
	int arr[6] = { 5,2,6,1,3,4 };
	//数组长度
	int len = sizeof(arr) / sizeof(arr[0]);
//创建函数，实现冒泡排序
	max(arr, len);
	//打印排序后的数组
	hr(arr, len);

	return 0;
}
```
# `结构体` #
- 结构体属于用户自定义的数据类型，允许用户储存不同的数据类型
## 58、结构体的定义和使用
- 语法；struct 结构体名 {结构体成员列表}；
- 通过结构体创建变量的方式有三种：
- 1、struct 结构体名 变量名
- 2、struct 结构体名 变量名={成员1值，成员2值·····}
- 3、定义结构体时顺便创建变量 
- 总结1、定义结构体时的关键字是struct，不可以省略
- 总结2、创建结构体变量是，struct可以省略
- 总结3、结构体变量利用操作符号"."访问成员
```c++
#include <iostream>
using namespace std;
//1、创建学生数据类型：学生包括（姓名，年龄，成绩）
//自定义数据类型，一些类型集合组成的一个类型
//语法：struct 类型名称{成员列表}
struct student
{
	string name;
	int age;
	int score;
}s3;//顺便创造结构体变量

//2、通过学生类型创造出具体学生
//2.1 struct student s1
//2.2 struct student s2={.....}
//2.3 在定于结构体时顺便创建结构体变量

int main() {
	//2.1 struct student s1
	//struct在c++中可以省略
	struct student s1;
	//给s1属性赋值,通过.访问结构体变量中的属性
	s1.name = "张三";
	s1.age = 18;
	s1.score = 100;
	cout << "姓名" << s1.name << "年龄" << s1.age << "成绩" << s1.score << endl;
//2.2 struct student s2={.....}
	struct student s2 = { "里斯",19,80 };
	cout << "姓名" << s2.name << "年龄" << s2.age << "成绩" << s2.score << endl;
//2.3 在定于结构体时顺便创建结构体变量
	s3.name = "王五";
	s3.age = 21;
	s3.score = 80;
	cout << "姓名" << s3.name << "年龄" << s3.age << "成绩" << s3.score << endl;

	return 0;
}
```
## 59、结构体数组
- 作用；将自定义的结构体放入数组中维护
- 语法；struct 结构名 数组名{元素个素}={{ }，{ }，······{}}
```c++
#include <iostream>
using namespace std;
//定义结构体
struct student 
{    //姓名
	string name;
	//年龄
	int age;
		//分数
	int score;
};
int main() {
	//2、创建结构体数据
	struct student arr[3]
	{
		{"张三",19,10,},
		{"李四",18,390},
		{"王五",21,43}
	};
	//3、给结构体数组中的元素赋值
	arr[2].name = "as";
	arr[2].age = 19;
	arr[2].score = 322;
	//4、遍历结构体数组
	for (int i = 0;i < 3;i++)
	{
		cout << "姓名" << arr[i].name << "年龄" << arr[i].age << "成绩" << arr[i].score << endl;
	}


	return 0;
}
```
## 60、结构体指针
- 通过指针访问结构体中的成员
- 利用操作符` ->`可以通过结构体指针访问结构体属性
- 通过结构体指针 访问结构体中的属性，需要利用` ->`
```c++
#include <iostream>
using namespace std;
//定义结构体
struct max
{
	string name;
	int age;
	int score;
};
int main() 
{
	//1、创建学生结构体变量
	struct max s = { "张三",19,99 };
	//2、通过指针指向结构体变量
	struct max* p = &s;
	//3、通过指针访问结构体变量中的数据
	cout << "姓名" << p->name << "年龄" << p->age << "成绩" << p->score << endl;

	return 0;
}
```
## 61、嵌套结构体
- 作用：结构体中的成员可以是另一个结构体
```c++
struct studen
{
	string name;
	int age;
	int score;
};
struct teacher
{
	int id;
	string name;
	int aeg;
	struct studen stu;//嵌套结构需要在一个结构体中包含另一个文件的头文件
};
int main() 
{
	struct teacher a;
	a.name = "狼王";
	a.aeg = 45;
	a.id = 12323;

	a.stu.name = "小王";
	a.stu.age = 15;
	a.stu.score = 89;
	cout << "老师叫 " << a.name << "年纪 " << a.aeg << "id" << a.id << endl;
	cout << "学生叫 " << a.stu.name << "年纪" << a.stu.age << "成绩" << a.stu.score << endl;
	return 0;
}
```
## 62、结构体参数
- 作用：将结构体作为参数向函数中传递
- 传递的方式有
- 值传递
- 地址传递
- 总结：如果不想修饰函数中的数据，用值传递，反之用地址传递
```c++
#include <iostream>
using namespace std;
//定义学生结构体
struct studen
{
	string name;
	int age;
	int score;
};
//打印学生信息函数
//1、值传递
void printstudent1(struct studen a)
{
	
	cout << "子函数中姓名 " << a.name << "年纪 " << a.age << "分数" << a.score << endl;
};
//2、地址传递
void printstudent2(struct studen*p)
{
	cout << "子函数中姓名 " << p->name << "年纪" << p->age << "分数" << p->score << endl;
}
int main() 
{
	//创建结构体变量
	struct studen a;
	a.name = "厉陈";
	a.age = 19;
	a.score = 99;
	printstudent1(a);//值传递
	printstudent2(&a);//地址传递
//cout << "在main函数打印" << a.name << "年纪" << a.age << "成绩" << a.score << endl;

	return 0;
}
```
## 63、const使用场景
- 作用·：用const来防止误操作
```c++
void printstudent1(const struct studen* a)//用const防止误操作
{
	
	cout << "子函数中姓名 " << a->name << "年龄" << a->age << "成绩" << a->score << endl;
};
//2、地址传递

int main() 
{
	//创建结构体变量
	struct studen a;
	a.name = "厉陈";
	a.age = 19;
	a.score = 99;
	printstudent1(&a);

	return 0;
}
```
# 64、结构体案例

```c++
#include <iostream>
using namespace std;
#include<ctime>
//学生的结构体定义
struct student
{
	string  sname;
	int score;
	
 };
//老师的结构体定义
struct teacher
{   //姓名
	string tname;
	//学生数组
	struct student sarr[5];
};
//给老师和学生赋值的函数
void allocate(struct teacher tarr[],int len)
{
	string nameseed = "ABCDE";
	//给老师开始赋值
	for (int i = 0;i < len;i++) {
		tarr[i].tname = "teacher_";
		tarr[i].tname += nameseed[i];
		//通过循环给每名老师所带学生进行赋值
		for (int j = 0;j < 5;j++) 
		{
			tarr[i].sarr[j].sname = "student_";
			tarr[i].sarr[j].sname += nameseed[j];
			int random = rand() % 61+40;//40~100之间的随机数
			tarr[i].sarr[j].score = random;
		}
	}
}
//打印所有信息
void printlnfo(struct teacher tarr[], int len) {
	for (int i = 0;i < len;i++) {
		cout << "老师的姓名 " << tarr[i].tname << endl;
		for (int j = 0;j < 5;j++)
		{
			cout << "\t学生姓名" << tarr[i].sarr[j].sname <<
				"考试分数 "<<tarr[i].sarr[j].score<<endl;
		}
	}
}
int main() 
{
	//随机数种子
	srand((unsigned int)time(NULL));
	//1、创建三名老师的数组
	struct teacher tarr[3];
	//2、通过函数给3名老师的信息赋值，并给老师带的学生信息赋值
	int len = sizeof(tarr) / sizeof(tarr[0]);
	allocate(tarr, 3);
	//3、打印所有老师及所带学生信息赋值
	printlnfo(tarr, len);
	return 0;
}
```
## 65、通讯录管理系统——菜单功能
- 封装函数显示该界面
- 在main函数中调用封装好的函数

```c++
#include <iostream>
#include <string>
using namespace std;

#define MAX 1000//定义常量MAX,表示通讯录最大容量

// 联系人结构体
struct Contact//定义联系人数据结构，包含姓名、年龄、电话、住址 
{
    string name;   // 姓名
    int age;       // 年龄
    int sex;       // 性别
    string phone;  // 电话
    string addr;   // 住址
};

// 通讯录结构体
struct AddressBook//定义通讯录数据，包含一个固定大小的联系人数组和当前联系人数量
 {
    Contact contacts[MAX];  // 联系人数组
    int size;  // 当前记录的联系人个数
};
```
## 66、添加联系人
```c++
void asdf(addew*abs)//添加联系人
{
	if (abs->m_size == MAX)
	{
		cout << "通讯录满了，无法添加" << endl;
		return;
     }
	else
	{
		string name;
		cout << "请输入名字" << endl;
		cin >> name;
		abs->arr[abs->m_size].name = name;
		cout << "性别" << endl;
		cout << "1--男" << endl;
		cout << "2--女" << endl;
		int exa = 0;
		while(true)//作用是如果输入的是1.2可以退出循环，如果不是则重新输入
		{
			cin >> exa;
			if (exa == 1 || exa == 2)
			{
				abs->arr[abs->m_size].exa = exa;
				break;
			}
			cout << "输入有误请重新输入" << endl;
		}
	}
	cout << "请输入年龄" << endl;
	int age = 0;
	cin >> age;
	abs->arr[abs->m_size].age = age;

	cout << "请输入电话" << endl;
	string phone = 0;
	cin >> phone;
	abs->arr[abs->m_size].phone = phone;


	cout << "请输入地址" << endl;
	string addr = 0;
	cin >> addr;
	abs->arr[abs->m_size].addr = addr;
	//更新通讯录人数
	abs->m_size++;
	cout << "已添加成功" << endl;
	system("pause");//请按任意键继续
		system("cls");//清屏操作
}

```




## 67、显示联系人
- 设计联系人结构体
- 设计通讯录结构体
- 在main函数中创建通讯录
- 封装添加联系人函数
- 测试添加联系人功能

```c++
void shouers(addew*abs)//添加通讯录addew
{
	//判断通讯录中人数是否为0，如果是，提示记录为空
	//如果不为0，显示记录的联系人信息
	if (abs->m_size == 0)
	{
		cout << "记录为空" << endl;
	}
	else
	{
		for (int i = 0;i < abs->m_size;i++)
		{
			cout << "姓名" << abs->arr[i].name << "\t";
			cout << "性别" << (abs->arr[i].exa==1?"男":"女") << "\t";
			cout << "年龄" << abs->arr[i].age << "\t";
			cout << "电话" << abs->arr[i].phone << "\t";
			cout << "地址" << abs->arr[i].addr << endl;
		}
	}
	     system("pause");//按任意键继续
		 system("cls");//清屏
}

```



## 68、删除联系人
- 封装检测联系人是否存在
- 封装删除联系人函数
- 测试删除联系人功能
```c++
//3.1检测联系人是否存在，如果存在，返回联系人所在数组中位置，不存在返回-1
//参数1 通讯录 参数2对比姓名 
int isesist(addew *abs,string name)
{
	for (int i = 0;i < abs->m_size;i++)
	{
		//找到用户输入的姓名
		if (abs->arr[i].name == name)
		{
			return i;//找到了，返回这个人在数组中的下标编号
	       }
     }
	      return -1;//如果遍历结束都没有找到，返回-1
}
//3.2删除指定联系人
void deletepe(addew*abs)
{
	cout << "请输入您要删除的联系人" << endl;
	string name;
	cin >> name;
	//ret==-1 未查到  
	//ret!=-1 查到了
	int ret = isesist(abs, name);
	if (ret != -1)
	{
		//查到人，要进行删除操作
		for (int i = ret;i < abs->m_size;i++)
		{
			//数据前移
			abs->arr[i] = abs->arr[i + 1];
		}
		abs->m_size--;//更新通讯录中的人员数
		cout << "删除成功" << endl;
	}
	else
	{
		cout << "查无此人" << endl;
	}
	system("pause");
		system("cls");
}
```





## 69、查找联系人
- 封装查找联系人函数
- 测试查找指定联系人
```c++
void abcetepe(addew *abs)
{
	cout << "请输入您要查找的联系人" << endl;
	string name;
	cin >> name;
	//判断指定联系人是否存在通讯录中
	int ret=isesist(abs, name);
	if (ret != -1)//找到联系人
	{
		cout << "姓名" << abs->arr[ret].name << "\t";
		cout << "性别" << abs->arr[ret].exa << "\t";
		cout << "年龄" << abs->arr[ret].age << "\t";
		cout << "电话" << abs->arr[ret].phone << "\t";
		cout << "地址" << abs->arr[ret].addr << endl;
	}
	else//未找到联系人
	{
		cout << "查无此人" << endl;
	}
	//按任意键清屏
	system("pause");
		system("cls");
}
```




## 70、修改联系人
- 封装修改联系人函数
- 测试修改联系人功能
```c++
void modfyponre(addew *abs)
{
	cout << "请输入要修改的联系人" << endl;
	string name;
	cin >> name;
	int ret= isesist(abs, name);
	if (ret != -1)//找到指定联系人
	{
		string name;
		cout << "请输入姓名" << endl;
		cin >> name;
		abs->arr[ret].name = name;
		cout << "请输入性别" << endl;
		cout << "1--男" << endl;
		cout << "2--女" << endl;
		int exa = 0;
		while (true)
		{
			cin >> exa;
			if (exa == 1 || exa == 2)
			{
				//输入的正确 退出循环
				abs->arr[ret].exa = exa;
				break;
			}
			cout << "输入有误重新输入" << endl;
		}
		cout << "请输入年龄" << endl;
		int age = 0;
		cin >> age;
		abs->arr[ret].age = age;

		cout << "请输入联系电话" << endl;
		string phone = 0;
		cin >> phone;
		abs->arr[ret].phone = phone;

		cout << "请输入地址" << endl;
		string  addr = 0;
		cin >> addr;
		abs->arr[ret].addr = addr;
		cout << "修改成功" << endl;
	}
	else//未找到联系人
	{
		cout << "查无此人" << endl;
	}
	//按任意键清屏
	system("pause");
	system("cls");

}
```
## 71、清空联系人
- 封装清空联系人函数
- 测试清空联系人
```c++
void modfyponre(addew *abs)
{
	cout << "请输入要修改的联系人" << endl;
	string name;
	cin >> name;
	int ret= isesist(abs, name);
	if (ret != -1)//找到指定联系人
	{
		string name;
		cout << "请输入姓名" << endl;
		cin >> name;
		abs->arr[ret].name = name;
		cout << "请输入性别" << endl;
		cout << "1--男" << endl;
		cout << "2--女" << endl;
		int exa = 0;
		while (true)
		{
			cin >> exa;
			if (exa == 1 || exa == 2)
			{
				//输入的正确 退出循环
				abs->arr[ret].exa = exa;
				break;
			}
			cout << "输入有误重新输入" << endl;
		}
		cout << "请输入年龄" << endl;
		int age = 0;
		cin >> age;
		abs->arr[ret].age = age;

		cout << "请输入联系电话" << endl;
		string phone = 0;
		cin >> phone;
		abs->arr[ret].phone = phone;

		cout << "请输入地址" << endl;
		string  addr = 0;
		cin >> addr;
		abs->arr[ret].addr = addr;
		cout << "修改成功" << endl;
	}
	else//未找到联系人
	{
		cout << "查无此人" << endl;
	}
	//按任意键清屏
	system("pause");
	system("cls");

}
```




## 显示菜单
```c++
void showmend()
{
	cout << "*************************" << endl;
	cout << "***** 1、添加联系人 *****" << endl;
	cout << "***** 2、显示联系人 *****" << endl;
	cout << "***** 3、删除联系人 *****" << endl;
	cout << "***** 4、查找联系人 *****" << endl;
	cout << "***** 5、修改联系人 *****" << endl;
	cout << "***** 6、清空联系人 *****" << endl;
	cout << "***** 0、退出通讯录 *****" << endl;
	cout << "*************************" << endl;
}

int main()
{

	addew abs;//通讯录结构体变量
	abs.m_size = 0;//初始化当前人员个数

	while (true)
	{
		int arr = 0;
		cin >> arr;
		showmend();//利用地址传递可以修饰实参
		switch (arr)
		{
		case 1://1、添加联系人
			asdf(&abs);
			break;
		case 2://2、显示联系人
			shouers(&abs);
			break;
		case 3://3、删除联系人
			deletepe(&abs);
			break;
		case 4://4、查找联系人
		     abcetepe(&abs);
			break;
		case 5://5、修改联系人
			modfyponre(&abs);
			break;
		case 6://6、清空联系人
			cleanpom(&abs);
			break;
		case 0://退出
			cout << "欢迎下次使用" << endl;
			return 0;
			break;
		default:
			break;
		}
	}
		
	return 0;
}
```
# c++核心编程
- 主要针对c++面向编程技术做详细讲解，探讨c++中的核心和精髓
## 72、内存分区模型
- c++程序在进行时，讲内存大方向分为4个区域
- 代码区：存放函数的二进制代码，由操作系统进行管理
- 代码区：
- 1、存放cpu执行的机器指令
- 2、代码区是`共享`的，共享的目的是对于频繁被执行的程序，只需要在内存中有一份代码即可
- 3、代码区是`只读`的，使其只读的原因是防止程序意外的修改了它的指令
- 全局区：存放全局变量和静态变量以及常量
- 全局区：
- 1、全局变量和静态变量存放在此
- 2、全局区还包含 `常量区`，`字符串常量`和其他常量也存放在此
- 3、该区域的数据在程序结束后由系统操作释放
- 栈区：由编译器自动分配释放，存放函数的的参数值，局部变量等
- 堆区：由程序员分配释放，若程序员不释放，程序结束时由操作系统回收
- 内存四区存在的意义
- 不同区域存放的数据，赋予不同的生命周期，给我们更大的灵活编译

## 72、全局变量
- 总结：
- c++中在程序运行前分为全局区和代码区
- 代码区特点是共享和只读
- 全局区中存放全局变量、静态变量、常量
- 常量区中存放const修饰的全局常量和字符串常量
```c++
#include<iostream>
using namespace std;
//全局变量(不在main函数里面）

int m_a = 10;
int m_b = 20;
//const修饰的全局变量,全局的常量
const int s_n_a = 10;
const int  s_n_b = 10;
int main()
{
	//全局区
	
	//全局变量、静态变量、常量
	//创建一个普通的局部变量
	int a = 10;
	int b = 20;
	cout << "局部变量a的地址为： " << (int )& a << endl;
	cout << "局部变量b的地址为： " << (int)&b << endl;
	cout << "全部变量m_a的地址为： " << (int)&m_a << endl;
	cout << "全部变量m_b的地址为： " << (int)&m_b<< endl;
	//静态变量 在普通变量前面加static,属于静态变量
	static int s_a = 10;
	static int s_b = 10;
	cout << "静态变量s_a的地址为： " <<(int ) & s_a << endl;
	cout << "静态变量s_b的地址为： " << (int ) & s_b << endl;
	//常量
	//字符串常量
	cout << "字符串常量的地址为： " << (int)&"hello wored" << endl;
	
	//const修饰的变量
	 //const修饰的全局变量，const修饰的局部变量
	cout << "全局常量s_n_a的的地址为： " << (int)&s_n_a << endl;
	cout << "全局常量s_n_b的的地址为： " << (int)&s_n_b << endl;
	const int c_1_a = 10;//c-const g-global l-local
	const int c_1_b = 10;
	cout << "局部常量c_l_a的地址为： " << (int)&c_1_a << endl;
	cout << "局部常量c_l_b的地址为： " << (int)&c_1_b<< endl;

	return 0;
}
```
## 73、栈区
- 栈区：由编译器自动分配释放，存放函数的的参数值，局部变量等
- 注意：不要返回局部变量的地址，栈区开辟的数据由编译器自动释放
```c++
include<iostream>
using namespace std;
//栈区的注意事项--不要返回局部变量的地址
//栈区的数据由编译器管理开辟和释放
int* arrs(int b)//形参数据也会放到栈区
{
	b = 100;
	int a = 10;//局部变量 存放在栈区，栈区的数据在函数执行完后自动释放
	return &a;//返回局部变量地址
}
int main()
{
	int* p = arrs(1);//接受arrs函数的返回值
	cout << *p << endl;
	cout << *p << endl;

	return 0;
}
```
## 74、堆区
-  堆区：由程序员分配释放，若程序员不释放，程序结束时由操作系统回收
- c++中主要利用new在堆区开辟新空间
```c++
#include<iostream>
using namespace std;
int* arrs()
{
	//利用new关键字，可以将数据开辟到堆区
	//指针本质也是局部变量，放在栈上，指针保存的数据放在了堆区
    int *p = new int(10);
	return p;
}

int main()
{
	//在堆区开辟数据
	int* p = arrs();
	cout << *p << endl;
	
	return 0;
}
```
## 75、new操作符
- c++中主要利用new在堆区开辟新空间
- 堆区开辟的数据，由程序员手动开辟，手动释放，释放利用操作符`delete`
- 语法：new数据类型
- 利用new创建的数据，会返回该数据对应的类型指针
```c++
#include<iostream>
using namespace std;
//new的基本语法
int* arr()
{
	//在堆区创建一个整形的数据
	//new返回的是一个该数据类型的指针
	int *p = new int(10);
	return p;

}
void phone()
{
	int* p = arr();
	cout << *p << endl;
	//堆区的数据由程序员管理开辟，程序员管理释放
	//如果想释放堆区的数据，利用关键字delete
	delete p;
	//cout << *p << endl;//这块内存已经被释放了，再次访问就是非法操作会报错
}
//在堆区利用new开辟数组
void phone1()
{
	int* arr =new int[10];//10代表有10个元素
	for (int i = 0;i < 10;i++)
	{
		arr[i] = i + 100;//给10个元素赋值100~~109
	}
	for (int i = 0;i < 10;i++)
	{
		cout << arr[i] << endl;
	}
	//释放堆区的数组.
	//释放数组的时候要加【】
	delete [] arr;
}

int main()
{
	phone();
	phone1();
	return 0;
}
```
## 76、引用的基本使用
- 作用：给变量起别名
- 语法：数据类型&别名=原名
```c++
#include<iostream>
using namespace std;


int main()
{
	//引用的基本语法
	//数据类型 &别名=原名
	int a = 10;
	int& b = a;
	cout <<"a="<< a << endl;
	cout << "b=" << b << endl;
	b = 100;
	cout << "a=" << a << endl;
	cout << "b=" << b << endl;
}
```
## 77、引用的注意事项
- 引用必须初始化
- 引用一旦初始化后，就
不可改变
```c++
#include<iostream>
using namespace std;


int main()
{
	//引用必须初始化
	int a = 10;
	int& b = a;
	//int& c;错误，引用必须初始化
	//引用在初始化后，不可以修改.
	int c = 20;
	b = c;//赋值操作而不是引用
	cout << "a=" <<a<< endl;
	cout << "b=" <<b<< endl;
	cout << "c=" <<c<< endl;
}
```
## 78、引用函数参数
- 作用：函数传参时，可以利用引用的技术让形参修饰实参
- 优点：可以简化指针修改实参
- 总结：通过引用参数产生的效果同按地址传递是一样的。引用的语法更清楚简单
```c++
#include<iostream>
using namespace std;

//交换函数
//1、值传递
void phone1(int a ,int b)
{
	int temp = a;
	a = b;
	b = temp;
	/*cout << "phone1 a=" << a << endl;
	cout << "phone1 b=" << b << endl;*/
}
//2、地址传递
void phone2(int *a,int *b)
{
	int temp = *a;
	*a = *b;
	*b = temp;
}
//3、引用
void  phone3(int &a,int &b)
{
	int temp = a;
	a = b;
	b = temp;
}
int main()
{
	int a = 10;
	int b = 20;
	//phone1(a, b);//值传递，形参不会修饰实参
	//phone2(&a, &b);//地址传递，形参会修饰实参
	phone3(a, b);//引用传递，形参会修饰实参
	cout << "a=" << a << endl;
    cout << "b=" << b << endl;
	
}
```
## 79、引用做函数返回值
- 作用：应用是可以作为函数的返回值存在的
- 注意：不要返回局部变量
- 用法：函数调用作为左值
```c++
#include<iostream>
using namespace std;
//引用做函数的返回值
	//1、不要返回局部变量的引用
int& phnoe1()
{
	int a = 10;//局部变量存在四区中的栈区
	return a;
}
	//2、函数的调用可以作为左值
int& phone2()
{
	static int a = 10;//静态变量，存放在全局区，全局区的数据在程序结束后系统释放
	return a;
}

int main()
{
//	int &ref = phnoe1();
//	cout <<"ref = "<< ref << endl;//第一次结果正确是编译器做了保留
//	cout << "ref = " << ref << endl;//第二次错误是因为a的内存已经释放了
	int& ref2 = phone2();
	cout << "ref2 = " << ref2 << endl;
	phone2() = 1000;//如果函数的返回值是引用，这个函数的调用可以作为左值
	cout << "ref2 = " << ref2 << endl;
}
```
## 80、引用的本质
- 本质：引用的本质在c++内部是一个指针常量
- 结论：c++推荐引用计数，因为语法方便，引用本质是指针常量，但是所有的指针操作编译器都帮我们做了
```c++
#include<iostream>
using namespace std;
//发现是引用，转换为int *constref=a
void phone(int &ref)
{
	ref = 100;//ref是引用，转换为*ref=100
}
int main()
{
	int a = 10;
	//自当转换为int *constref=&a;指针常量是指针指向不可改，也说明为什么引用不可改
	int& ref = a;
	ref = 20;//内部发现ref是引用，自动帮我们转换为*ref=20;
	cout << "a= " << a << endl;
	cout << "ref= " << ref << endl;
	phone(a);

}
```
## 81、常量引用
- 作用：常量引用主要用来修饰形参，防止误操作
- 在函数列表中，可以加const修饰形参，防止形参改变实参
```c++
#include<iostream>
using namespace std;
//打印数据函数
void phone(const int &val)
{
	//val = 1000;
	cout << "val= " << val << endl;
}
int main()
{
	//常量引用
	//使用场景，用来修饰形参防止误操作
	//int a = 10;
	//加上const之后，编译器代码修改，int temp=10;int& ref=temp
	//const int& ref = a;//引用必须引一块合法的内存空间
	//ref = 20;//加入const之后改为只读不可修改
	int a = 100;
	cout << "a= " << a << endl;
	phone(a);

}
```
## 82、函数提高-函数默认参数
- 在c++中，函数的形参列表中的形参是可以有默认值的
- 语法：返回值类型 函数名 （参数=默认值）{}
```c++
#include<iostream>
using namespace std;
//函数的默认参数
//如果我们自己传入了数据，就用自己的数据，如果没有，用默认值
//语法：  返回值类型 函数名（形参=默认值）{}
int  phone(int b,int a=20,int c=30)
{
	return a + b + c;
}
//注意事项
//1、如果某个位置有默认参数，那么从这个位置往后，从左到右都必须有默认值
//int phone1(int a=10, int b, int c)
//{
//	return a + b + c;
//}
//2、如果函数声明有默认参数，函数的实现就不能有默认参数了
//声明和实现只能有一个有默认参数
int phone2(int a=10, int b=20);

int phone2(int a, int b)
{
	return a + b;
}
int main()
{
	//cout << phone(10) << endl;
	cout << phone2(10, 20) << endl;
	
}
```
## 83、函数占位参数
- c++中函数的形参列表里可以有占位参数，用来占位，调用函数时必须填补该位置
- 语法：返回值类型 函数名（数据类型）{}
- 在现阶段的函数占位参数意义不大，但是后面的课程中会用到该技术
```c++
#include<iostream>
using namespace std;
//占位参数
//返回值类型 函数名 （数据类型）{}
//目前阶段占位参数，我们还用不上，后边的课程中会用到
//占位参数 还可以有默认参数
void phone(int a,int)
{
	cout << "this is phone" << endl;
}
int main()
{
	phone(100,90);
}
```
# 函数重载
## 84、 函数重载
- 作用：函数名可以相同，提高复用性
- 函数重载满足条件
- 1、同一作用域下
- 2、函数名称相同
- 3、函数参数类型不同或者个数不同或者顺序不同
- 注意：函数的返回值不可以作为函数重载的条件
```c++
#include<iostream>
using namespace std;
//函数重载
//可以让函数名相同，提高函数复用性
//函数重载的条件
//1、必须在同一作用域下
//2、函数名称相同
//3、函数参数类型不同，或者个数不同，或者顺序不同
void phone()
{
	cout << "phone的调用" << endl;
}
void phone(int a)
{
	cout << "phon e(int a)的调用" << endl;
}
void phone(double a)
{
	cout << "phon e(double a)的调用" << endl;
}
void phone(int a, double b)
{
	cout << "phone(int a, double b)的调用" << endl;
}
void phone(double a, int b)
{
	cout << "phone(double a, int b)的调用" << endl;
}
//注意事项
//函数的返回值不可以作为函数重载的条件
//int  phone(double a, int b)
//{
//	cout << "phone(double a, int b)的调用" << endl;
//}
int main()
{
	//phone();
	//phone(10);
	//phone(3.14);
	//phone(10, 3.14);
	phone(3.14,10);
}
```
## 85、函数重载注意事项
- 引用作为重载条件
- 函数重载碰到函数默认参数
```c++
#include<iostream>
using namespace std;
//函数重载的注意事项
//1、引用作为重载条件
void phone(int &a)//int &a=10;不合法的
{
	cout << "phone(int&a)的调用" << endl;
}
void phone(const int& a)//const int&a=10;合法
{
	cout << "phone(const int& a)的调用" << endl;
}
//2、函数重载碰到默认参数
void phone1(int a)
{
	cout << "phone1(int a)调用" << endl;
}
void phone1(int a,int b=10)
{
	cout << "phone1(int a int b)调用" << endl;
}

int main()
{
	/*int a = 10;
     phone(a);*/
	//phone(10);
	//phone1(10);//当函数碰到默认参数，出现二义性，报错，尽量避免这种情况
}
```
# 类和对象
- c++面向对象的三大特性为；`封装` `继承` `多态`
- c++认为`万事万物都皆为对象` 对象上有其属性和行为
- 例如：人可以为对象，属性有姓名、年龄、身高、体重····行为有走、跑、跳、吃饭唱歌····
- 具有相同性质的`对象`，我们可以抽象称为`类`，人属于人类，车属于车类

## 86、封装
- 封装的意义
- 封装是c++面向对象的三大特征之一
- 封装的意义：
- 将属性和行为作为一个整体，表现生活中的事物
- 将属性和行为加以权限控制
- 封装意义一：
- 在设计类的时候，属性和行为写在一起，表现事物
- 语法：class 类名{访问权限：属性/行为};
```c++
const double PI = 3.14;
//设计一个圆类，求圆的周长
//圆求周长公式：2*pI*半径
//class代表设计一个类，类后面紧跟着的就是类名称
class yuan
{
	//访问权限
	//公共权限
public:
	//属性:
	//半径
	int m_r;
	//行为:
	//获取圆的周长
	double zhouchang()
	{
		return 2 * PI * m_r;
	}
};
int main()
{
	//通过一个圆类创建具体的圆（对象）
	//实例化（通过一个类 创建一个对象的过程）
	yuan c1;
	//给圆对象的属性进行赋值操作
	c1.m_r = 10;
	//2*PI*10=62.8
	cout << "圆的周长为；" << c1.zhouchang() << endl;
}
```
## 87、封装案例-设计学生
```c++
#include<iostream>
using namespace std;
//设计一个学生类，属性有姓名和学号
//可以给姓名和学号赋值，可以显示学生的姓名和学号
class students 
{
public://公共权限

	//类中的属性和行为 我们统一称为成员
	// 属性 成员属性 成员变量
	// 行为 成员函数 成员方法
	
	//属性
	string m_name;//姓名
	int m_id;//学号
	//行为
	//显示姓名和学号
	void student()
	{
		cout << "名字: " << m_name << "工作号: " << m_id << endl;
	}
	//给姓名赋值
	void stuname(string name)
	{
		m_name = name;
	 }
	void stuid(int id)
	{
		m_id = id;
	}
};

int main()
{
	//创建一个具体学生 实例化对象
	students s1;
	//给s1对象赋值
	//s1.m_name = "张三";
	s1.stuname("张三");
	//s1.m_id = 1;
	s1.stuid(54);
	//显示学生信息
	s1.student();

	students s2;
	s2.m_name = "李思";
	s2.m_id = 2;
	s2.student();
}
```
## 88、封装意义二
- 类在设计时，可以把属性和行为放在不同的权限下，加以控制
- 访问权限有三种：
- 1、public(公共访问)：成员 类内可以访问 类外也可以访问
- 2、protected(保护权限)：成员 类内可以访问 类外不可以访问：` 儿子也可以访问父亲中保护的内容`
- 3、private(私有权限)：成员 类内可以访问 类外不可以访问：`儿子不可访问父亲私有内容`
```c++
#include<iostream>
using namespace std;
class phone {
public:
	//公共权限
	string m_name;//姓名


	//保护权限
protected:
	string m_car;//汽车


	//私有权限
private:
	int m_pass;//银行卡


public://类内
	void phones()
	{
		m_name = "张三";
		m_car = "本田";
		m_pass = 12332;
	}

};
int main()
{
	phone s1;
	s1.m_name = "李四";
	//s1.car = "奔驰";//保护权限内容，在类外访问不到
	//s1.m_pass = 134224;//私有权限内容，类外访问不到
}
```
## 89、struct和class的区别
- 在c++中struct和class的唯一区别就在于默认访问权限不同
- 区别：struct默认权限为公共 、class默认权限为私有
```c++
#include<iostream>
using namespace std;
class c1
{
	int m_a;//默认私有权限
};
struct c2
{
	int m_b;//默认公共权限
};
int main()
{
	//struct和class区别
//struct 默认权限是 公共 public
//class 默认权限是 私有 private
	//c1 c1;
	//c1.m_a = 100;//class默认权限为私有，因此类外不可以访问

	c2 c2;//在stryct默认权限为公共，因此可以访问
	c2.m_b = 100;
}
```
## 90、成员属性设置为私有
- 优点1：将所有成员属性设置为私有，可以自己控制读写权限
- 优点2：对于写权限，我们可以检测数据有效性
```c++
#include<iostream>
using namespace std;
//人类
class perse
{
public:
	//设置姓名
	void satname(string name)
	{
		m_name = name;
	}
	//获取姓名
	string  getname()
	{
		return m_name;
	}
	//读取年龄
	int gteage()
	{
		return m_age;
	}
	//设置年龄
	void steage(int age)
	{
		if (age < 0 || age >= 150)
		{
			cout << "年龄有误" << endl;
			return;
		}
	}
	//设置偶像
	void steiod(string m_iod)
	{
		m_iod = m_iod;
	}
private:
	string m_name;//姓名 可读可写
	int m_age=18;//年龄 只读
	string  m_iod;//偶像 只写
};
int main()
{
	perse s;
	s.satname("张撒");
	//获取姓名
	cout << "姓名" << s.getname()<< endl;
	//年龄
	//s.satname(20);
	//s.m_age=20；
	cout << "年龄" << s.gteage()<< endl;
//偶像设置
	s.steiod("夏教");//只写
	//cout << "偶像" << s.steiod << endl;//只写状态外界访问不到
}
```
## 91、设计体案例
- 设计立方体类（cube）
- 求出立方体的面积和体积
- 分别用全局函数和成员函数判断两个立方体是否相等
```c++
#include<iostream>
using namespace std;
//立方体设计
//1、创建立方体
//2、设计属性和行为
//3、设计行为 获取立方体面积和体积
//4、分别利用全局函数和成员函数判断两个立方体是否相等
class cube
{
public:
	//设置长
	void setL(int l)
	{
		m_L = l;
	}
	//获取长
	int getL()
	{
		return m_L;
	}
	//设置宽
	void setW(int w)
	{
		m_W = w;
	}
	//获取宽
	int getW()
	{
		return m_W;
	}
	
	//设置高
	void setH(int h)
	{
		m_H = h;
	}
	//获取高
	int getH()
	{
		return m_H;
	}

	//获取立方体的面积
	int calculateS()
	{
		return 2 * m_L * m_W + 2 * m_W * m_H + 2 * m_L * m_H;
	}
	//获取立方体的体积
	int calculatesV()
	{
		return m_L * m_W * m_H;
	}
	//利用成员函数判断两个立方体是否相等
	bool issamebyclass(cube &c)//只需要传入一个立方体
	{
		if (m_L == c.getL() && m_W == c.getW() && m_H == c.getH())
		{
			return true;
	    }
		return false;
	}
private:
	int m_L;//长
	int m_W;//宽
	int m_H;//高

};
//利用全局函数判断两个立方体是否相等
bool issame(cube &c1,cube &c2)//需要传入两个立方体
{
	if (c1.getL() == c2.getL() && c1.getW() == c2.getW() && c1.getH() == c2.getH())
	{
		return true;
     }
	return false;
}


int main()
{
	//创建立方体对象
	cube c1;
	c1.setL(10);
	c1.setW(10);
	c1.setH(10);
	cout << "c1的面积为：  " << c1.calculateS() << endl;
	cout << "c1的体积为：  " << c1.calculatesV() << endl;
	//创建第2个立方体
	cube c2;
	
		c2.setL(10);
		c2.setW(10);
		c2.setH(10);
		//利用全局函数判断
	bool ret=issame(c1, c2);
	if (ret)
	{
		cout << "c1和c2相等" << endl;
	}
	else
	{
		cout << "c1和c2不相等" << endl;
	}
	//利用成员函数判断
	ret = c1.issamebyclass(c2);
	if (ret)
	{
		cout << "成员函数判断结果c1和c2相等" << endl;
	}
	else
	{
		cout << "成员函数判断结果c1和c2不相等" << endl;
	}
}
```
## 92、设计案例2(重点)
- 设计一个圆类（circle),和一个点类（point).计算点和圆的关系
```c++
#include<iostream>
using namespace std;

//点和圆关系案例
// 点类
class point
{
public:
	//设置x坐标
	void setx(int x)
	{
		m_x = x;
	}
	//获取x坐标
	int getx()
	{
		return m_x;
	}
	//设置y坐标
	void sety(int y)
	{
		m_y = y;
	}
	//获取y坐标
	int gety()
	{
		return m_y;
	}

private:
	int m_x;
	int m_y;
};
//圆类
class circle
{
public:

	//设置半径
	void setR(int r)
	{
		m_R = r;
	}
	//获取半径
	int getR()
	{
		return m_R;
	}
	//设置圆心
	void setcenter(point center)
	{
		m_center = center;
	}
	//获取圆心
	point getcenter()
	{
		return m_center;
	}
private:

	int m_R;//半径
	//在类中可以让另一个类 作为本来中的成员/——|
	point m_center;//圆心
};
//判断点和圆的关系
void islncircle(circle &c,point&p)
{
	//计算两点之间距离 平方
	int distance =
		(c.getcenter().getx() - p.getx()) * (c.getcenter().getx() - p.getx())
		+ (c.getcenter().gety() - p.gety()) * (c.getcenter().gety() - p.gety());
	//计算半径平方
	int rdistaance = c.getR() * c.getR();
	//判断关系
	if (distance == rdistaance)
	{
		cout << "点在圆上" << endl;
	}
	else if (distance > rdistaance)
	{
		cout << "点不在圆上" << endl;
	}
	else
	{
		cout << "点在圆内" << endl;
	}
}
int main()
{
	//创建圆
	circle c;
	c.setR(10);
	point center;
	center.setx(10);
	center.sety(0);
    c.setcenter(center);
	//创建点
	point p;
	p.setx(10);
	p.sety(10);
	//判断关系
	islncircle(c, p);
	return 0;
}
```
# 对象函数-构造函数和析构函数
## 对象的初始化和清理
- 生活中我们买的电子产品都基本会出场设置 在某一天我们不用时候也会删除一些自己信息数据保证安全
- c++中的面向对象来源于生活，每个对象也会有初始化设置以及对象销毁前的清理数据的设置
## 93、构造函数和析构函数
- 对象的初始化和清理也是两个非常重要的安全问题
- 一个对象或者变量没有初始状态，对其使用后果是未知
- 同样的使用完一个对象和变量 没有及时清理，也会造成一定的安全问题
- c++利用了构造函数和析构函数解决上述问题，这两个函数将会被编译器自动调用，完成对象初始化和清理工作。对象的初始化和清理工作是编译器强制要求我们做的事，因此如果我们不提供构造和析构，编译器会提供编译器提供的构造函数和析构函数是空间
- 构造函数：主要作用于创建对象时为对象的成员属性赋值，构造函数由编译器自动调用，无需手动调用
- 析构函数：主要作用在于对象销毁前系统自动调用，执行一些清理工作
- ### 构造函数语法：类名（）{}
- 1、构造函数，没有返回值也不写void
- 2、函数名称和类名相同
- 3、构造函数可以有参数，因此可以发生重载
- 4、程序在调用对象时候会自动调用构造，无需手动调用，而且只会调用一次
- ### 析构函数语法：~类名（）{}
- 1、析构函数，没有返回值也不写void
- 2、函数名称与类名相同，在名称前加上符号~
- 3、析构函数不可以有参数，因此不可发生重载
- 4、程序在对象销毁前会自动调用析构，无需手动调用，而且只会调用一次
```c++
#include<iostream>
using namespace std;
class phone
{
public:
	//构造函数没有返回值不用写void
	//构造函数可以有参数 可以发生重载
	//创建对象的时候，构造函数会自动调用，而且只会调用一次
	phone()//函数名与类名相同
	{
		cout << "构造函数phone" << endl;
	}


	//析构函数
	//没有返回值不写void
	//函数名和类名相同在名称前加~符号
	//析构函数不可以有参数，不可以发生重载
	//对象在销毁前，会自动调用析构函数，而且只会调用一次
	~phone()
	{
		cout << "析构函数phone" << endl;
	}
};
//构造和析构都是必须有的实现，如果我们自己不写编译器会提供一个空实现的构造和析构
void parr()
{
	phone p;//在栈上的数据，parr运行完了后就会释放这个对象
}
int main()
{
	parr();
	
}
```
## 94、构造函数的分类及调用
- ### 两种分类方式
- 按参数分为：有参构造和无参构造
- 按类型分为：普通构造和拷贝构造
- ### 三中调用方式
- 括号法
- 显示法
- 隐式转换法
```c++
#include<iostream>
using namespace std;
class phone
{
public:
	
	phone()//无参构造函数 也是默认构造函数
	{
		cout << "无参构造函数phone" << endl;
	}
	phone(int a)//有参构造函数
	{
		age = a;
		cout << "有参构造函数" << endl;
		
	}
	phone(const phone &p)//拷贝构造函数
	{
		cout << "拷贝构造函数" << endl;
		age = p.age;
	}
	
	~phone()//析构函数
	{
		cout << "析构函数phone" << endl;
	}
	int age;
};
//调用
void arrf()
{
	//括号法
	//phone p;//默认构造函数调用
	//phone p2(10);//有参构造函数
	//拷贝构造函数调用
	//phone p3(p2);

	//注意事项
	//调用默认构造函数时不要加（）
	// 因为下面这行代码，编译器会认为是一个函数的声明,不会认为在创建对象
	//phone p();
	 
	
	//cout << "p3= " << p3.age << endl;
	
	
	//显示法
	//phone p1;
	//phone p2 = phone(10);//有参构造
	//phone p3 = phone(p2);//拷贝构造

	//phone(10);//匿名对象 特点：当前行执行完后，系统会立马回收匿名对象

	//注意事项2 
	//不要利用拷贝函数初始化 匿名对象 编译器会认为phone（p3）==phone p3;对象声明
	//phone(p3);


	//隐式转换法
	phone p4 = 10;//相当于写了 phone p4==phone(10);有参构造
	//拷贝构造
	phone p5 = p4;
}
int main()
{
	arrf();
	
}
```
## 95、拷贝构造函数调用时机
- ### c++中构造函数调用时机有三种情况
- 使用一个已经创建完毕的对象来初始化一个新对象
- 值传递的方式给函数参数传值
- 以值方式返回局部数据
```c++
#include<iostream>
using namespace std;
//拷贝构造函数调用时机
//1、使用一个已经创建完毕的对象来初始化一个新对象
//2、值传递的方式给函数参数传值
//3、值方式返回局部对象
class phone
{
public:
	phone()
	{
		cout << "默认构造函数调用" << endl;
	}
	phone(int age)
	{
		cout << "有参构造函数调用" << endl;
		m_age = age;
	}
	phone(const phone & p)
	{
		cout << "拷贝构造函数调用" << endl;
		m_age = p.m_age;
	}
	~phone()
	{
		cout << "析构函数调用" << endl;
	}
	int m_age;
};
//拷贝构造函数调用时机
//1、使用一个已经创建完毕的对象来初始化一个新对象
void arrf()
{
	phone p1(20);
	phone p2(p1);
	cout << "p2的年龄为：" << p2 .m_age<< endl;
}
//2、值传递的方式给函数参数传值
void duwor(phone p)
{

}
void arrf2()
{
	phone p;
	duwor(p);
}
//3、值方式返回局部对象
phone duwor2()
{
	phone p1;
	cout << (int*)&p1 << endl;
	return p1;
}
void arrf3()
{
	phone p = duwor2();
	cout << (int*)&p << endl;
}

int main()
{
	//arrf();
	//arrf2();
	arrf3();

	return 0;
}
```
## 96、构造函数调用规则
- ### 默认情况下，c++编译器至少给一个类添加3个函数
- 1、默认构造函数（无参，函数体为空）
- 2、默认析构函数（无参，函数体为空）
- 3、默认拷贝构造函数，对属性进行值拷贝
- ### 构造函数调用规则如下
- 如果用户定义有参构造函数，c++不在提供默认无参构造，但是会提供默认拷贝构造
- 如果用户定义拷贝构造函数，c++不会在提供其他构造函数
- 总结：如果属性有在堆区开辟的，一定要自己提供拷贝构造函数，防止浅拷贝带来问题
```c++
#include<iostream>
using namespace std;
//创建函数的调用规则
//1、创建一个类，c++编译器会给每个类都添加至少三个函数
//默认构造（空实现）
//析构函数（空实现）
//拷贝函数（值拷贝）
// 
//2、如果我们写了有参构造函数，编译器不在提供默认构造，依然提供拷贝构造
//如果我们写了拷贝构造函数，编译器就不会提供其他普通构造函数
class phone
{
public:
	phone()
	{
		cout << "默认构造函数调用" << endl;
	}
	phone(int age)
	{
		m_age = age;
		cout << "有参构造函数调用" << endl;
	}
	phone(const phone &p)
	{
		m_age = p.m_age;
		cout << "拷贝构造函数调用" << endl;
	}
	~phone()
	{
		cout << "析构函数调用" << endl;
	}
	int m_age;
};
void arrf()
{
	phone p;
	p.m_age = 19;
	phone p2(p);
	cout << "p2=" << p.m_age << endl;
}
void arrf1()
{
	phone p(19);
	phone p2(p);
	cout << "p2=" <<p.m_age<< endl;
}
int main()
{
	//arrf();
	arrf1();
	return 0;
}
```
## 97、深拷贝和浅拷贝
- 深浅拷贝是面试经典问题，也是常见的一个坑
- 浅拷贝：简单的赋值拷贝操作
- 深拷贝：在堆区重新申请空间，进行拷贝操作
```c++
#include<iostream>
using namespace std;
//深拷贝与浅拷贝
class phone
{
public:

	phone()
	{
		cout << "默认构造函数调用" << endl;
	}
	phone(int age,int height)
	{
		m_age = age;
		m_height = new int(height);
		cout << "有参构造函数调用" << endl;
	}
	//自己实现拷贝构造函数，解决浅拷贝带来的问题
	phone(const phone &p)
	{
		cout << "拷贝函数的调用" << endl;
		m_age = p.m_age;
		//m_height = p.m_height;编译器默认实现的就是这行代码
		//深拷贝操作

		m_height = new int(*p.m_height);
	}
	~phone()
	{
		//析构代码，将堆区开辟的数据做释放操作
		if (m_height != NULL)
		{
			delete m_height;
			m_height = NULL;
		}
		cout << "析构函数调用" << endl;
	}
	int m_age;//年龄
	int *m_height;//身高
};
void arrf()
{
	phone p1(17,199);
	cout << "p1的年龄" <<p1.m_age<<"身高为； "<<*p1.m_height<< endl;
	phone p2(p1);
	cout << "p2的年龄" << p2.m_age << "身高为； " << *p2.m_height << endl;
}
int main()
{
	arrf();
}
```
## 98、初始化列表
- 作用：c++提供了初始化列表语法，用来初始化属性
- 语法：构造函数（）：属性1（值1），属性2（值2）·····{}
```c++
#include<iostream>
using namespace std;
//初始化列表
class phone
{
public:

	//传统初始化操作
	//phone(int a,int b,int c)
	//{
		//m_a = a;
		//m_b = b;
		//m_c = c;
	//}
	//初始化列表初始化属性
	phone(int a,int b,int c):m_a(a), m_b(b), m_c(c)
	{

	}
	int m_a;
	int m_b;
	int m_c;
};
void arrf()
{
	//phone p(10,20,30);
	phone p(30, 40, 10);
	cout << "m_a= " << p.m_a << endl;
	cout << "m_b= " << p.m_b << endl;
	cout << "m_c= " << p.m_c << endl;
}
int main()
{
	arrf();
}
```
## 99、类对象作为类成员
- c++类中的成员可以是另一个类的对象，我们可以抽象称为称该成员为对象成员
- 示例：
```c++
class A{}
class B
{
	A a;
}
```
- B类中有对象A作为成员，A为成员对象
- 那么当创建对象时，A与B的构造和析构的顺序谁先谁后
```c++
#include<iostream>
using namespace std;
//类对象作为类成员
//手机类
class phone
{
public:
	phone(string pname)
	{
		cout << "phone的构造函数调用" << endl;
		m_pname = pname;
	}
	//手机品牌名称
	string m_pname;
};
//人类
class persn
{
public:
	persn(string name,string pname):m_name(name),m_phone(pname)//phone m_phone=pname 隐式转换法
	{
		cout << "persn的函数调用" << endl;
	}
	~persn()
	{
		cout << "persn的析构函数调用" << endl;
	}

	//姓名
	string m_name;
	//手机
	phone m_phone;
};
//当其他类对象作为本类成员，构造时候先构造类对象，在构造自身，析构的顺序相反
void arrf()
{
	persn p("炸弹", "华为40");
	cout << p.m_name << "拿着" << p.m_phone.m_pname  << endl;
}
int main()
{
	arrf();
}
```
## 100、静态成员
- 静态成员就是在成员变量和成员函数前加上关键字static,称为静态成员
### 静态成员分为：
#### 静态成员变量
- 所有对象共享同一份数据
- 在编译阶段分配内存
- 类内声明，类外初始化
```c++
#include<iostream>
using namespace std;
class phone
{
public:
	//1、所有对象都共享一份数据
	//2、编译阶段就分配内存
	//3、类内声明，类外初始化
	static int m_a;
	//静态成员变量也是有访问权限的
	private:
		static int m_b;

};
int phone::m_b = 3232;
int phone:: m_a=100;
void arrf()
{
	phone p;
	
	cout << p.m_a << endl;

	phone p2;
	p2.m_a = 200;
	cout << p2.m_a << endl;
}
void arrf2()
{
	//静态成员变量 不属于某个对象上，所有对象都同享一份数据
	//因此静态成员变量有两种访问方式
	//1、通过对象进行访问
	 phone p;
	 cout << p.m_a << endl;
	//2、通过类名进行访问
	 cout << phone::m_a << endl;
	// cout << phone::m_b << endl;类外访问不到私有静态成员变量
}
int main()
{
	//arrf();
	arrf2();
}
```
#### 静态成员函数
- 所有对象共享同一个函数
- 静态成员函数只能访问静态成员变量
```c++
#include<iostream>
using namespace std;
//静态成员函数
// 所有对象共享同一个函数
//静态成员函数只能访问静态成员变量
class phone
{
public:
	//静态成员函数
	static void arrf()
	{
		m_A = 100;//静态成员函数可以访问静态的成员变量
		//m_B= 200;//静态成员函数不可以访问非静态成员变量，无法区分到底是哪个对象
		cout << "static void arrf的调用" << endl;
	}
	static int  m_A;//静态成员变量
	int m_B;//非静态成员变量
	//静态成员函数也是有访问权限的
private:
	static void arrf3()
	{
		cout << "static void arrf3的调用" << endl;
	}
};
int phone::m_A = 0;
//两种访问方式
void test01()
{
//1、通过对象访问
	phone p;
	p.arrf();
	//2、通过类名访问
	phone::arrf();
	//phone::arrf3();类外访问不到私有静态成员函数
}
int main()
{
	test01();
}
```
## 类和对象特征-c++对象模型和this指针
## 101、成员变量和成员函数分开存储
- 在c++中，类内的成员变量和成员函数分开存储
- 只有非静态成员才属于类的对象上
```c++
#include<iostream>
using namespace std;
//成员变量和成员函数分开存储
class phone
{
public:
	int m_A;//非静态成员变量 属于类的对象上
	static int m_b;//静态成员变量 不属于类对象上
	void arr(){}//非静态成员函数 不属于类对象上
	static void arr1(){}//静态成员变量 不属于类对象上


};
int phone::m_b;
void arrf()
{
	phone p;
	//空对象占用内存为；1
	//c++编译器会给每个空对象也分配一个字节空间，是为了区分空对象占内存位置
	//每个空对象也应该有一个独一无二的内存地址
	cout << "sizeof p的内存; " << sizeof(p) << endl;
}
void arrf1()
{
	phone p;
	cout << "sizeof p的内存; " << sizeof(p) << endl;
}

int main()
{
	//arrf();
	arrf1()ti;
	return 0;
}
```
## 102、this指针概念
- c++中的成员变量和成员函数是分开存储的
- 每一个非静态成员函数只会诞生一份函数实例，也就是说多个同类型的对象会共用一块代码。那么问题是：这一块代码如何区分那个对象会调用自己？
- c++通过提供特殊的对象指针，this指针，解决上述问题，``this指针指向被调用的成员函数所属的对象``
- this指针是隐含每一个非静态成员函数内的一种指针
- this指针不需要定义，直接使用即可
#### this指针的用途：
- 当形参和成员变量同名时，可用this指针来区分
- 在类的非静态成员函数中返回对象本身，可用`return*this`
```c++
#include<iostream>
using namespace std;
class phone
{
	public:

	phone(int age)
	{
		//this指针指向 被调用的成员函数 所属对象
		 this->age = age;
	}
	phone &phones(phone &p)
	{
		this->age += p.age;
		return *this;//this 指向p2的指针，而*this指向的就是p2这个对象的本体
	}
	int age;
};
//1、解决名称冲突
void arrf()
{
	phone p1(90);
	cout << "p1= " << p1.age << endl;

}
//2、返回对象本身用*this
void arrf1()
{
	phone p1(92);
	phone p2(92);
	//链式编程思想
	p2.phones(p1).phones(p1).phones(p1).phones(p1);

	cout << "p2= " << p2.age << endl;
}
int main()
{
	//arrf();
	arrf1();
	return 0;
}
```
## 103、空指针访问成员函数
- c++中空指针也可以调用成员函数的，但是也要注意有没有用到this指针
- 如果用到this指针，需要加以判断保证代码的健壮性
```c++
#include<iostream>
using namespace std;
class phone
{
public:
	void phonename()
	{
		cout << "phone name" << endl;
	}
	void phoneAge()
	{
		if (this == NULL)
		{
			return;
		}
		cout << "phoneAge" <<this->Age<< endl;//报错原因是传入的指针为NULL
	}
	int Age;
};
void arrf()
{
	phone* p = NULL;
	p->phonename();
	p->phoneAge();

}
int main()
{
	arrf();
	return 0;
}
```
## 104、const 修饰成员函数
#### 常函数
- 成员函数后加const后我们称为这个函数为`常函数`
- 常函数内不可以修改成员属性
- 成员属性声明时加关键字`mutable`后在常函数中依然可以修改
#### 常对象
- 声明对象前加`const`称该对象为常对象
- 常对象只能调用函数
```c++
#include <iostream>
using namespace std;
//常函数
class phone
{
public:
	//this指针的本质 是指针常量指针的指向是不可以修改的
	//const phone *const this;
	//在成员函数后面加const，修饰的是this指向，让指针指向的值也不可以修改
	void arrf() const

	{
		//this->m_a = 100;
		//this=NULL;//this是不可以修改指针指向的
		this->m_b = 100;
	}
	//void func()
	//{

	//}
	int m_a;
	mutable int m_b;//特殊变量，即使在常函数中，也可以修改这个值,加关键字mutable
	
};
void arrf1()
{
	phone p;
	p.arrf();

}
//常对象
void arrf2()
{
	const phone p;//在对象前加上const，变为常对象
	//p.m_a = 100;
	p.m_b = 100;//m_b是特殊值，在常对象下也可以修改
	//常对象只能调用常函数
	p.arrf();
	//p.func();常对象 不可以调用普通成员函数，因为普通成员函数可以修改属性
}
int main()
{

	return 0;
}
```
## 105、友元
- 生活中你的家有客厅（public）卧室（private）客厅所有人都可以进去卧室是私有的，只有你能进去，但是你也允许你的好朋友进去
- 在重新里，有些私有的属性也想让类外特殊的一些函数或者类访问，就需要友元技术
#### 友元的关键字`friend`
#### 友元的三种实现
- 全局函数做友元
- 类做友元
- 成员函数做友元
```c++
#include <iostream>
using namespace std;

// 建筑
class libai
{
    // goodgai全局函数是libai的好朋友，可以访问libai中的私有成员
    friend void goodgay(libai* libai);

public:
    libai()
    {
        keting = "客厅";
       woshi1 = "卧室";
    }

public:
    string keting;

private:
    string woshi1;
};

// 全局函数
void goodgay(libai* libai)
{
    cout << "好基友的全局函数正在访问： " << libai->keting << endl;
    cout << "好基友的全局函数正在访问： " << libai->woshi1 << endl;
}

void arrf()
{
    libai libai;
    goodgay(&libai);
}

int main()
{
    arrf();
    return 0;
}
```
## 106、类做友元
```c++
#include <iostream>
using namespace std;
//类做友元
class Building;
class goodgay
{
public:
	goodgay();


	void canguan();//参观函数访问Building中的属性
	
	Building* building;
};
class  Building
{
	//goodgay是本类的好朋友，可以访问本类中私有成员
	friend class goodgay;
public:
	Building();
public:
	string m_keting;//客厅
private:
	string m_woshi;//卧室
};
//类外写成员函数
Building::Building()
{
	m_keting = "客厅";
	m_woshi = "卧室";
}
goodgay::goodgay()
{
	//创建建筑物
	building = new Building;
}
void goodgay::canguan()
{
	cout << "好基友类正在访问；" << building->m_keting << endl;
	cout << "好基友类正在访问；" << building->m_woshi << endl;
}
void arrf()
{
	goodgay gg;
	gg.canguan();

}
int main()
{
	arrf();
}
```
## 107、成员函数做友元
```c++
#include<iostream>
using namespace std;
class Buding;
class goodgay
{
public:
	goodgay();
	void visit();//让visit函数可以访问Building中的私有成员
	void visst2();//让visit2访问不到Building中的私有成员
	Buding* buding;


};
class Buding
{
	//告诉编译器good gay类下的visst成员函数作为类的朋友可以访问私有成员
	friend void goodgay::visit();
public:
	Buding();
	
public:
	string m_keting;//客厅
private:
	string m_woshi;//卧室

};
//类外实现成员函数
Buding::Buding()
{
	m_keting = "客厅";
	m_woshi = "卧室";
}
goodgay::goodgay()
{
	buding = new Buding;
}
void goodgay::visit()
{
	cout << "visst函数正在访问； " << buding->m_keting << endl;
	cout << "visst函数正在访问； " << buding->m_woshi << endl;
}
void goodgay::visst2()
{
	cout << "visst2函数正在访问； " << buding->m_keting << endl;
	//cout << "visst2函数正在访问； " << buding->m_woshi << endl;
}
void arrf1()
{
	goodgay gg;
	gg.visit();
	gg.visst2();
}
int main()
{

	arrf1();
	return 0;
}
```
# 运算符重载
- 运算符重载概念：对已有的运算符重新进行定义，赋予其另外一种功能，以适应不同的数据类型
## 108、加号运算符重载
- 作用：实现两个自定义数据类型相加的运算
- 总结1：对于内置的数据类型的表达式的运算符是不可能改变的
- 总结2：不要滥用运算符重载
```c++
#include<iostream>
using namespace std;
class phone
{
public:
	//1、成员函数重载+号
	/*phone operator+ (phone&p)
	{
		phone temp;
		temp.m_A = this->m_A + p.m_A;
		temp.m_B = this->m_B + p.m_B;
		return temp;
	}*/
	int m_A;
	int m_B;
};


//2、全局函数重载+号
phone operator+ (phone& p1, phone& p2)
{
	phone temp;
	temp.m_A = p1.m_A + p2.m_A;
	temp.m_B = p1.m_B + p2.m_B;
	return temp;
}

//3、函数重载的版本
phone operator+(phone& p1, int num)
{

	phone temp;
	temp.m_A = p1.m_A + num;
	temp.m_B = p1.m_B + num;
	return temp;
}
void arrf()
{
	phone p1;
	p1.m_A = 10;
	p1.m_B = 10;
	phone p2;
	p2.m_A = 10;
	p2.m_B = 10;
	//成员函数本质的调用
	//phone p3 = p1.operator +(p2);
	// 全局函数重载的调用
	//phone p3= operator+(p1,p2);

	phone p3 = p1 + p2;

	//运算符重载，也可以发生函数重载
	phone p4 = p1 + 100;//phone +int 

	cout << "p3= " << p3.m_A<< endl;
	cout << "p3= " << p3.m_B<< endl;

	cout << "p4= " << p4.m_A << endl;
	cout << "p4= " << p4.m_B << endl;
}

int main()
{

	arrf();
}
```
## 109、左移运算符重载
- 作用：可以输出自定义数据类型
- 总结：重载左移动运算符配合友元可以实现输出自定义数据类型
- 核心代码： ostream& operator<<(ostream&cout ,phone& p)
 

```c++
#include<iostream>
using namespace std;
class phone
{
	friend ostream& operator<<(ostream& cout, phone& p);
    //（访问私有权限的方式）

public:
	phone(int a, int b)
	{
		m_A = a;
		 m_B = b;
	}
private:
	//利用成员函数重载 左移运算符  p.operator<<(cout)   简化版P<<cout
	/*void operator <<(cout)
	{

	}*/
	int m_A;
	int m_B;

};
//只能利用全局函数重载左移运算符
ostream& operator<<(ostream&cout ,phone& p)//本质  operator<<(cout,p)  简化cout<<p
{
	cout << "m_A" << p.m_A << " m_B" << p.m_B << endl;
	return cout;
}

void arrf()
{
	phone p(10,40);
	
	cout << p << endl;
}
int main()
{
	arrf();
	return 0;
}
```
## 110、递增运算符重载
- 作用：通过重载递增运算符，实现自己的整形数据
- 总结：前置递增要返回引用`&`在写`operator++`
- 后置递增返回的是值要加`int`
```c++
#include<iostream>
using namespace std;
//重载递增运算符

//自定义的整形
class phone
{
	friend	ostream& operator<<(ostream& cout, phone myint);
public:
	phone()
	{
		m_num = 0;
	}
	//重载前置++运算符  返回引用为了一直对一个数据进行递增
    phone &operator++()
	{
		//先进行++运算
		m_num++;
		//再将自身做返回
		return *this;
	}
	//重载后置++运算符
	//int 代表占位参数，可以用于区分前置和后置递增
	phone  operator++(int)
	{

		//先 记j录当时结果
		phone temp = *this;
		//后递增
		m_num++;
		//最后将结果返回
		return temp;
	}
private:
	int m_num;

};
//重载<<运算符
ostream& operator<<(ostream& cout,phone myint)
{
	cout << myint.m_num;
	return cout;
}
void arrf()
{
	phone myint;
	cout << ++myint << endl;
}
void arrf2()
{
	phone myint;
	cout << myint++ << endl;
	cout << myint << endl;

}
int main()
{
	//arrf();
		arrf2();
	return 0;
}
```
## 111、赋值运算符重载
- c++编译器至少给一个类添加4个函数
- 1、默认构造参数（无参，函数体为空）
- 2、默认析构函数（无参，函数体为空）
- 3、默认拷贝构造函数，对属性进行值拷贝
- 4、赋值运算符operator=，对属性进行值拷贝
- 如果类中有属性指向堆区，做赋值操作时也会出现深浅拷贝问题
```c++
#include<iostream>
using namespace std;
//赋值运算符重载
class phone
{
public:
	phone(int age)
	{
		m_age = new int(age);
	}
	~phone()
	{
		if (m_age != NULL)
		{
			delete m_age;
			m_age = NULL;
		}
	}
	//重载 赋值运算符
	phone& operator=(phone&p)
	{
		//编译器都是通过浅拷贝
		//m_age = p.m_age;
		//应该先判断是否有属性在堆区，如果有先释放干净，让后在深拷贝
		if (m_age != NULL)
		{
			delete m_age;
			m_age = NULL;
		}
		m_age=new int(*p.m_age);//深拷贝操作
		//返回对象本身
		return *this;
	}

	int *m_age;
};
void arrf()
{
	phone p1(19);
	phone p2(18);
	phone p3(30);
	p3= p2 = p1;//赋值操作
	cout <<"p1年龄为；"<< *p1.m_age << endl;
	cout << "p2年龄为；" << *p2.m_age << endl;
	cout << "p3年龄为；" << *p3.m_age << endl;
}

int main()
{
	arrf();
	/*int a = 10;
	int b = 20;
	int c = 30;
	c = b = a;
	cout << "a= " << a << endl;
	cout << "b= " << b << endl;
	cout << "c= " << c << endl;*/
	return 0;
}
```
## 112、关系运算符
- 作用：重载关系运算符。可以让两个自定义类型对象进行对比操作
```c++
#include<iostream>
using namespace std;
//操作关系运算符
class phone
{
public:
	phone(string nae, int age)
	{
		m_name = nae;
		m_age = age;
	}
	//重载==
	bool operator==(phone& p)
	{
		if (this->m_name == p.m_name && this->m_age == p.m_age)
		{
			return true;
		}
		return false;
	}
	bool operator!=(phone& p)
	{
		if (this->m_name == p.m_name && this->m_age == p.m_age)
		{
			return false;
		}
		return true;
	}
	string m_name;
	int m_age;
};
void arrf()
{
	phone p1("撒洒", 19);
	phone p2("流浪者", 19);
	if (p1 == p2)
	{
		cout << "p1 p2相等" << endl;
	}
	else
	{
		cout << "p1 p2不相等" << endl;
	}

	if (p1 != p2)
	{
		cout << "p1 p2是不相等" << endl;
	}
	else
	{
		cout << "p1 p2是相等" << endl;
	}

}
int main()
{
	arrf();

	return 0;
}
```
## 113、函数调用运算符重载
- 函数调用运算符（）也可以重载
- 由于重载后使用的方式非常像函数的调用，因此称为仿函数
- 仿函数没有固定写法，非常灵活
```c++
#include <iostream>
using namespace std;
//函数调用运算符重载
//打印输出类
class Myprint
{
public:
	//重载函数调用运算符
	void operator()(string test)
	{
		cout << test << endl;
	}
};
void Myprint02(string test)
{
	cout << test << endl;
}
void test01()
{
	Myprint myprint;
	myprint("hello world");//
	Myprint02("hello world");//由于使用起来非常类似函数调用，所以我们称为仿函数
}

//仿函数非常灵活，没有固定写法
//加法类
class Myadd
{
public:
	int operator()(int num1, int num2)
	{

		return num1 + num2;
	}
};
void tesst02()
{
	Myadd myagg;
	int ret= myagg(100, 100);
	cout << ret << endl;
	//匿名对象
	cout << Myadd()(100, 100) << endl;
}
int main()
{
	//test01();
	tesst02();
	return 0;
}
```
## 114、继承
#### 继承是面向对象三大特征之一
- 如动物分猫狗。猫有（加菲猫，波斯猫、、、、）狗有（哈士奇，牧羊犬、、、）定义这些类时，下级别成员除了拥有上一级别共性，还有自己的特性
- 这时候我们就可以考虑利用继承技术，减少代码重复性
- 语法：class 子类：继承方式(public) 父类
- 例如：class Java :public gonggongyemian
```c++
#include<iostream>
using namespace std;
//用继承实现网页

class gonggongyemian//公共页面
{
public:
	void dingbu()
	{
		cout << "首页,公开课,登录,注册....(等等)"<< endl;
	}
	void dibu()
	{
		cout << "帮助中心,交流合作，站内地图...(等等)" << endl;
	}
	void zuobian()
	{
		cout << "Java,Pathon,c++...(等等)" << endl;
	}

};
//Java页面
class Java :public gonggongyemian
{
public:
    void content()
	{
			cout << "Java学科" << endl;
	}
};
//Python页面
class python :public gonggongyemian
{
public:
	void content()
	{
		cout << "python学科" << endl;
	}
};
//c++页面
class cpp :public gonggongyemian
{
public:
	void content()
	{
		cout << "cpp学科" << endl;
	}
	//继承的好处：减少代码重复
	//语法：class 子类:继承方式 父类
	//子类 也称为 派生类
	//父类 也称为 基类
};
void arrf()
{
	cout << "Java下载视频页面如下" << endl;
	Java ja;
	ja.dingbu();
	ja.dibu();
	ja.zuobian();

	cout << "-------------------------" << endl;
	cout << "python下载视频页面如下" << endl;
	python py;
	py.dingbu();
	py.dibu();
	py.zuobian();

	cout << "-------------------------" << endl;
	cout << "c++下载视频页面如下" << endl;
	cpp cpp;
	ja.dingbu();
	ja.dibu();
	ja.zuobian();

}
int main()
{
	arrf();
}
```
## 115、继承方式
- 语法：class 子类：继承方式 父类
- 有三种继承方式
- 1、公共继承
- 2、保护继承
- 3、私有继承
```c++
#include<iostream>
using namespace std;

class gong
{
public:
	int M_a;
protected:
	int M_b;
private:
	int M_c;

};
class son:public gong
{
	void arr()
	{
		 M_a = 10;//父类中的公共权限成员 到子类中依然是公共权限
		 M_b = 10;//父类中的保护权限成员 到子类中依然是保护权限
		// M_c = 10;//父类中的私有权限成员 子类访问不到
	}
};
void arrf()
{
	son s;
	s.M_a = 100;
	//s.M_b = 100;//到son中M_b是保护权限类外访问不到
}
//保护继承
class gong2
{
public:
	int M_a;
protected:
	int M_b;
private:
	int M_c;

};
class son2:protected gong2
{
public:
	void  arrf2()
	{
		M_a = 100;//父类中的公共成员，到子类中变为保护权限
		M_b = 100;//父类中保护权限成员，到子类中变为保护权限
		//M_c = 100;//父类中私有成员 子类访问不到
	}

};
void arrf2()
{
	son2 s1;
	//s1.M_a = 1000;//在son2中M_a变为保护权限，因此类外访问不到
	//s1.M_b = 2222;//在son2中M_b变为保护权限，因此类外访问不到
}
//私有继承
class gong3
{
	public:
public:
	int M_a;
protected:
	int M_b;
private:
	int M_c;

};
class son3 :private gong3
{
public:
	void arrf3()
	{
		M_a - 100;//父类中的公共成员，到子类中变为私有成员
		M_b = 100;//父类中的保护成员，到子类中变为私有成员
		//M_c = 100;//父类中私有成员 子类访问不到
	}
};
void arrf3()
{
	son3 s1;
	//s1.M_a = 1000;//到son3中 变为私有成员 类外访问不到
	//s1.M_b = 1000;//到son3中 变为私有成员 类外访问不到
}
int main()
{


	return 0;
}
```
## 116、继承中的对象模型
- 利用开发人员命令查看对象模型
- 跳转盘符   F：
- 跳转文件路径 cd 具体路径下
- 查看命名
- Cl /d1 reportSingleClassLayout类名 文件名
- 总结：父类中私有成员属性，是被编译器隐藏了的，因此访问不到，但是确实被继承下去了
```c++
#include<iostream>
using namespace std;
class gong
{
public:
	int M_a;
protected:
	int M_b;
private:
	int M_c;

};
class song :public gong
{
public:
	int M_d;
};
//利用开发人员命令查看对象模型
//跳转盘符   F：
//跳转文件路径 cd 具体路径下
//查看命名
//Cl /d1 reportSingleClassLayout类名 文件名
void arrf()
{
	//父类中所有非静态成员都会被子类继承下去
	//父类中私有成员属性，是被编译器隐藏了的，因此访问不到，但是确实被继承下去了
	cout << "song=" << sizeof(song) << endl;
}
int main()
{
	arrf();

	return 0;
}
```
## 117、继承中的构造和析构顺序
- 子类继承父类后，当创建子类对象，也会定义父类构造函数
- 问题：父类和子类的构造函数和析构函数谁先谁后？
- 总结：先构造父类，在构造子类  析构是先构造子类在构造父类
```c++
#include<iostream>
using namespace std;
class fu
{
public:
	fu()
	{
		cout << "fu类中的构造函数" << endl;
	}
	~fu()
	{
		cout << "fu类中的析构函数" << endl;
	}

};
class son :public fu
{
public:
	son()
	{
		cout << "son类中的构造函数" << endl;
	}

	~son()
	{
		cout << "son类中的析构函数" << endl;
	}
};
void arrf()
{
	//fu f;
	//继承中的构造和析构顺序如下
	//先构造父类，在构造子类  析构是先构造子类在构造父类
	son s;
}
int main()
{
	arrf();
}
```
## 118、继承同名成员处理方式
- 访问子类同名成员，直接访问即可
- 访问父类同名成员，需要加作用域
- 总结：当子类与父类拥有同名成员函数时，子类会隐藏父类中同名成员函数，加作用域可以访问到父类中同名函数
- 问题：当子类和父类出现同名成员，如何通过子类成员，访问到子类或父类中同名数据呢？
```c++
#include<iostream>
using namespace std;
//继承中同名成员处理
class fu
{
public:
	fu()
	{
		M_a = 100;
	}
	void func()
	{
		cout << "fu-func()调用" << endl;
	}
	
	void func(int a)
	{
		cout << "fu-func(int a)调用" << endl;
	}
	int M_a;
};
class son :public fu
{
public:
	son()
	{
		M_a = 200;
	}
	void func()
	{
		cout << "son-func()调用" << endl;
	}
	int M_a;
};
void arrf()
{
	son s;
	cout << "son 下 M_a= " << s.M_a << endl;
	//如果通过子类对象  访问到父类中的成员需要加作用域
	cout << "fu 下 M_a= " << s.fu::M_a << endl;
}
//同名成员函数处理
void arrf2()
{
	son s;
	s.func();//直接调用 调用子类中的同名成员
	//如何调用父类中同名成员？隐藏的同名成员函数，需要加作用域
	s.fu::func();
	//如果子类中出现了和父类同名的成员函数，子类的同名成员会隐藏父类中所有的同名成员函数
	//如果想访问父类中
	s.fu::func(100);
}
int main()
{
	//arrf();
	arrf2();
}
```
## 119、继承同名静态成员的处理方式
- 访问子类同名成员，直接访问即可
- 访问父类同名成员，需要加作用域
- 静态成员同名和非静态成员同名处理方式一样
- 子类出现了和父类同名静态成员函数，也会隐藏父类中所有同名成员函数
- 如果想访问父类中被隐藏同名成员，需要加作用域
- `son;;fu::func();`
- 继承中同名的静态成员在子类对象上如何访问？
```c++
#include<iostream>
using namespace std;
//继承中同名静态成员处理
class fu
{
public:
	static int M_A;
	static void func()
	{
		cout << "fu-static void func()" << endl;
	}
	static void func(int a)
	{
		cout << "fu-static void func(int a)" << endl;
	}
};
int fu::M_A=100;
class son :public fu
{
public:
	static int M_A;
	static void func()
	{
		cout << "son-static void func()" << endl;
	}
};
int son::M_A =200;
//同名的静态成员属性
void arrf()
{
	//1、通过对象访问
	cout << "通过对象访问" << endl;
	son s;
	cout << "son M_a= " <<s.M_A<< endl;
	cout << "fu M_a= " << s.fu::M_A << endl;

	//2、通过类名访问
	cout << "通过类名访问" << endl;
	cout << "son 下 M_A= " << son::M_A << endl;
	//第一个 ::代表通过类名方式来访问  第二个 ::代表访问父类的作用域下
	cout << "fu 下 M_A= " << son::fu::M_A << endl;
}
//同名静态成员函数
void arrf2()
{
	//1、通过对象访问
	cout << "通过对象访问" << endl;
	son s;
	s.func();
	s.fu::func();
	//2、通过类名访问
	cout << "通过类名访问" << endl;
	son::func();
	son;;fu::func();

	//子类出现了和父类同名静态成员函数，也会隐藏父类中所有同名成员函数
	//如果想访问父类中被隐藏同名成员，需要加作用域
	son::fu::func(100);
};
int main()
{
	//arrf();
	arrf2();
}
```
## 120、多继承语法
- c++允许一个类继承多个类
- 语法：class 子类:继承方式 父类，继承方式 父类
- 多继承可能引发父类中有同名的出现，需要加作用域区分
- 多继承中父类出现了同名的情况，子类要加作用域
#### c++实际开发中不建议用多继承
```c++
#include<iostream>
using namespace std;
class fu1
{
public:
	fu1()
	{
		 M_A = 100;
	}
	int M_A;
};
class fu2
{
public:
	fu2()
	{
		 M_A = 200;
	}
	int M_A;
};
//子类需要继承fu1和fu
//语法 class 子类:继承方式 父类1，继承方式 父类2
class son :public fu1, public fu2
{
public:
	son()
	{
		 M_C = 300;
		 M_D = 400;
	}
	int M_C;
	int M_D;
};
void arrf()
{
	son s;
	cout << "sizeof son= " << sizeof(s) << endl;
	//当父类中出现同名的成员，需要加作用域
	cout << "fu1M_A= " << s.fu1::M_A << endl;
	cout << "fu2M_A= " << s.fu2::M_A << endl;
}
int main()
{
	arrf();
}
```
## 121、菱形继承
#### 菱形继承概念：
- 两个派生类继承同一个基类
- 又有某个类同时继承两个派生类
- 这种继承被称为菱形继承，或者钻石继承
#### 总结：
- 继承前加关键字  `virtual`
- dongwu类称为 虚基类 当发生虚继承了之后这份数据只有一份了
```c++
#include<iostream>
using namespace std;
//动物类
class dongwu
{
public:
	int M_age;
};
//利用虚继承 解决菱形继承问题
//继承前加关键字  virtual
//dongwu类称为 虚基类 当发生虚继承了之后这份数据只有一份了
//羊类
class yang :virtual public dongwu{};

//驼类
class tuo:virtual public dongwu{};

//羊驼类
class yangtuo:public yang,public tuo{};

void arrf()
{
	yangtuo yt;
	yt.yang::M_age = 18;
	yt.tuo::M_age = 28;
	//当菱形继承，两个父类拥有相同的数据，需要加作用域区分
	cout << "yt.yang::M_age= " << yt.yang::M_age << endl;
	cout << "yt.yuo::M_age= " << yt.tuo::M_age << endl;
	//这份数据我们知道 只有一份就够了，菱形继承导致数据有两份资源浪费

}
int main()
{
	arrf();

	return 0;
}
```
# 多态
## 多态是c++面向对象的三大特性之一
## 122、多态的基本概念
#### 多态分为两种：
- 静态多态：函数重载和运算符重载属于静态多态，复用函数名
- 动态多态：派生类和虚函数实现运行时多态
- 动态多态满足条件
- 1、有继承关系
- 2、子类重写父类的虚函数
- 3、重写:  函数返回值类型 函数名 参数列表 完全相同
- 动态多态的调用
- 1、父类的指针或引用  指向子类对象
#### 静态多态和动态多态的区别
- 静态多态的函数地址早绑定，编译阶段确定函数地址
- 动态多态的函数地址晚绑定，运行阶段确定函数地址
```c++
#include <iostream>
using namespace std;
//动物类
class Dongwu
{
public:
	virtual void shuohua()//虚函数
	{
		cout << "动物说话" << endl;
	}

};
//猫
class Mao :public Dongwu
{
public:
	//重写  函数返回值类型 函数名 参数列表 完全相同
	//子类中的 virtaul可写可不写
	virtual void shuohua()
	{
		cout << "猫说话" << endl;
	}
};
//狗
class Gou:public Dongwu
{
public:
	void shuohua()
	{
		cout << "狗说话" << endl;
	}
};
//执行说话的函数
//地址早绑定 在编译阶段绑定函数地址
//如果想让猫说话，这个函数就不能提前绑定，要在运行阶段进行绑定，晚绑定

//动态多态满足条件
//1、有继承关系
//2、子类重写父类的虚函数


//动态多态的调用
//1、父类的指针或引用  指向子类对象
void Shuohua(Dongwu&dongwu)//Dongwu&dongwu=mao
{
	dongwu.shuohua();
}
void arrf()
{
	Mao mao;
	Shuohua(mao);

	Gou gou;
	Shuohua(gou);
}
int main()
{
	arrf();
	return 0;
}
```
## 123、多态案例1-计算类
- 案例描述：
分别利用普通写法和多态技术，设计实现两个操作数进行运算的计算器类
- 优点：
- 1、代码组织结构清晰
- 2、可读性强
- 总结：c++开发提倡利用多态设计程序架构，因为多态优点很多
```c++
#include<iostream>
using namespace std;
//普通实现
class Calcullator
{
public:
	int  getResult(string oper)
	{
		if (oper == "+")
		{
			return M_num1 + M_num2;
		}
		else if (oper == "-")
		{
			return M_num1 - M_num2;
		}
		else if (oper == "*")
		{
			return M_num1 * M_num2;
		}
		//如果想拓展新的功能。需要修改源码
		//在真实开发中 提倡 开闭原则
		//开闭原则，对扩展进行开放，对修改进行关闭
	}
	int M_num1;//操作数1
	int M_num2;//操作数2

};
void test01()
{
	//创建计算器对象
	Calcullator c;
	c.M_num1 = 10;
	c.M_num2 = 10;

	cout << c.M_num1 << "+" << c.M_num2 << "=" << c.getResult("+") << endl;
	cout << c.M_num1 << "-" << c.M_num2 << "=" << c.getResult("-") << endl;
	cout << c.M_num1 << "*" << c.M_num2 << "=" << c.getResult("*") << endl;

}
//多态实现
//多态好处：
// 1、组织结构清晰
// 2、可读性强
// 3、对于前期和后期扩展以及维护性高
//实现计算器的抽象类

class chouxiangCalcullator
{
public:
	virtual int  getResult()
	{
		return 0;
	}
	int m_Num1;
	int m_Num2;

};
//加法计算器类
class jiafa:public  chouxiangCalcullator
{
public:
	virtual int  getResult()
	{
		return m_Num1+m_Num2;
	}
};
//减法计算器类
class jianfa :public  chouxiangCalcullator
{
	public:
		virtual int  getResult()
		{
			return m_Num1 - m_Num2;
		}
};
//乘法计算器
class chengfa :public  chouxiangCalcullator
{
public:
	virtual int  getResult()
	{
		return m_Num1 * m_Num2;
	}
};
void test02()
{
	//多态使用条件
	//父类指针或引用指向子类对象
	//加法
	chouxiangCalcullator* abc = new jiafa;
	abc->m_Num1 = 100;
	abc->m_Num2 = 100;

	cout << abc->m_Num1 << "+" << abc->m_Num2 << "=" << abc->getResult() << endl;
	//用完后释放
	delete abc;
	//减法运算
	abc = new jianfa;
	abc->m_Num1 = 100;
	abc->m_Num2 = 100;
	cout << abc->m_Num1 << "-" << abc->m_Num2 << "=" << abc->getResult() << endl;
	delete abc;

	//乘法
	abc = new chengfa;
	abc->m_Num1 = 100;
	abc->m_Num2 = 100;
	cout << abc->m_Num1 << "*" << abc->m_Num2 << "=" << abc->getResult() << endl;
	delete abc;
}
int main()
{

	test02();
	return 0;
}
```
## 124、纯虚函数和抽象类
- 在多态中，通常父类中虚函数的实现毫无意义的，主要是调用子类中的重写的内容
- 因此可以将虚函数改为`纯虚函数`
- 纯虚函数语法：`virtual 返回值类型 函数名 （参数列表）=0；`
- 当类中有了纯虚函数，这个类也称为`抽类`
#### 抽象类特点：
- 无法实例化对象
- 子类必须重写抽象类中的纯虚函数，否则也属于抽象类
```c++
#include<iostream>
using namespace std;
//纯虚函数
class Gonggong
{
public:
	//纯虚函数
	//只要有一个纯虚函数这个类就是抽象类
	//抽象类特点：
	//1、无法实例化对象
	//2、抽象类子类必须重写父类纯虚函数，否则也为抽象类
	virtual void song() = 0;

};
class son:public Gonggong
{
public:
	virtual void song() 
	{
		cout << "son的调用" << endl;
	};


};
void arrf()
{
	//gonggong g;//抽象类无法实例化对象
	//new gonggong;//抽象类无法实例化对象
	//son s;//子类必须重写父类中的纯虚函数，否则无法实例化对象
	//s.song();
	Gonggong* gonggong = new son;
	gonggong->song();


}
int main()
{
	arrf();

	return 0;
}
```
## 125、多态-案例2-制作饮品
- 制作饮品流程为：煮水-冲泡-倒入杯中-加入辅料
- 利用多态技术实现本案例，提供抽象制作饮品基类，提供子类制作咖啡和茶
```c++
#include<iostream>
using namespace std;
//制作饮品

class Yingping
{
public:
	virtual void zhushui() = 0;//煮水
	virtual void chongpao() = 0;//冲泡
	virtual void daorubeizhong() = 0;//倒入杯中
	virtual void jiarufuliao() = 0;//加入辅料

	void zhizuo()
	{
		zhushui();
		chongpao();
		daorubeizhong();
		jiarufuliao();
	}
};
//制作咖啡
class Kafei :public Yingping
{
	public:
		virtual void zhushui()
		{
			cout << "煮农夫山泉水" << endl;
		}
		virtual void chongpao()
		{
			cout << "冲泡" << endl;
		}
		virtual void daorubeizhong()
		{
			cout << "倒入杯子" << endl;
		}
		virtual void jiarufuliao()
		{
			cout << "加入糖和牛奶" << endl;
		}
};
//制作茶叶
class Cha :public Yingping
{
public:
	virtual void zhushui()
	{
		cout << "煮矿泉水水" << endl;
	}
	virtual void chongpao()
	{
		cout << "冲泡茶叶" << endl;
	}
	virtual void daorubeizhong()
	{
		cout << "倒入茶杯" << endl;
	}
	virtual void jiarufuliao()
	{
		cout << "加入柠檬" << endl;
	}
};
//制作函数
void Dowurk(Yingping*abc)//Yingping*abc=new kafei
{
	abc->zhizuo();
	delete abc;//释放
}
void arrf()
{
	Dowurk(new Kafei);//制作咖啡
	cout << "---------------" << endl;
	Dowurk(new Cha);

}
int main()
{
	arrf();

	return 0;
}
```
## 126、虚析构和纯虚析构
- 多态使用时，如果子类中有属性开辟到堆区，那么父类指针在释放时无法调用到子类的析构代码
- 解决方法：将父类中的析构函数改为`虚析构`或者`纯虚析构`
#### 虚析构和纯虚析构共性
- 可以解决父类指针释放子类对象
- 都需要具体的函数实现
#### 虚析构和纯虚析构区别
- 如果时纯虚析构，该类属于抽象类，无法实现实例化
- 虚析构语法：virtual~类名(){};
- 纯虚析构语法：virtual ~类名()=0;
- 类名::~类名(){};
- 总结：1、`虚析构或纯虚析构就是用来解决父类指针释放子类对象`
- 2、`如果子类中没有堆区数据，可以不写虚析构或纯虚析构`
- 3.`拥有纯虚析构函数的类也属于抽象类`
```c++
#include<iostream>
using namespace std;
class Dongwu
{
public:
	Dongwu()
	{
		cout << "Dongwu的构造函数" << endl;
	}
	//利用虚析构可以解决 父类指针释放子类对象时不干净的问题
	/*virtual ~Dongwu()
	{
		cout << "Dongwu的虚析构函数" << endl;
	}*/

	//纯虚析构   需要声明也需要实现
	//有了纯虚析构之后，这个类也属于抽象类，无法实例化对象
	virtual ~Dongwu() = 0;
	//纯虚函数
	virtual void sepk() = 0;

};
Dongwu:: ~Dongwu() 
{
	cout << "Dongwu的纯虚析构函数" << endl;

};


class Cat :public Dongwu
{
public:
	Cat(string name)
	{
		cout << "Cat的构造函数" << endl;
		m_Name= new string(name);
	}
	virtual void sepk()
	{
		cout <<*m_Name<< "小猫在说话" << endl;
	}
	~Cat()
	{
		if (m_Name != NULL)
		{
			cout << "Cat的析构函数" << endl;
			delete m_Name;
			m_Name = NULL;
}
	}

	string *m_Name;

};
void arrf()
{
	Dongwu* dongwu = new Cat("Tom");
	dongwu->sepk();
	//父类指针在析构时候，不会调用子类中的析构函数，导致子类如果有堆区属性，出现内存泄露
	delete dongwu;
}
int main()
{
	arrf();
	return 0;
}
```
## 127 、多态案例3-电脑组装
- 电脑组成部件为cpu（用于计算），显卡（用于显示），内存条（用于储存）
- 将每个零件封装出抽象基类，并且提供不同的厂商生产不同的零件，例如lntel厂商和enovo厂商
- 创建电脑类提供让电脑工作的函数，并且调用每个零件工作的接口
- 测试时组装三台不同的电脑进行工作
```c++
#include<iostream>
using namespace std;
//抽象不同零件类
//抽象cpu类
class Cpu
{
public:
	//抽象的计算函数
	virtual void calculate() = 0;
};
//抽象显卡类
class Videocard
{
public:
	//抽象的显示函数
	virtual void display() = 0;
};
//抽象内存条
class Memory
{
public:
	//抽象的存储函数
	virtual void storage() = 0;
};
//电脑类
class Computer
{
public:
	Computer(Cpu* cpu, Videocard* vc, Memory* mem)
	{
		m_cpu = cpu;
		m_vc = vc;
		m_mem = mem;
	}
	//提供工作的函数
	void work()
	{
		//让零件工作起来，调用接口
		m_cpu->calculate();

		m_vc->display();

		m_mem->storage();
	}
	//提供析构函数 释放3个电脑的零件
	~Computer()
	{
		//释放cpu零件
		if (m_cpu != NULL)
		{
			delete m_cpu;
			m_cpu = NULL;
		}
		//释放显卡零件
		if (m_vc != NULL)
		{
			delete m_vc;
			m_vc = NULL;
		}
		//释放内存条零件
		if (m_mem!= NULL)
		{
			delete m_mem;
			m_mem = NULL;
		}
	}
private:
	Cpu* m_cpu;//cpu的零件指针
	Videocard* m_vc;//显卡零件指针
	Memory* m_mem;//内存条零件指针
};
//具体厂商
//Intel厂商
class IntelCpu :public Cpu
{
public:
	virtual void calculate()
	{
		cout << "Intel的cpu开始计算" << endl;
	}
};
class IntelVidepcard :public Videocard
{
public:
	virtual void display()
	{
		cout << "Intel的显卡开始显示" << endl;
	}
};
class IntelMemory :public Memory
{
public:
	virtual void storage()
	{
		cout << "Intel的内存条开始存储" << endl;
	}
};

//lenovo
class lenovoCpu :public Cpu
{
public:
	virtual void calculate()
	{
		cout << "lenovo的cpu开始计算" << endl;
	}
};
class lenovoVidepcard :public Videocard
{
public:
	virtual void display()
	{
		cout << "lenovo的显卡开始显示" << endl;
	}
};
class lenovoMemory :public Memory
{
public:
	virtual void storage()
	{
		cout << "lenovo的内存条开始存储" << endl;
	}
};
void arrf()
{
	//第一台电脑的零件
	Cpu* intelCpu = new IntelCpu;
	Videocard* intelCard = new IntelVidepcard;
	Memory* intelmem = new IntelMemory;
	//创建第一台电脑
	Computer* computer1 = new Computer(intelCpu, intelCard, intelmem);
	computer1->work();
	delete computer1;

	cout << "---------------" << endl;
	cout << "第二台电脑开始工作" << endl;
	//第二台电脑组装
	Computer* computer2 = new Computer(new lenovoCpu,new lenovoVidepcard,new lenovoMemory);
	computer2->work();
	delete computer2;

	cout << "---------------" << endl;
	cout << "第三台电脑开始工作" << endl;
	//第三台电脑组装
	Computer* computer3 = new Computer(new lenovoCpu, new IntelVidepcard, new lenovoMemory);
	computer3->work();
	delete computer3;
}
int main()
{
	arrf();

	return 0;
}
```
# 文件操作
- 程序运行时的数据都属于临时数据，程序一旦运行结束都会被释放
- 通过`文件可以将数据持久化`
- c++中对文件操作需要包含头文件`<fstream>`
#### 文件类型分为两种
- 1、文本文件 -文件以文本的`ASCII`码形式存储在计算机中
- 2、二进制文件 -文件以文本的二进制形式存储在计算机中，用户一般不能直接读懂它们
#### 操作文件三大类
- 1、ofstream:写操作
- 2、ifstream:读操作
- 3、fstream:读写操作
## 128、写文件
- 步骤：
- 1、包含头文件`#include<fstream>`
- 2、创建流对象`ofstream ofs;`
- 3、打开文件`ofs.open("文件路径"，打开方式);`
- 4、写数据`ofs<<"写入数据;"`
- 5、关闭文件
#### 文件打开方式
- ios::in(为读文件而打开文件)
- ios::out(为写文件而打开文件)
- ios::ate(初始位置，文件尾)
- ios::app(追加方式写文件)
- ios::trunc(如果文件存在先删除，后创建)
- ios::binary(二进制方式)
- 注意：文件打开方式可以配合使用，利用|操作符
- 例如：用二进制方式写文件：`ios::binary|ios::out`
```c++
#include<iostream>
using namespace std;
#include<fstream>//头文件
//文本文件 写文件
void arrf()
{
	//1、包含头文件 fstream
	//2、创建流对象
	ofstream ofs;
	//3、指定方式
	ofs.open("test.txt",ios::out);
	//4、写内容
	ofs << "姓名：李成以" << endl;
	ofs << "性别：男" << endl;
	ofs << "年龄：19" << endl;
	//5、关闭文件
	ofs.close();
}
int main()
{
	arrf();

	return 0;
}
```
- 总结：文件操作必须包含头文件fstream
- 读文件可以利用ifstream,或者fstream
- 打开文件夹的时候需要指定操作文件的路径，以及打开方式
- 利用<<可以向文件中写数据
- 操作完毕，要关闭文件
## 129、读文件
- 读文件和写文件步骤相似，但是读取方式相对于比较多
- 1、包含头文件`#include<fstream>`
- 2、创建流对象`ifstream ifs;`
- 3、打开文件`ifs.open("文件路径"，打开方式);`
- 4、读数据 四种方式读取
- 5、关闭文件`ifs.close`
```c++
#include<iostream>
using namespace std;
#include<fstream>
void arrf1()
{
	//2、创建流对象
	ifstream ifs;
	//3、打开文件 判断是否打开成功
	ifs.open("test. txt", ios::in);
	if (!ifs.is_open())
	{
		cout << "文件打开失败" << endl;
		return;
	}
	//4、读文件
	//第一种
	/*char bur[1024] = { 0 };
	while(ifs>>bur)
	{
		cout << bur << endl;
	}*/
	//第二中
	/*char bur[1024] = { 0 };
	while (getline(bur, sizeof(bur)))    
	{
		cout << bur << endl;
	}*/
	//第三种
	/*string bur;
	while ( getline(ifs.bur))
	{
		cout << bur << endl;
	}*/
	//第四种
	char c;
	while ((c = ifs.get()) !=EOF  )//EOF end offile
	{
		cout << c;
	}

	//5、关闭文件
	ifs.close();
}
int main()
{
	arrf1();
	return 0;
}
- 总结：读文件可以用ifstream,或者fstream
- 利用s_open函数可以判断文件是否打开成功
- close关闭文件
```
# 二进制文件
- 以二进制的方式对文件进行读写操作
- 打开方式要指定为`ios::binary`
## 130、二进制写文件
- 二进制方式写文件主要利用流对象调用成员函数`write`
- 函数原型：`ostream& write(const char*buffe,int len)`
- 参数解释：字符指针buffer指向内存中一段存储空间，len是读写的字节数
```c++
#include<iostream>
using namespace std;
#include <fstream>//头文件
//二进制  写文件
class phone
{
public:
	char m_Name[64];
	int m_Age;

};
void test01()
{
	//1、包含头文件
	//2、创建流对象
	ofstream ofs("phone.txt", ios::out | ios::binary);

	//3、打开文件
	//ofs.open("phone.txt", ios::out | ios::binary);
	//4、写文件


//@
	phone p = {"张三", 19};
	ofs.write((const char*)&p, sizeof(phone));
	//5、关闭文件
	ofs.close();
}
int main()
{
	test01();
	return 0;
}
```
- 总结:文件输出流对象 可以通过write函数，以二进制方式写数据
## 131、二进制读文件
- 二进制方式读文件主要利用流对象调用成员函数read
- 函数原型：ifstrea& read(char *buffer,int len)
- 参数解释：字符指针buffer指向内存中一段存储空间，len是读写的字节数
```c++
#include<iostream>
using namespace std;

#include<fstream>
class phone
{
public:
	char m_Name[64];
	int m_Age;

};

//二进制读文件
void test01()
{
	//2、创建流对象
	ifstream ifs;
	//3、打开文件 判断文件是否打开成功
	ifs.open("phone txt", ios::in | ios::binary);
	if (!ifs.is_open())
	{
		cout << "文件打开失败" << endl;
		return;
	}
	//4、读文件


//@	重点
	phone p;
	ifs.read((char*)&p, sizeof(phone));
	cout << "姓名；  " << p.m_Name <<"年龄；  "<<p.m_Age << endl;

	//5、关闭文件
	ifs.close();
}
int main()
{
	test01();

	return 0;
}
```
## 132、职工管理系统

- 1、创建管理类
## 1、创建文件
- 在头文件和源文件的文件夹下分别创建worManager.h和workManager.cpp文件
- 在workManager.h中设计管理类
```c++
#pragma onc//防止头文件重复包含
#include<iostream>
using namespace std;
class WorerManager
{
public:
	//构造函数
	WorerManager();
	//析构函数
	~WorerManager();

};
////////////////

#include"workerManager.h"
WorerManager::WorerManager()
{

}
WorerManager::~WorerManager()
{

}

```
## 133、菜单功能
- 功能描述：与用户沟通界面
#### 添加成员函数
- 在管理类workerMannager.h中添加成员函数`void shou_Menu();`
```c++
//职工管理.cpp
#include<iostream>
using namespace std;
#include"workerManager.h"
int main()
{
	//实例化管理类对象
	WorerManager wm;
	//调用展示菜单的成员函数
	wm.Shou_Menu();

	system("pause");
    return 0;
}

//////// WorerManager.h
#pragma onc//防止头文件重复包含
#include<iostream>
using namespace std;
class WorerManager
{
public:
	//构造函数
	WorerManager();
	//展示菜单
	void Shou_Menu();
	//析构函数
	~WorerManager();

};

```
## 134、退出功能
#### 提供功能接口
- 在main函数中提供分支选择，提供每个功能接口
- 在workerManager.h中提供退出系统函数void exitsystem();
- 在workerManager.cpp中提供具体功能实现
```c++
//WorerManager.cpp
void WorerManager::exitsystem()
{
	cout << "欢迎下次使用" << endl;
	system("pause");
	exit(0);//退出程序
}


///// 职工管理系统.cpp
	wm.Shou_Menu();
	cout << "请输入你的选择" << endl;
	cin >> choice;//接受用户的选项
	switch (choice)
	{
	case 0://退出系统
		wm.exitsystem();
		break;
	case 1://增加职工
		break;
	case 2://显示职工
		break;
	case 3://删除职工
		break;
	case 4://修改职工
		break;
	case 5://查找职工
		break;
	case 6://排序职工
		break;
	case 7://清空文档
		break;

	default:
		system("cls");//清屏操作
	break;
	}
}
```
## 135、创建职工类
#### 创建职工抽象类
- 职工分为：普通员工、经理、老板
- 将三种职工抽象到一个类（worker）中，利用多态管理不同职工种类
- 职工的属性分为：职工编号、职工名字、职工所在部门编号
- 职工的行为：岗位职责信息描述、获取岗位名称
- 头文件夹下 创建文件worker.h文件并且添加如下代码
#### 创建普通员工类
- 普通员工类继承职工抽象类，并重写父类中纯虚函数
- 在头文件和源文件的文件夹下分别创建`empioyee.h` 和`employee.cpp`文件
```c++
//普通职工文件  empioyee.h


#pragma once
#include<iostream>
using namespace std;
#include"worker.h"

class Employee:public  Worker
{
public:
	//构造函数
	Employee(int id,string name,int dId);
	//显示个人信息
	virtual void shoulnfo();
	
	//获取岗位名称
	virtual string getDeptName();
};





////////////employee.cpp`
#include "emplyee.h"
//构造函数
Employee::Employee(int id, string name, int dId)
{
	this->m_Id = id;
	this->m_Name=name;
	this->m_Detld = dId;
}
//显示个人信息
void Employee::shoulnfo()
{
	cout << "职工编号" << this->m_Id
		<< "\t职工姓名" << this->m_Name
		<< "\t职工岗位" << this->getDeptName()
		<< "\t岗位职责; 完成经理给得任务" << endl;
 }

//获取岗位名称
string  Employee::getDeptName()
{
	return string ("员工");
 }
```
#### 创建经理类
- 经理类继承职工抽象类，并重写父类中纯虚函数，和普通员工类似
- 在头文件和源文件分别创建`manager.h`和`manager.cpp`文件
```c++
///////////// manager.cpp
#include"manager.h"
//构造函数
Manager::Manager(int id, string name, int dId)
{
	this->m_Id = id;
	this->m_Name = name;
	this->m_Detld = dId;
}
//显示个人信息
void Manager::shoulnfo()
{
	cout << "职工编号" << this->m_Id
		<< "\t职工姓名" << this->m_Name
		<< "\t职工岗位" << this->getDeptName()
		<< "\t岗位职责; 完成老板给的任务，并下发任务给普通员工" << endl;
 }
//获取岗位名称
string Manager ::getDeptName()
{
	return string("经理");
 }
//////////////////////// manager.h

#pragma onc
#include<iostream>
using namespace std;
#include"worker.h"
//经理类
class Manager :public Worker
{
public:
	//构造函数
	Manager(int id, string name, int dId);
	//显示个人信息
	virtual void shoulnfo();
	//获取岗位名称
	virtual string getDeptName();


};
```
#### 创建老板类
- 老板类继承职工抽象类，并重写父类中纯虚函数，和普通员工类似
- 在头文件和源文件的文件夹下分别创建`boss.h`和p`boss.cp`文件
```c++

////  boss.h
#pragma onc
#include<iostream>
using namespace std;
#include"worker.h"
//老板类
class Boss :public Worker
{
public:
	//构造函数
	Boss (int id, string name, int dId);
	//显示个人信息
	virtual void shoulnfo();
	//获取岗位名称
	virtual string getDeptName();


};
////////////  `boss.cpp

#include"boss.h"
//构造函数
Boss::Boss(int id, string name, int dId)
{
	this->m_Id = id;
	this->m_Name = name;
	this->m_Detld = dId;
}
//显示个人信息
void Boss::shoulnfo()
{
	cout << "职工编号" << this->m_Id
		<< "\t职工姓名" << this->m_Name
		<< "\t职工岗位" << this->getDeptName()
		<< "\t岗位职责; 管理公司所有事务" << endl;
}
//获取岗位名称
string Boss::getDeptName()
{
	return string("老板");
}

```
#### 136、添加职工
- 功能描述；批量添加职工，并且保存到文件中
#### 功能分析
- 用户在批量创建时，可能会创建不同种类的职工
如果将所有不同种类的员工都放入一个数组中，可以将所有员工的指针维护到员工数组里
- 如果想在程序中维护这个不定长度数组，可以将数组创建到堆区，并且利用Worker**的指针维护
#### 功能实现
- 在workerManage.h头文件中添加成员属性 代码：
```c++
int m_EmpNUm;//记录文件中的人员个数
worker**m_Emparray;//员工数组指针
```
- 在workerManage构造函数中初始化属性
```c++
WorerManager::WorerManager()
{
	//初始化人数
	this->EmpNum=0;
	//初始化数组指针
	this->m_Emparray=NULL:
}
```
- 在workerManager.h中添加成员函数
```c++
//增加职工
void Add_Emp();
```
- 在workerManager.cpp中实现该函数
```c++
void WorkerManager::Add_Emp()
{
	cout <<"请输入增加职工数量">>
	int addnum=0;
	cin>>addnum;
	if(addnum>0)
	{
		//计算新空间大小
		int newsize=this->m_EmpNum+addNum;
		//开辟新空间
		worker**newSppce=new worker*[newsize];
		//将原空间下内容放入新空间下
		if(this m_EmpArray!=NULL)
		{
			for(int i=0;i<this ->m_EmpNum;i++)
			{
				new Space[i]=this->m_EmpArray[i]
			}
		}
		//输入新数据
		for(int i=0;i<addNum;i++)
		{
			int id;
			string name;
			int dselect;
			cout <<"请输入"<<i+1<<"个新职工编号"<<endl;
			cin>>id;

			cout <<"请输入"<<i+1<<"个新职工姓名"<<endl;
			cin>>name;

			cout<<"请选择该职工的岗位"<<endl;
			cout <<"1、普通职工"<<endl;
            cout <<"2、经理"<<endl;
			cout <<"3、老板"<<endl;		
			cin>>dselect;
			
			
			WOrker*worer=NULL;
			swiltch(dselect)
			{
				case 1://普通员工
				worer=new Employee(id,name,1)
				break;

                case 2://经理
				worer=new Manager(id,name,2)
				break;

                case 3://老板
				worer=new Boss(id,name,3)
				break;
               default;
			   break;

			}
			new Space[this->EmpNum+i]=worker;
		}
		//释放原空间
		delete[] this->m_EnpArrayy;

		//更改新空间的指向
		this->m_EmpArray=newSpace

		//更新个数
		this->m_EmpNum=newsize;

		//提示信息
		cout <<"成功添加"<<addNum<<"名新职工"<<endl;
	}
	ease
	{
		cout <<"输入有误"<<endl;
	}
}
```
## 137、文件交互-写文件
- 功能描述：对文件进行读写
- 在上一个添加功能中，我们只是将所有数据添加到了内存中，一旦程序结束就无法保存了
因此文件管理类中需要一个与文件进行交互的功能，对于文件读写操作
#### 设定文件路径
- 首先我们将文件路径，在workerManager.h中添加宏常量，并且包含头文件`fstream`
```c++
#include<fstream>
#define FILENAME "empFile.txt"
```
#### 成员函数声明
在workerManager.h中类里添加成员函数`void save`
```c++
//保存文件
void save();
```
#### 保存文件功能实现
```c++
void WorkerManager::save()
{
	ofstream ofs;
	ofs.open(FILENAME , ios::out);
	for(int i=0;i<this->m_EmpNum;i++)
	{
		ofs<<this->m_EmpArray[i]->m_Id<<"  "
		<<this->m_EmpArray[i]->m_Name<<"  "
		<<this->m_EmpArray[i]->m_Detld<<endl;

	}
	ofs.close();
}
```
## 138、文件交互-读文件
- 功能描述：将文件中的内容读到程序中
- 虽然我们实现了添加职工后保存到文件的操作，但是每次开始运行程序，并没有将文件中数据读取到程序中
- 而我们的程序功能还有清空文件的需求
- 因此构造函数初始化数据的情况分为三种
- 1、第一次使用，文件未创建
- 2、文件存在，但是数据被用户清空
- 3、文件存在，并且保存职工的所有数据
#### 文件未创建
- 在workerManage.h中添加新成员属性m_FilelsEmpty标志文件是否为空
```c++
//标志文件是否为空
bool m_FilelsEmpty;
```
- 修改workeranager.cpp中构造函数代码
```c++
WorkerManager::workerManager()
{
	ifstream ifs;
	ifs.open(FILENAME,ios::in);

	if(!ifs.is_open())
	{
		cout <<"文件不存在"<<endl;//测试输出
		this->m_EmpNum=0;//初始化人数
		this->m_FilelsEmpty=true;//初始化文件为空标志
		this->m_EmpArray=NULL;//初始化数组
		ifs.close();//关闭文件
		return ;
	}
}
```
#### 文件存在且数据为空
- 在workerManage.cpp中的构造函数追加代码
```c++
//文件存在，并且没有记录
char ch;
ifs>>ch;
if(ifs.eof())
{
	cout <<"文件为空"<<endl;
	this->m_EmpNum=0;
	this->m_FilelsEmpty=true;
	this->m_EmpArray=NULL;
	ifs.close();
	return;
}
```
- 将文件创建后清空文件内容，并测试情况下初始化功能
- 我们发现文件不存在或者为空m_FilelsEmpty判断文件是否为空的标志都为真，那何时为假？
- 成功添加职工后，应该更改文件不为空的标志
- 在void Workeransger::Add_Emp()成员函数中添加
```c++
//更新职工不为空
this->m_FilelsEmpty=false;
```
#### 文件存在且保存职工数据
- 在workeranager.h中添加成员函数 int get_EmpNum;
```c++
//统计人数
int   get_EmpNum();
```
- workerManager.cpp中实现
```c++
int WorkerManager::get_EmpNum()
{
	ifstream ifs;
	ifs.open(FILENAME,ios::in)
	int id;
	string name;
	int dId;

	int num=0;

	while(ifs>>id&&ifs>>name&&ifs>>dId)
	{
		//记录人数
		num++;
	}
	ifs.close();
	return num;
}
```
- 在workerManager.cpp中构造函数继续追加代码
```c++
int num=this->get_EmpNum();
cout <<"职工个数"<<num<<endl;//测试代码
this->m_EmpNum=num;//更新成员属性
```
#### 初始化数组
- 根据职工的数据以及职工数据，初始化workerManager中的worker**m_EmpArray
- 在workerManager.h中添加成员函数 void init_Emp();
```c++
//初始化员工
void init_Emp();
```
- 在workerManager.cpp中实现
```c++
void WorerManager::init_Emp()
{
	ifstream ifs;
	ifs.open(FILENAME,ios::in);

	int id;
	string name;
	int dId;

	int index=0;

	while(ifs>>id && ifs>>name && ifs>>dId)
	{
		Worker*worker=NULL:
		//根据不同的部门Id创建不同对象
		if(dId==1)//普通员工
		{
			worker=new Employee(id,name,dId);
		}
		else if(dId==2)//经理
		{
           worker=new Manager(id,name,dId);
		}
		else//总裁
		{
			worker=new Boss(id,name,dId);
		}
		//存放在数组中
		this->m_EmpArray[index]=worker;
		index++;
	}
}
```
- 在WorkerManager.cpp构造函数追加代码
```c++
//根据职工数创建数组
this->m_EmpArray=new Worker*[this->m_EmpNum];
//初始化职工
init_Emp();

//测试代码
for(int i=0;i<m_EmpNum;i++)
{
	cout << "职工号" << this->m_EmpArray[i]->m_Id
	<< "\t职工姓名" << this->m_EmpArray[i]->m_Name
	<< "\t部门编号" << this->m_EmpArray[i]->m_Detld;<<endl;
}
```
## 139、显示职工
- 功能描述；显示当前所有职工信息
#### 显示职工的函数声明
- 在workerManager.h中添加成员函数 void Shou_Emp();
```c++
//显示职工
void Shou_Emp();
```
#### 显示职工函数实现
在worerManager.cp中实现成员函数 void Shou_Emp();
```c++

//显示职工
void WorkerManager::Shou_Emp()
{
	if(this-> m_FilelsEmpty)
	{
		cout <<"文件不存在或者记录为空"<<endl;
	}
	else
	{
		for(int i=0;i<m_EmpNum;i++)
		{
			//利用多态调用接口
			this->m_EmpArray[i]->shoulnfo();
		}
	}
	system("pause");
	system("cls");
}
```
## 140、删除职工
- 功能描述；按照职工的编号进行删除职工操作
#### 删除职工函数声明
- 在workerManager.h中添加成员函数 void Del_Emp();
```c++
//删除职工
void Del_Emp();
```
#### 职工是否存在函数声明
- 很多功能都需要用到根据职工是否存来进行操作：删除职工、修改职工、查找职工
- 因此添加该公告函数，以便后续调用
- 在workerManager.h中添加成员函数 int IsExist(int id);
```c++
//按照职工编号判断职工是否存在，若存在返回职工在数组中位置，不存在返回-1
int IsExist(int id);
```
#### 职工是否存在函数实现
在workeranager.cpp中实现成员函数 int IsExist(int id);
```c++
int WorkerManager::IsExist(int id)
{
	int index=-1;
	for(int i=0;i<this->m_EmpNum;i++)
	{
		if(this->m_EmpArray[i]->m_Id)
		{
			index=i;//找到职工
			break;
		}
	}
	return index;
}
```
#### 删除职工实现
- 在WorkerManager.h中添加成员函数 void Del_Emp();
```c++
//删除职工
void Del_Emp();
```
在workeranager.cpp中实现成员函数 Del_Emp();
```c++
//删除职工
void WorerManager::Del_Emp()
{
	if (this->m_FilelsEmpty)
	{
		cout << "文件不存在" << endl;
	}
	else
	{
		//按照职工编号删除
		cout << "请输入想要删除职工编号" << endl;
		int id = 0;
		cin >> id;

		int index=this->IsExist(id);

		if (index != -1)//说明职工存在，并且要删除index位置上的职工
		{
             //数组前移
			for (int i = index;i < this->m_EmpNum - 1;i++)
			{
				//数据前移
				this->m_EmpArray[i] = this->m_EmpArray[i + 1];
			}
			this->m_EmpNum--;//更新数组中记录的人员个数
			//同步更新到文件中
			this->save();
			cout << "删除成功" << endl;
		}
		else
		{
			cout << "删除失败，未找到该职工" << endl;
		}
	}
	//按任意键清屏
	system("pauce");
	system("cls");

}
```
## 141、修改职工
- 功能描述：能够按照职工编号对职工信息进行修改保存
#### 修改职工函数声明
- 在workerManager.h中添加成员函数 void Mod_Emp();
```c++
//修改职工
void Mod_Emp();
```
#### 修改职工函数实现
- 在workerManager.cpp中实现成员函数 void Mod_Emp();
```c++
//修改职工
void WorerManager:: Mod_Emp()
{
	if(this->m_FilelsEmpty)
	{
		cout <<"文件不存在"<<endl;
	}
	else
	{
		cout <<"请输入修改职工信息"<<endl;
		int id;
		cin>>id;

		int ret=this->IsExist(id);
		if(ret!=-1)
		{
			//查找到编号的职工
			delete this->m_EmpArray[ret];

			int newId=0;
			string newName="";
			int dSelect=0;

			cout <<"查到；"<<id<<"号职工，请输入新职工编号"<<endl;
			cin>>newId;

			cout <<"请输入新名字"<<endl;
			cin>>newName

			cout <<"请输入岗位"<<endl;
			cout <<"1、普通员工"<<endl;
			cout <<"2、经理"<<endl;
			cout <<"3、老板"<<endl;
			cin>>dSelect;

			Worker*worker=NULL:
			switch(dSelect)
			{
				case1:
				worker=new Employee(newId,newName,dSelect)
				break;

				case2:
				worker=newManager(newId,newName,dSelect)
                break;


				case3:
				worker=new Boss(newId,newName,dSelect)
                break;
				default:
				break;

			}
            //更改数据到数组中
			this->m_EmpArray[ret]=worker;

			cout <<"修改成功"<<endl;

			//保存到文件中
			this->save();
		}
		else
		{
			cout <<"修改失败，查无此人"<<endl;
		}
	}
	//按任意键 清屏
	system("pause");
	system("cls");
}
```
## 142、查找职工
- 功能描述：提供两种查找职工的方式，一种是按照职工编号，一种是按照职工姓名
#### 查找职工函数声明
- 在workerManager.h中添加函数 void Find_Emp();
```c++
//查找职工
void Find_Emp();
```
#### 查找职工函数实现
- 在workerManager.cpp中实现成员函数 void Find_Emp();
```c++
void WorerManager:: Find_Emp()
{
	if(this->m_FileIsEmpty)
	{
		cout <<"文件不存在或记录为空"<<endl;
	}
	else
	{
		cout <<"请输入查找的方式"<<endl;
		cout <<"1、按职工编号查找"<<endl;
		cout <<"2、按姓名查找"<<endl;

		int select=0;
		cin>>select;

		if(select==1)//按职工查找
		{
			int id;
			cout <<"请输入查找的职工编号"<<endl;
			cin>>id;

			int ret=IsExist(id);
			if(ret!=-1)
			{
				cout <<"查找成功！ 该职工信息如下"<<endl;
				this->m_EmpArray[ret]->shouInfo();
			}
			else
			{
				cout <<"查找失败，查无此人"<<endl;
			}
		}
		else if(select==2)//按姓名查找
		{
         string name;
		 cout <<"请输入查找的姓名"<<endl;
		 cin>>name;

		 bool flag=false;//查找到的标志
		 for(int i=0;i<m_EmpNum;i++)
		 {
			if(m_EmpArray[i]->m_Name==name)
			{
				cout <<"查找成功，职工编号为："
				<<m_EmpArray[i]->m_Id
				<<"号的信息如下"<<endl;

				flag=true;


				this->m_EmpArray[i]->shouInfo();
			}
		 }
		 if(flag==false)
		 {
          //查无此人
		  cout <<"查找失败，查无此人"<<endl;

		 }
		}
		else
		{
			cout <<"输入选项有误"<<endl;
		}
	}
	//按任意键 清屏
	system("pause");
	system("cls");
}
```
## 143、排序
- 功能描述：按照职工编号进行排序 ，顺序由用户自己选择
#### 排序函数声明
- 在workerManager.h中添加成员函数 void Sort_Emp();
```c++
//排序职工
void Sort_Emp();
```
#### 排序函数实现
- 在worerNabager.cpp中添加成员函数 void Sort_Emp();
```c++
void  WorerManager:: Sort_Emp()
{
if(this->m_FileIsEmpty)
{
	cout <<"文件不存在或为空"<<endl;
	system("pauce");
	system("cls");
}
else
{
	cout <<"请选择排序方式"<<endl;
	cout <<"1、按照工号进行升序"<<endl;
	cout <<"2、按照工号进行降序"<<endl;

	int select=0;
	cin>>select;

	for(int i=0;i<m_EmpNum;i++)
	{
		int minOrMax=i;
		for(int j=i+1;j<m_EmpNum;j++)
		{
			if(select==1)//升序
			{
				if(m_EmpArray[minOrMax]->m_Id>m_EmpArray[i]->m_Id)
				{
					minOrMax=j;
				}
			}
			else//降序
			{
				if(m_EmpArray[minOrMax]->m_Id<m_EmpArray[j]->m_Id)
				{
					minOrMax=j;
				}

			}
		}
		if(i!=minOrMax)
		{
			Worker*temp=m_EmpArray[i];
		m_EmpArray[i]=m_EmpArray[minOrMax];
		m_EmpArray[minOrMax]=temp;
		}
	}

	cout <<"排序成功，排序后的结果为"<<endl;
	this->save();
	this->Shou_Emp();
}

}
```
 ## 144、清空文件
 - 功能描述：将文件记录清空
 #### 清空的函数声明
 - 在workranager.h中添加成员函数 void Clean_File();
 ```c++
 //清空文件
 void Clean_File();
 ```
 #### 清空的函数实现
 - 在workerMan.cpp中实现成员函数 void Clean_File();
 ```c++
 void  WorerManager::Clean_File()
 {
	cout <<"确认清空？"<<endl;
	cout <<"1、确认"<<endl;
	cout <<"2、返回"<<endl;

	int select=0;
	cin>>select;

	if(select==1)
	{
		//打开模式ios::trunc 如果存在删除文件并重新创建
		ofstream ofs(FILENAME,ios::trunc);
		ofs.close();

		if(this->m_EmpArray !=NULL)
		{
			for(int i=0;i<this->m_EmpNum;i++)
			{
				if(this->m_EmpArray[i]!=NULL)
				{
					delete this->m_EmpArray[i];
				}
			}
			this->m_EmpNum=0;
			delete[] this->m_EmpArray;
			this->m_EmpArray=NULL;
			this->m_FileIsEmpty=true;
		}
		cout <<"清除成功"<<endl;
	}
//按任意键 清屏
	system("pause");
	system("cls");

 }
 ```
 # c++提高编程
## 本阶段主要针对c++泛型编程和STL技术做详细讲解，探讨c++更深层次的使用
## 模板
## 145、模板的概念
- 模板就是建立通用的摸具，大大提高复用性
- 模板的特点； 
- 模板不可以直接使用，它只是一个框架
- 模板的通用并不是万能的
## 146、模板函数
- c++另一种编程思想称为泛型编程，只要利用的技术就是模板
- c++提供两种模板机制：`函数模板`和`类模板`
#### 函数模板的语法
- 函数模板作用：
- 建立一个通用函数，其函数返回值类型和形参可以不具体制定，用一个`虚拟的类型`来代表
```c++
- 语法：template <tyename T>//声明一个模板告诉编译器后面代码中紧跟着的T不要报错。T是一个通用类型
- 函数声明或定义
```
- 解释：
- template----声明创建模板
- typename----表面其后面的符号是一种数据类型，可以用`class`代替
- T---通用的数据类型，名称可以替换，通常为大小字母
```c++
//函数模板
template<typename T>
void jiaohuan(T&a,T&b)
{
	T temp = a;
	a = b;
	b = temp;
}

void arrf()
{
	int a = 10;
	int b = 20;
	//利用函数模板交换
	//两种方法使用模板

	//1、自动类型推导
	//jiaohuan(a, b);
	
	//2、显示指定类型
	jiaohuan<int>(a, b);


	cout << "a=" << a << endl;
	cout <<"b=" << b << endl;

		
}
int main()
{
	arrf();
	return 0; 
	
}
```
- 总结：
- 函数模板利用关键字 `template`
- 使用函数模板有两种方式：1、自动类型推导 2、显示指定类型
- 模板的目的是为了提高复用性，将类型参数化
## 147、函数模板的注意事项
- 1、自动类型推导，必须推导出一致的数据类型T，才可以使用
```c++
void test()
{
	int a = 10;
	int b = 20;
	char c = 'c';
	//jiaohuan(a, b);//正确
	//jiaohuan(a, b, c);//错误 推导不出一致的T类型
	cout << "a=" << a << endl;
	cout << "b=" << b << endl;
}
```
- 2、模板必须要确定出T的数据类型，才可以使用
```c++
template<class T>
void fuen()
{
	cout << "函数fuen的调用" << endl;
}
void test01()
{
	fuen<int >();//要想能运行只能指定一个数据类型 用显示指定类型 指定类型 int```
}
```
- 总结；使用模板时必须确定出通用数据类型T，并且能够推导出一致的类型
## 148、函数模板案例
 案例描述：
 -利用函数模板封装一个排序的函数，可以对不同数据类型数组进行排序
 - 排序规则从大到小，排序算法为选择排序
 - 分别利用char数组和int数组进行测试
 ```c++
 #include<iostream>
using namespace std;
//实现通用 对数组进行排序函数
// 规则 从大到小
//算法  选择
// 测试 char 数组 int 数组
//交换函数模板
template<class T>
void myswap(T& a, T& b)
{
	T temp = a;
	a = b;
	b = temp;
}
//排序算法
template<class T>
void mySort (T arr[], int len)
{
	for (int i = 0;i < len;i++)
	{
		int max = i;//认定最大值的下标
		for (int j = i + 1;j < len;j++)
		{
			//认定最大值 比遍历出的数值要小，说明j下标的元素才是真正最大值
			if (arr[max] < arr[j])
			{
				max = j;//更新最大值下标
			}
		}
		if (max != i)
		{
			//交换max和i元素
			myswap(arr[max], arr[i]);
		}


	}
}
//提供打印数组模板
template<class T>
void printArray(T arr[],int len)
{
	for (int i = 0;i < len;i++)
	{
		cout << arr[i] << " ";
     }
}
void test01()
{
	//测试char数组
	char chararr[] = "badcfe";
	int num = sizeof(chararr) / sizeof(char);
	mySort(chararr, num);
	printArray(chararr, num);
}
void test02()
{
	//测试int 数组
	int intarr[] = { 7,5,4,6,2,1,3, };
	int num = sizeof(intarr) / sizeof(int);
	mySort(intarr, num);
	printArray(intarr, num);
}
int main()
{
	//test01();
	test02();
	return 0;
}
 ``` 
 ## 149、普通函数和函数模板的区别
 - 普通模板函数调用时可以发生自动类型转换（隐式类型转换）
 - 函数模板调用时，如果利用自动类型推导，不会发生隐式类型转换
- 如果利用显示指定类型的方式，可以发生隐式类型转换
```c++
#include<iostream>
using namespace std;
//普通函数与函数模板区别
//1、普通函数调用时可以发生隐式类型转换
//2、函数模板 用自动类型推导，不可以发生隐式类型转换
//3、函数模板 用显示指定类型，可以发生隐式转换
//普通函数
int myAdd01(int a,int b)
{
	return a + b;
}

//函数模板
template<class T>
T myAdd02(T a,T b)
{
	return a + b;
}

void test01()
{
	int a = 10;
	int b = 20;
	char c = 'c';//c-99
	cout << myAdd01(a, c) << endl;

	//自动类型推导 不会发生隐式类型转换
	//cout << myAdd02(a, c) << endl;;
	
	//显示指定类型 会发生隐式类型转换
	cout <<myAdd02<int >(a, c) << endl;
}
int main()
{
	test01();

	return 0;
```
- 总结：建议使用显示指定类型的方式，调用函数模板，因为可以自己确定通用类型T
## 150、普通函数和模板函数调用规则
- 调用规则如下：
- 1、如果普通函数和函数模板都可以实现，优先调用普通函数
- 2、可以通过空模板参数列表来强制调用函数模板
- 3、函数模板也可以发生重载
- 4、如果函数模板可以产生更好的匹配，优先调用函数模板
```c++
#include<iostream>
using namespace std;
//普通函数和函数模板的调用规则
// 1、如果普通函数和函数模板都可以实现，优先调用普通函数
// 2、可以通过空模板参数列表来强制调用函数模板
// 3、函数模板也可以发生重载
// 4、如果函数模板可以产生更好的匹配，优先调用函数模板
void myPrint(int a, int b)
{
	cout << "调用的普通函数" << endl;
}

template<class T>
void myPrint(T a,T b)
{
	cout << "函数模板调用" << endl;
}

template<class T>
void myPrint(T a, T b,T c)
{
	cout << "重载函数模板调用" << endl;
}


void test01()
{
	int a = 10;
	int b = 20;
	//myPrint(a, b);
	
	//通过空模板参数列表强制调用函数模板
	//myPrint<>(a,b);

	//myPrint(a, b, 100);

	//如果函数模板产生更好的匹配，优先调用函数模板
	char c1 = 'a';
	char c2 = 'b';
	myPrint(c1, c2);
}
int main()
{
	test01();

	return 0;
}
```
- 总结：既然提供了函数模板，最好不要提供普通函数，否则容易出现二义性
## 151、模板的局限性
- 模板的通用并不是万能的
- 例如：
```c++
termplate<class T>
void f(T a,T b)
{
	a=b;
}
```
在上述中提供的赋值操作，如果传入a和b是一个数组，就无法实现了
- c++为了解决这种问题，提供模板的重载，可以为这些特定类型提供具体化模板
- 例如；
```c++
#include<iostream>
using namespace std;
//模板的局限性
//模板并不是万能的，有些特定的数据类型，需要用具体化方式做特殊实现
class phone
{
public:

	phone(string name, int age)
	{
		this->m_Name = name;
		this->m_Age = age;
}
	string m_Name;
	int m_Age;
};
//对比两个数据是否相等函数
template<class T>
bool myCompare(T &a,T &b)
{
	if (a == b)
	{
		return true;
	}
	else
	{
		return false;
	}
}

//利用具体化phone的版本实现代码，具体化优先调用

template<>bool myCompare(phone& p1, phone& p2)
{
	if (p1.m_Name == p2.m_Name && p1.m_Age == p2.m_Age)
	{
		return true;
	}
	else
	{
		return false;
	}
}
void test01()
{
	int a = 10;
	int b = 20;
	bool ret= myCompare(a, b);
	if (ret)
	{
		cout << "a==b" << endl;
	}
	else
	{
		cout << "a!=b" << endl;
	}
}
void test02()
{
	phone p1("Tom",10);
	phone p2("Tom",11);
	bool ret = myCompare(p1, p2);
	if (ret)
	{
		cout << "p1==p2" << endl;
	}
	else
	{
		cout << "p1!=p2" << endl;
	}

}
int main()
{
	test01();
	test02();
	return 0;
}

```
- 总结：
- 利用具体化的模板，可以解决自定义类型的通用化
- 学习模板并不是为了写模板，而是在STL能够运用系统提供的模板
## 152、类模板
```c++
- 语法：template<typename T>
类
```
解释：
- template----声明创建模板
- typename----表面其后面的符号是一种数据类型，可以用`class`代替
- T---通用的数据类型，名称可以替换，通常为大小字母
```c++
#include<iostream>
using namespace std;
//类模板
template<class NameType,class AgeType>
class phone
{
public:
	phone(NameType name, AgeType age)
	{
		this->m_Name = name;
		this->m_Age = age;
	}
	void showphone()
	{
		cout << "name=:"<<this->m_Name << endl;
		cout << "age=; "<<this->m_Age << endl;
	}
	NameType m_Name;
	AgeType m_Age;
};

void test01()
{
	phone<string ,int >p1("sa1", 29);
	p1.showphone();
}
int main()
{
	test01();
	return 0;
}
```
- 总结：类模板和函数模板语法相似，在声明模板templateh后面加类，此类为类模板
## 153、类模板和函数模板的区别
类模板和函数模板的区别有两点
- 1、类模板没有自动类型的使用方式
- 2、类模板在模板参数列表中可以有默认参数
```c++
#include<iostream>
using namespace std;
//类模板和函数模板的区别
template<class NameType,class AgeType=int>
class phone
{
public:
	phone(NameType name, AgeType age)
	{
		this->m_Name = name;
		this->m_Age = age;
	}
	void showphone()
	{
		cout << "name=  " << this->m_Name << endl;
		cout << "age=  " << this->m_Age << endl;
	}
	NameType m_Name;
	AgeType m_Age;

};
//1、类模板没有自动类型的使用方式
void test01()
{
	//phone p("匈奴王"，923);//错误，无法用自动类型推导
	phone <string, int >p("匈奴王", 923);//正确，只能用显示指定类型
	p.showphone();
}

//2、类模板在模板参数列表中可以有默认参数
void test02()
{
	phone<string>p1("雪狼湖",93932);
	p1.showphone();
}
int main()
{
	//test01();
	test02();
	return 0;
}
```
-总结：
- 类模板使用只能用显示指定类型方式
 -类模板中的模板参数列表可以有默认参数 
 ## 154、类模板中成员函数创建时机
 - 类模板中成员函数和普通类中成员函数创建时机是有区别的
 - 普通类中的成员函数一开始就可以创建
 - 类模板中的成员函数只有在调用时才能创建
 ```c++
 #include<iostream>
using namespace std;
//类模板中成员函数的创建时机
//类模板中成员函数在调用时才能创建
class phone1
{
	public:
		void showphone1()
		{
			cout << "phone01 show" << endl;
		}

};

class phone2
{
public:
	void showphone2()
	{
		cout << "phone02 show" << endl;
	}

	
};

template <class T>
class myclass
{
public:
	T obj;

	//类模板中成员函数
	void func1()
	{
		obj.showphone1();
	}

	void func2()
	{
		obj.showphone2();
	}

};
void test01()
{
	myclass<phone1>m;
	m.func1();
	//m.func2();
}

int main()
{
	test01();
	return 0;
	
}
 ```
- 总结：类模板成员函数并不是一开始创建的，在调用时才会去创建
## 155、类模板对象做函数参数
- 学习目标：
- 类模板实例化出的对象，向函数传参的方式
- 一共有三种传入方式； 
- 1、指定传入方式----直接显示对象数据类型
- 2、参数模板化----将对象中的参数变为模板进行传递
- 3、整个类模板化---将这个对象类型模板化传递

```c++
#include<iostream>
using namespace std;
//类模板对象函数参数
template<class T1, class T2>
class phone
{
public:
	phone (T1 name,T2 age)//构造函数
	{
		this->m_Name = name;
		this->m_Age = age;
	}
	void showphone()//成员函数 打印函数
	{
		cout << "name= " << this->m_Name << "age= " << this->m_Age << endl;
	}
	T1 m_Name;
	T2 m_Age;
};
//1、指定传入方式----直接显示对象数据类型
void printphone1(phone<string ,int>&p )//封装函数
{
	p.showphone();
}

void test01()//调用函数
{
	phone<string, int >p("关羽", 933);
	printphone1(p);
}
 

	//2、参数模板化----将对象中的参数变为模板进行传递
template<class T1, class T2>
void printphone2(phone<T1, T2 >&p)
{
	p.showphone();
	//cout << "T1类型" << typeid(T1).name() << endl;
	//cout << "T2类型" << typeid(T2).name() << endl;
}
void test02()
{

	phone<string, int >p("张飞", 9833);
	printphone2(p);
}

	//3、整个类模板化-- - 将这个对象类型模板化传递
template<class T>
void printphone3(T &p)
{
	p.showphone();
	//cout << "T类型" << typeid(T).name() << endl;
}
void test03()
{
	phone<string, int >p("刘备", 91833);
	printphone3(p);
}
int main()
{
	test01();
	test02();
	test03();
	return 0;
}
```
- 总结：`最常用的是第一种：指定传入方式（直接了当的告诉编译器 2和3相当于类模板配合函数模板比较复杂 且需要编译器推导）`
## 156、类模板与继承
- 当类模板碰到继承时，需要注意一下几点
- 当子类继承的父类是一个类模板时，子类在声明的时候，要指出父类中`T`的类型
- 如果不指定，编译器无法给子类分配内存
- 如果想灵活指出父类中`T`的类型，子类也需要变为类模板
```c++
#include<iostream>
using namespace std;
template<class T>
class Base
{
public:
	T m;

};
//class Son:public Base//1、错误，必须知道父类中T的类型，才能继承给子类
class Son :public Base<int>
{

};
void test01()
{

}

//2、如果想灵活的指定父类中T的类型，子类也需要变类模板
template<class T1,class T2>
class Son2 :public Base<T2>
{
public:
	Son2()
	{
		cout << "T1的数据类型=  " << typeid(T1).name() << endl;
		cout << "T2的数据类型=  " << typeid(T2).name() << endl;

	}
	T1 obj;
};
void test02()
{
	Son2<int, char>s2;
}
int main()
{
	//test01();
	test02();
	return 0;
}
```
- 总结：如果父类是模板，子类需要指出父类中T的数据类型
## 157、类模板成员函数类外实现
- 学习：能够掌握模板中成员函数类外实现
- 总结：类模板中成员函数类外实现时，需要加上模板参数列表
```c++
phone<T1, T2>::phone(T1 name, T2 age)//模板参数列表phone<T1,T2>
```

```c++
#include<iostream>
using namespace std;
//类模板成员函数类外实现
template<class T1,class T2>
class phone
{
public:
	phone(T1 name, T2 age);
	void shoephone();
	T1 m_Name;
	T2 m_Age;
};

//构造函数类外实现
template<class T1,class T2>
phone<T1, T2>::phone(T1 name, T2 age)
{
	this->m_Name = name;
	this->m_Age = age;
}
//成员函数的类外实现
template<class T1, class T2>
void phone<T1, T2>::shoephone()
{
		cout << "name= " << this->m_Name << "age= " << this->m_Age << endl;	
}
void test01()
{
	phone<string, int>p("hsdh", 4823);
	p.shoephone();

}
int main()
{
	test01();

	return 0;
}
```
## 158、类模板分文件编写
- 学习：掌握类模板成员函数分文件编写产生的问题已经解决方式
- 问题：类模板中成员函数创建时机是在调用阶段，导致分文件编写时链接不到
- 解决：
- 1、直接包含.cpp源文件
- 2、将声明和实现写到同一个文件里，并更改后缀名.hpp,hpp是约定的名称，并不是强制
- 总结：主流的解决方式是第二种，将模板成员函数写在一起，并将后缀名改为.hpp
## 159、类模板与友元
- 目标；掌握类模板配合友元的类内和内外实现
- 全局函数类内实现：直接在类内声明友元即可
- 全局函数类外实现：需要提前让编译器知道全局函数的存在
```c++
#include<iostream>
using namespace std;
//通过全局函数 打印phone函数
//提前让编译器知道phone存在
template<class T1, class T2>
class phone;
//2、全局函数类外实现
template<class T1, class T2>

void printphone2(phone<T1, T2>p)
{
	cout << "类外Name" << p.m_Name << "类外Age" << p.m_Age << endl;
}

template<class T1, class T2>

class phone
{
	//全局函数类内实现
	friend void printphone(phone<T1, T2>p)
	{
		cout << "类外Name" << p.m_Name << "类外Age" << p.m_Age << endl;
	}

	
	//全局函数类外实现
	//加<>参数列表
	//如果全局函数类外实现的话，需要让编译器提前知道这个函数的存在
	friend void printphone2<>(phone<T1, T2>p);


	
public:
	phone(T1 name,T2 age)
	{
		this->m_Name = name;
		this->m_Age = age;
	}
	
private:
	T1 m_Name;
	T2 m_Age;
};
//1、全局函数在类内实现
void test01()
{
	phone<string, int >p("果是", 2838);
	printphone(p);
}

//类外实现的调用
void test02()
{
	phone<string, int >p("骄傲是", 238);
	printphone2(p);
}
int main()
{
	test01();
	test02();
	return 0;
}
```
- 总结：建议用全局函数做类内实现，用法简单，而且编译器可以直接识别
## 160、类模板案例
- 案例描述
- 可以对内置数据类型以及自定义数据类型的数据进行存储
- 将数组中的数据传递到堆区
- 构造函数中可以传入数组的容量
- 提供对应的拷贝构造函数以及operator=防止浅拷贝问题
- 提供尾插法和尾删法对数组中的数据进行增加和删除
- 可以通过下标的方式访问数组中的元素
- 可以获取数组中当前元素个数和数组容量
```c++
- 头文件.hpp
//////// MyArrar.hpp/////
#pragma once
#include<iostream>
using namespace std;

template<class T>
class MyArrar
{
public:
    // 有参构造  参数 容量
    MyArrar(int capacity)
    {
       // cout << "MyArrar有参构造调用" << endl;
        this->m_Capacity = capacity;
        this->m_Size = 0;
        this->pAddress = new T[this->m_Capacity];
    }

    // 拷贝构造函数
    MyArrar(const MyArrar& arr)
    {
       // cout << "MyArrar拷贝构造调用" << endl;
        this->m_Capacity = arr.m_Capacity;
        this->m_Size = arr.m_Size;
        // 深拷贝
        this->pAddress = new T[arr.m_Capacity];

        // 将arr中的数据都拷贝过来
        for (int i = 0; i < this->m_Size; i++)
        {
            this->pAddress[i] = arr.pAddress[i];
        }
    }

    // operator= 防止浅拷贝问题
    MyArrar& operator=(const MyArrar& arr)
    {
      //  cout << "MyArrar operator=调用" << endl;
        // 先判断原来堆区是否有数据，如果有先释放掉
        if (this->pAddress != NULL)
        {
            delete[] this->pAddress;
            this->pAddress = NULL;
            this->m_Capacity = 0;
            this->m_Size = 0;
        }

        // 深拷贝
        this->m_Capacity = arr.m_Capacity;
        this->m_Size = arr.m_Size;
        this->pAddress = new T[this->m_Capacity];
        for (int i = 0; i < this->m_Size; i++)
        {
            this->pAddress[i] = arr.pAddress[i];
        }
        return *this;
    }

    //尾插法
    void Push_Back(const T&val)
    {
        //判断容量是否等于大小
        if (this->m_Capacity == this->m_Size)
        {
            return;
        }
        this->pAddress[this->m_Size] = val;
        this->m_Size++;//更新数组大小 在数组的末尾插入数据
    }
    //尾删法
    void Pop_Back()
    {
        //让用户访问不到最后一个元素，即为尾删
        if (this->m_Size == 0)
        {
            return;
        }
        this->m_Size--;
    }

    //通过下标方式访问数组中的元素
    T & operator[](int index)
    {
        return this->pAddress[index];
    }
    //返回数组容量
    int getCapacity()
    {
        return this->m_Capacity;
    }
    // 返回数组大小
    int getSize()
    {
        return this->m_Size;
    }
    // 析构函数
    ~MyArrar()
    {
        if (this->pAddress != NULL)
        {
           // cout << "MyArrar析构调用" << endl;
            delete[] this->pAddress;
            this->pAddress = NULL;
        }
    }

private:
    T* pAddress; // 指针指向堆区开辟的真实数组
    int m_Capacity; // 数组容量
    int m_Size; // 数组大小
};
```
- 源文件.cpp
```c++
#include<iostream>
using namespace std;
#include"MyArray.hpp"

void printInArray(MyArrar<int>arr)
{
	for (int i = 0;i < arr.getSize();i++)
	{
		cout << arr[i] << endl;
	}
}

void test01()
{
	MyArrar<int>arr1(5);

	for (int i = 0;i < 5;i++)
	{
		//利用尾插法向数组中插入数据
		arr1.Push_Back(i);
	}
	cout << "array1的打印输出" << endl;

	printInArray(arr1);

	cout << "arr1的容量" <<arr1.getCapacity()<< endl;
	cout << "arr1的大小" << arr1.getSize() << endl;

	
	MyArrar<int>arr2(arr1);
	cout << "array2的打印输出" << endl;
	printInArray(arr2);

	//尾删
	arr2.Pop_Back();
	cout << "arr2的尾删后； " << endl;
	cout << "arr2的容量" << arr2.getCapacity() << endl;
	cout << "arr2的大小" << arr2.getSize() << endl;
	//MyArrar<int>arr3(100);
	//arr3 = arr1;
}
//测试自定义数据类型
class phone
{
public:
	phone() {};
	phone(string name, int age)
	{
		this->m_Name = name;
		this->m_Age = age;
	}

	string m_Name;
	int m_Age;
};
void printphoneArr(MyArrar<phone>& arr)
{
	for (int i = 0;i < arr.getSize();i++)
	{
		cout << "姓名" << arr[i].m_Name << "年龄" << arr[i].m_Age << endl;
	}
}
void test02()
{
	MyArrar<phone>arr(10);
	phone p1("萧瑟", 23);
	phone p2("女巫", 75);
	phone p3("乖哈", 79);
	phone p4("赛前", 73);
	phone p5("静安", 79);
	//将数据插入到数组中
	arr.Push_Back(p1);
	arr.Push_Back(p2);
	arr.Push_Back(p3);
	arr.Push_Back(p4);
	arr.Push_Back(p5);
	//打印数组
	printphoneArr(arr);

	//输出容量
	cout << "arr容量为：  " << arr.getCapacity() << endl;
	//输出大小
	cout << "arrr大小为：  " << arr.getSize() << endl;
}
int main()
{
	//test01();
	test02();
	return 0;
}
```
# STL初识
## STL的诞生
- 长久以来，软件界一直希望建立一种可重复利用的东西
- c++的面向对象和泛型编程思想，目的就是复用性的提升
- 大多数情况下，数据结构和算法都未能有一套标准，导致被迫从事大量重复工作
- 为了建立数据结构和算法的一套标准，诞生了STL
### STL的基本概念
- STL(Standard Template Library,标准模板库)
- STL从广义上分为：容器(container)算法(algorithm)迭代器(iterator)
- 容器和算法之间通过迭代器进行无缝连接
- STL几乎所有的代码都采用了模板类或者模板函数
### STL六大组件
- STL分为六大组件，分别是：容器、算法、迭代器、仿函数、适配器（配接器）、空间配置器
- 1、容器：各种数据结构，如：`vector、list、deque、set、map`等，用来存放数据
- 2、算法：各种常用算法。如:`sort、find、copy、for_each`等
- 3、迭代器：扮演了容器与算法之间的胶合剂
- 4、仿函数：行为类似函数，可做为算法某种策略
- 5、适配器：一种用来修饰容器或者仿函数或迭代器接口的东西
- 6、空间配置器：负责空间的配置与管理
### STL中容器、算法、迭代器
容器：置物之所也
- STL容器就是将运用最广泛的一下数据结构实现出来
- 常用的数据结构：数组、链表、树、栈、队列、集合、映射表 等
- 这些容器分为`序列式容器` 和`关联式容器`两种：
- 序列式容器：强调值的排序，序列式容器中的每个元素均有固定的位置
- 关联式容器：二叉数结构，各元素之间没有严格的物理上的顺序关系

算法：问题之解法
- 有限的步骤，解决逻辑或数学上的问题，这一门学科我们叫算法(Algorithms)
- 算法分为：`质变算法和非质变算法`
- 质变算法：是指运算过程中会更改区间内元素的内容。例如拷贝、替换、删除等等
- 非质变算法：是指运算过程中不会更改区间内的元素内容，例如查找、计数、遍历、寻找极值等等
迭代器：容器和算法之间的粘合剂
- 提供一种方法，使之能够依序寻访某个容器所含的各个元素，而又无需暴露该容器的内部表达方式每个容器都有之间专属的迭代器
- 迭代器使用非常类似指针，初学阶段我们可以先理解为指针

 迭代器种类：
- 输入迭代器：对数据的只读访问（只读 支持++、==、！=）
- 输出迭代器：对数据的只写访问（只写 支持++）
- 前向迭代器：读写操作，并能向前推进迭代器（读写 支持++、==、！=）
- 双向迭代器：读写操作，并且能向前向后操作（读写 支持++、--）
- 随机访问迭代器：读写操作，可以以跳跃的方式访问任意数据，功能最强的迭代器（读写 支持++、--、【n】、-n、<、<=、>、>=

常用的容器中迭代器种类为双向迭代器，和随机迭代器
## 161、容器算法迭代器初识
- 了解STL中容器、算法、迭代器概念之后，我们利用代码感受STL的魅力
- STL中最常用的容器为`vector`可以理解为数组，下面我们学习如何向这个容器插入数据，并遍历容器

vecter存放内置数据类型
- 容器：vector
- 算法：for_each
- 迭代器:vector<int>::iterator
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<algorithm>//标志算法头文件
//vector容器存放内置数据类型
void myprint(int val)
{
	cout << val << endl;
}
void test01()
{
	//创建了一个vector容器，数组
	vector<int>v;
	//向容器插入数据
	v.push_back(10);
	v.push_back(20);
	v.push_back(30);
	v.push_back(40);
	v.push_back(50);
	//通过迭代器访问容器中的数据
	//vector<int>::iterator itBegin = v.begin();//起始迭代器  指向容器中第一个元素
	//vector<int>::iterator itEnd = v.end();//结束迭代器 指向容器最后一个元素的下一个位置

	////第一种遍历方式
	//while (itBegin != itEnd)
	//{
	//	cout << *itBegin << endl;
	//	itBegin++;
	//}


	//第二种遍历方式
	//for (vector<int>::iterator it = v.begin();it != v.end();it++)
	//{
		//cout << *it << endl;
	//}



	//第三种遍历方式 利用STL提供遍历数组
	for_each(v.begin(), v.end(), myprint);


};
int main()
{
	test01();

	return 0;
}
```
## 162、vector存放自定义数据类型
- 目标：vector中存放自定义数据类型，并打印
```c++
#include <iostream>
using namespace std;
#include<vector>
//vector容器中存放自定义数据类型
class phone
{
	public:
		phone(string name, int age)
		{
			this->m_Name = name;
			this->m_Age = age;
		}
		string m_Name;
		int m_Age;
};
void test01()
{
	vector<phone>v;
	phone p1("yehh", 217);
	phone p2("yehw", 343);
	phone p3("ewq", 341);
	phone p4("eqwh", 35);
	phone p5("resh", 27);

	//向容器中添加数据
	v.push_back(p1);
	v.push_back(p2);
	v.push_back(p3);
	v.push_back(p4);
	v.push_back(p5);
	//遍历容器中的数据
	for (vector<phone>::iterator it = v.begin();it != v.end();it++)
	{
		//cout << "姓名" << (*it).m_Name << "年龄" << (*it).m_Age << endl;
		cout << "姓名； " << it->m_Name << "年龄； " << it->m_Age << endl;
	}
}

//存放自定义数据类型指针
void stet02()
{
	vector<phone*>v;
	phone p1("yehh", 217);
	phone p2("yehw", 343);
	phone p3("ewq", 341);
	phone p4("eqwh", 35);
	phone p5("resh", 27);

	//向容器中添加数据
	v.push_back(&p1);
	v.push_back(&p2);
	v.push_back(&p3);
	v.push_back(&p4);
	v.push_back(&p5);

	//遍历容器
	for (vector<phone*>::iterator it = v.begin();it != v.end();it++)
	{
		cout << "姓名； " << (*it)->m_Name << "年龄； " << (*it)->m_Age << endl;
	}
}
int main()
{
	//test01();
	stet02();
	return 0;
}

```
## 163、vector容器嵌套容器
- 目标；容器中嵌套容器，我们将所有数据进行遍历输出
```c++
#include<iostream>
using namespace std;
#include<vector>
void test01()
{
	vector<vector<int>>v;
	//创建小容器
	vector<int>v1;
	vector<int>v2;
	vector<int>v3;
	vector<int>v4;
	vector<int>v5;

	//向小容器中添加数据
	for (int i = 0;i < 5;i++)
	{
		v1.push_back(i + 1);
		v2.push_back(i + 2);
		v3.push_back(i + 3);
		v4.push_back(i + 4);
		v5.push_back(i + 5);
	}
	//将小容器插入大容器中
	v.push_back(v1);
	v.push_back(v2);
	v.push_back(v3);
	v.push_back(v4);
	v.push_back(v5);

	//通过大容器，把所有数据遍历一遍
	for (vector<vector<int>>::iterator it = v.begin();it != v.end();it++)
	{
		//(*it)-----容器 vector<int>
		for (vector<int>::iterator vit = (*it).begin();vit != (*it).end();vit++)
		{
			cout << *vit << " ";
		}
		cout << endl;
	}

}

int main()
{
	test01();

	return 0;
}
```
## 164、string基本概念
- 本质：string 是c++风格的字符串，而string本质也是一个类

string和char*的区别：
- char*是一个指针
- string是一个类，类内部封装了char*，管理这个字符串，是一个char*型容器

特点：
- string类内部封装了很多成员方法
- 例如：查找find,拷贝copy，替换replace,插入insert
- string管理char*所分配的内存，不用担心复制越界和取值越界等，由类内部进行负责
#### string 构造函数
- 构造函数原型
- string(); `//创建一个空的字符串 例如：string str;`
- string(const char*s);`//使用字符串s初始化`
- string(const string&str);`//使用一个string对象初始化另一个string对象`
- string(int n,char c);//`使用n个字符c初始化`
```c++
#include<iostream>
using namespace std;
//string 构造函数
 

//string();                          // 创建一个空的字符串 例如：string str;
//string(const char* s);            `// 使用字符串s初始化`
//string(const string & str);         `// 使用一个string对象初始化另一个string对象`
//string(int n, char c);              //`使用n个字符c初始化`
void test01()
{
	string();//默认构造（无参构造）
	
	const char* str="hello world";
	string s2(str);
	cout << "s2= " << s2 << endl;

	string s3(s2);
	cout << "s3= " << s3 << endl;

	string s4(10, 'a');
	cout << s4 << endl;

}
int main()
{
	test01();

	return 0;

}
- 总结：string 的多种构造方式没有可比性灵活使用即可
```
## 165、string赋值操作
功能描述：
- 给string字符串进行赋值

赋值的函数原型：
- string& operator=(const char*s); //char*类型字符串 赋值给当前的字符串
- string& operator=（const string &s);//把字符串s赋值给当前的字符串
- string& operator=(char c);//字符串赋值给当前的字符串
- string& assign(const char *s);//把字符串s赋给当前的字符串
- string& assign(const char *s,int n);//把字符串s的前n个字符串赋给当前字符串
- string& assign(const string &s);//把字符串s赋值给当前字符串
- string& assign(int n,char c);//用n个字符串c赋给当前字符串
```c++
#include<iostream>
using namespace std;

void test01()
{
	//string& operator=(const char* s); //char*类型字符串 赋值给当前的字符串
	string str1;
	str1 = "hello wreid";
	cout << str1 << endl;

	//string & operator=（const string & s);//把字符串s赋值给当前的字符串
	string str2;
	str2 = str1;
	cout << str2 << endl;

	//string & operator=(char c);//字符串赋值给当前的字符串
	string  str3;
	str3 = 'a';
	cout << str3 << endl;

	//string & assign(const char* s);//把字符串s赋给当前的字符串
	string str4;
	str4.assign("hello c++");
	cout << str4 << endl;

	//string & assign(const char* s, int n);//把字符串s的前n个字符串赋给当前字符串
	string str5;
	str5.assign("hello c++",5);
	cout << str5 << endl;

	//string & assign(const string & s);//把字符串s赋值给当前字符串
	string str6;
	str6.assign(str5);
	cout << str6 << endl;

	//string & assign(int n, char c);//用n个字符串c赋给当前字符串
	string str7;
	str7.assign(10, 'w');
	cout << str7 << endl;

}
int main()
{
	test01();

	return 0;
}
- 总结：string的赋值方法很多，operator=这种方式是比较实用的
```
## 166、string字符串拼接
- 功能描述：实现字符串末尾拼接字符串

函数原型：
- string& operator+=(const char*str); //重载+=操作符
- string& oerator+=(congst char c);//重载+=操作符
- string& oerator+=(const string&str);//重载+=操作符
- string& append(const char *s);//把字符串s连接到当前字符串结尾
- string& append(const char*s,int n);//把字符串s的前n个字符连接到当前字符串结尾
- string& append(conse string &s);//同operator+=（const string &str）
- string& append(const string &s,int pos,int n);//字符串s中从pos开始的n个字符连接到字符串结尾
```c++
#include<iostream>
using namespace std;

void test01()
{
	string str1 = "我";
	str1 += "爱玩游戏";
	cout <<"str1= "<< str1 << endl;
	str1 += ';';
	cout << "str1= " << str1 << endl;

	string str2 = "LOL  DNF";
	str1 += str2;
	cout << "str1= " << str1 << endl;;


	string str3 = "I";
	str3.append("LOVE");
	str3.append("ALHS",3);
	//I LOVE ALH
	cout << "str3= " << str3 << endl;

	//str3.append(str2,0,3);//只截取LOL
	//I LOVE ALH LOL DNF
	str3.append(str2, 4, 4);//只截取了DNF，参数2  从哪个位置截取 参数3  截取字符个数
	cout << "str3= " << str3 << endl;


}
int main()
{
	test01();

	return 0;
}
- 总结：字符串拼接的重载版本很多，初学阶段记住几种即可
```
## 167、string查找和替换
功能描述：
- 查找：查找指定字符串是否存在
- 替换：在指定的位置替换字符串

函数原型：
- int find(const string& str,int pos=0)const;` 查找str第一次出现的位置，从pos开始查找`
- int find(const char*s,int pos=0)const; `查找s第一次出现的位置，从pos开始查找`
- int find(const char*s,int pos,int n);`从pos位置查找s的前n个字符第一次的位置`
- int find(const char c,int pos=0)const; `查找字符C第一次出现的位置`
- int rfing(const string& str,int pos=npos)const; `查找str最后一次位置，从pos开始`
- int rfind(const char*s,int pos=npos)const;` 查找S最后一次出现的位置，从pos开始查找`
- int rfind(const char*s,int pos,int n)const; `从pos查找S的前n个字符串最后一次位置`
- int rfind(const char c,int pos=0)consst; `查找字符c最后一次出现的位置`
- string& replace(int pos,intn,const string &str);`替换从pos开始n个字符为字符串str`
- string& replace(int pos,int n,const char*s); `替换从pos开始的n个字符为字符串s`
```c++
#include<iostream>
using namespace std;
//字符串查找和替换
//1、查找
void test01()
{
	string str1 = "abcdefg";
	int pos=str1.find("de");
	if (pos == -1)
	{
		cout << "未找到字符串" << endl;
	}
	else
	{
		cout << "找到字符串" << pos << endl;
	}

	//rfind和find的区别
	//rfind从右往左查找，find从左往右查找
	pos=str1.rfind("de");
	cout << pos << endl;

}
//2、替换
void test02()
{
	string str1 = "abcdefg";
	//从1号位置起 3个字符串 替换为“111” 
	str1.replace(1, 3, "111");
	cout << str1 << endl;
}
int main()
{
	//test01();
	test02();
	return 0;
}
```
- 总结：
- find查找是从左往右，rfind是从右往左
- find找到字符串后返回查找的第一个字符位置，找不到返回-1
- replace在替换时，要指定从哪个位置起，多少个字符，替换成什么样的字符串
## 168、string字符串比较
- 功能：字符串之间的比较

比较方式
- 字符串比较是按照字符ASCII码进行对比
- `=`返回 0
- `>`返回 1
- `<`返回 -1

函数原型
- int compare(const string &s); 与字符串s比较
 - int compare(const char*s)const; 与字符串s比较
 ```c++
 #include<iostream>
using namespace std;
//字符串比较操作

void test01()
{
	string str1 = "hello";
	string str2 = "xello";

	if (str1.compare(str2) == 0)
	{
		cout << "str1等于str2" << endl;
	}
	else if(str1.compare(str2)>0)
	{
		cout << "str1大于str2" << endl;
	}
	else
	{
		cout << "str1小于str2" << endl;
	}
}

int main()
{
	test01();
	return 0;
}
- 总结：字符串对比主要是用于比较两个字符串是否相等，判断谁大谁小的意义并不是很大
 ```
 ## 169、string 字符存取
 string 中单个字符存取方式有两种
 - char& operator[](int n);//通过[]方式取字符
 - char& at(int n);//通过at方法获取字符
 ```c++
 #include<iostream>
using namespace std;
void test01()
{
	string str = "hello";
	//1、通过[]访问单个字符
	for (int i = 0;i < str.size();i++)
	{
		cout << str[i] << " ";
	}
	cout << endl;
	//2、通过at方式访问单个字符
	for (int i = 0;i < str.size();i++)
	{
		cout << str.at(i) << " ";
	}
	cout << endl;

	//修改单个字符
	str[0] = 'x';
	//xello
	cout << str << endl;

	str.at(1) = 'x';
	cout << str << endl;
}
int main()
{
	test01();
	
	return 0;
}
- 总结：str，ing 字符串中单个字符串存取有两种方式[]和at
 ```
 ## 170、string 插入和删除
 - 功能：
 - string字符串进行插入和删除字符操作

 函数原型
 - string& insert(int pos,const char *s);//插入字符
 - string& insert(int pos,const string& str)//插入字符串
 - string& insert(int pos,int n,char c);//在指定位置插入n个字符c
 - string7 erase(int pos,int n=npos);//删除从pos开始的n个字符
 ```c++
 #include<iostream>
using namespace std;
//字符串插入和删除
void test01()
{
	string str = "hello";
	//插入
	str.insert(1, "111");
	cout << str << endl;

	//删除
	str.erase(1, 3);
	cout << str << endl;

}
int main()
{
	test01();

	return 0;
}
- 总结：插入和删除的起始下标都是从0开始
 ```
 ## 171、string子串
 功能：
 - 从字符串中获取想要的子串

 函数原型
 - string substr(int pos=0,int n=npos)const;//返回由pos开始的n个字符组成的字符串
 ```c++
 #include<iostream>
using namespace std;
//string 求子串
void test01()
{
	string str = "abcdef";
	string subStr = str.substr(1, 3);
	cout << subStr << endl;
}
//实用操作
void test02()
{
	string email = "hello@sina.com";
	//从邮件地址中获取用户名
	int pos=email.find("@");
	cout << pos << endl;
	string usName = email.substr(0, pos);
	cout <<  usName << endl;
}
int main()
{
	//test01();
	test02();

	return 0;
}
- 总结；灵活运用求字串功能，可以在实际开发中获取有效的信息
 ```
## 172、vector容器
- 功能；
- vector 和数据结构数组非常相似，也称为单端数组

vector与普通数组区别
- 不同之处在于数组是静态空间，而vector可以动态扩展

动态扩展
- 并不是在原空间之后续接新空间，而是找更大的内存空间，然后将原数据拷贝新空间，释放原空间

vector容器的迭代器是支持随机访问的迭代器
#### vector构造函数
- 功能：创建vector容器

函数原型；
- vector<T>v;  `采用模板实现类实现，默认构造函数`
- vector(v.begin(),v.end());`//将v(begin(),end())区间中的元素拷贝给自身`
- vector(n,elem);`构造函数将n个elem拷贝给本身`
- vector(const vector &vec);`拷贝构造函数`
```c++
#include<iostream>
using namespace std;
#include<vector>

void printvector(vector<int>&v)
{
	for (vector<int>::iterator it = v.begin();it != v.end();it++)
	{
		cout << *it << " ";
	}
		
}
//vector 构造函数
void test01()
{
	vector<int>v1;//默认构造  无参构造

	for (int i = 0;i < 10;i++)
	{
		v1.push_back(i);
	}
	printvector(v1);

	//通过区间方式进行构造
	vector<int>v2(v1.begin(), v1.end());
	printvector(v2);

	//n个elem方式构造
	vector<int>v3(10, 100);
	printvector(v3);

	//拷贝构造
	vector<int>v4(v3);
	printvector(v4);
}
int main()
{
	test01();

	return 0;
}
```
## 173、vector赋值操作
- 给vector容器赋值

函数原型
- vector& operator=(const vector &vec);`重载等号操作符`
- assign(beg,end);`将(beg,end)区间中的数据拷贝赋值给本身`
- assign(n,elem)`将n个elem拷贝赋值本身`
```c++
#include<iostream>
using namespace std;
#include<vector>

void printvector(vector<int>&v)
{
	for (vector<int>::iterator it = v.begin();it != v.end();it++)
	{
		cout << *it << " ";
	}
	cout << endl;
}
//vector赋值操作
void test01()
{
	
	vector<int>v1;
	for (int i = 0;i < 10;i++)
	{
		v1.push_back(i);
	}
	printvector(v1);

	//1、赋值 operator=
	vector<int>v2;
	v2 = v1;
	printvector(v2);

	//2、assign
	vector<int>v3;
	v3.assign(v1.begin(), v1.end());
	printvector(v3);

	//3、n个elem 方式赋值
	vector<int>v4;
	v4.assign(10, 100);
	printvector(v4);

}
int main()
{
	test01();

	return 0;
}
- 总结：vector赋值比较简单，使用operator=,或者assign都可以
```
## 174、vector容量和大小
- 描述：对vector容器的容量和大小操作

函数原型：
- empty();`判断容器是否为空`
- capacity();`容器的容量`
- size();`返回容器中元素个数`
- resize(int num);`重新指定容器的长度为num，若容器变长，则以默认值填充新位置；如果容器变短，则末尾超出容器长度的元素被删除`
- resize(int num,elem);`重新指定容器的长度为Num,若容器变长，则以elem值填充新位置；如果容器变短，则末尾超出容器长度的元素被删除`
```c++
#include<iostream>
using namespace std;
#include<vector>
void printvector(vector<int>& v)
{
	for (vector<int>::iterator it = v.begin();it != v.end();it++)
	{
		cout << *it << " ";
	}
	cout << endl;
}

void test01()
{
	vector<int>v1;
	for (int i = 0;i < 10;i++)
	{
		v1.push_back(i);
	}
	printvector(v1);

	//判断容器是否为空
	if (v1.empty())//为真  代表容器为空
	{
		cout << "v1为空" << endl;
	}
	else
	{
		cout << "v1不为空" << endl;
		cout << "v1容量" << v1.capacity() << endl;
		cout << "v1的大小" << v1.size() << endl;
	}

	//重新指定大小
	//利用重载版本，可以指定默认填充值，参数2就是指定的
	v1.resize(19,88);//如果重新指定过长 默认0来填充位置
	printvector(v1);


	v1.resize(8);
	printvector(v1);//如果重新指定的比原来短，超出部分就会删除
}
int main()
{
	test01();
	return 0;
}
- 总结：
- empty---判断是否为空
- size----返回元素个数
- capacity---返回容器容量
- resize---重新指定大小
```
## 175、vector插入和删除
 - 描述：对vector容器进行插入，删除操作

 函数原型
 - push_back(elem);`尾部插入元素ele`
 - pop_back();`删除最后一个元素`
 - insert(const_iterator  pos,elem);`迭代器指向位置pos插入元素elem`
 - insert(const_iterator pos,int count,elem);`迭代器指向位置pos插入count个元素elem`
 - erase(const_iterator pos);`删除迭代器指向的元素`
 - erase(const_iterator start,const_iterator end);`删除迭代器从start到end之间的元素`
 - clear();`删除容器中所有元素`
 ```c++
 #include<iostream>
using namespace std;
#include<vector>
void printvector(vector<int>& v)
{
	for (vector<int>::iterator it = v.begin();it != v.end();it++)
	{
		cout << *it << " ";
	}
	cout << endl;
}
void test01()
{
	vector<int>v1;
	//尾插
	v1.push_back(10);
	v1.push_back(20);
	v1.push_back(30);
	v1.push_back(40);
	v1.push_back(50);
	//遍历
	printvector(v1);
	//尾删
	v1.pop_back();
	printvector(v1);
	//插入 第一个参数是迭代器
	v1.insert(v1.begin(),100);
	printvector(v1);

	v1.insert(v1.begin(), 2, 1000);
	printvector(v1);

	//删除  参数也是迭代器
	v1.erase(v1.begin());
	printvector(v1);
	//清空
	//v1.erase(v1.begin(), v1.end());
	v1.clear();
	printvector(v1);
}
int main()
{
	test01();

	return 0;
}
- 总结
- 尾插----push_back
- 尾删----pop_back
- 插入----insert(位置迭代器)
- 删除----erase(位置迭代器)
- 清空----clear
 ```
 ## 176、vector数据存取
 - 描述：对vector中的数据的存取操作

 函数原型
 - at(int idx);`返回索引lidx所指的数据`
 - operator[];`返回索引lidx所指的数据`
 - front();`返回容器中第一个数据元素`
 - back();`返回容器中最后一个数据元素`
 ```c++
 include<iostream>
using namespace std;
#include<vector>
//vector数据存取
void test01()
{
	vector<int>v1;
	for (int i = 0;i < 10;i++)
	{
		v1.push_back(i);
	}
	//利用[]方式访问数组中元素
	for (int i = 0;i < v1.size();i++)
	{
		cout << v1[i] << " ";
	}
	cout << endl;

	//利用at方式访问
	for (int i = 0;i < v1.size();i++)
	{
		cout << v1.at(i) << " ";
	}
	cout << endl;

	//获取第一个元素
	cout << "第一个元素为； " << v1.front() << endl;
	//获取最后一个元素
	cout << "最后一个元素为； " << v1.back() << endl;
}
int main()
{
	test01();

	return 0;
}
- 总结
- 除了用迭代器获取vector容器中元素。[]也可以
- front返回容器第一个元素
- back返回容器最后一个元素
 ```
 ## 177、vector互换容器
 - 描述； 实现两个容器内部进行互换

 函数原型
 - swap(vec);`将vec与本身的元素互换`
 ```c++
 #include<iostream>
using namespace std;
#include<vector>
//vector 容器互换
void printvector(vector<int>& v)
{
	for (vector<int>::iterator it = v.begin();it != v.end();it++)
	{
		cout << *it << " ";
	}
	cout << endl;
}
//1、基本使用
void test01()
{
	vector<int>v1;
	for (int i = 0;i < 10;i++)
	{
		v1.push_back(i);
	}
	cout << "互换前" << endl;
	printvector(v1);

	vector<int>v2;
	for (int i = 10;i >0;i--)
	{
		v2.push_back(i);
	}
	printvector(v2);


	cout << "交换后" << endl;
	v1.swap(v2);
	printvector(v1);
	printvector(v2);
}

//2、实际用途
//巧用swap可以收缩内存空间
void test02()
{
	vector<int>v;
	for (int i = 0;i < 100000;i++)
	{
		v.push_back(i);
	}
	cout << "v的容量为：" << v.capacity() << endl;
	cout << "v的大小为:" << v.size() << endl;


	v.resize(3);//重新指定大小
	cout << "v的容量为：" << v.capacity() << endl;
	cout << "v的大小为:" << v.size() << endl;

	//巧用swap收缩
	vector<int>(v).swap(v);
	cout << "v的容量为：" << v.capacity() << endl;
	cout << "v的大小为:" << v.size() << endl;

}

int main()
{
	//test01();
	test02();
	return 0;
}
- 总结：swap可以使用两个容器互换，可以达到实用的收缩内存效果
 ```
 ## 178、vector预留空间
 - 描述：减少vector在动态扩展容量时的扩展次数

 函数原型
 - reserve(int len);`容器预留len个长度，预留位置不初始化，元素不可访问`
 ```c++
 #include<iostream>
using namespace std;
#include<vector>
//预留空间
void test01()
{
	int num = 0;//统计次数
	int* p = NULL;
	vector<int>v1;
	//利用reserve预留空间
	v1.reserve(100000);
	for (int i = 0;i < 100000;i++)
	{
		v1.push_back(i);
		if (p != &v1[0])
		{
			p = &v1[0];
			num++;
		}
	}
	cout << "num=" << num << endl;
}
int main()
{
	test01();
	
	return 0;
}
- 总结；如果数据量大 可以用reserve预留空间
 ```
 # deque容器基本概念
 - 描述：双端数组，可以对头端进行插入和删除操作

 deque和vector区别
 - vector对于头部的插入删除效率低，数据量越大，效率越低
 - deque相对而言，对于头部的插入删除速度会比vector快
 - vector访问元素时的速度会比deque快，这和两者内部实现有关

 deque内部工作原理：
 - deque内部有个中控器，维护每段缓冲区中的内容，缓冲区中存放真实数据
 - 中控器维护的是每个缓冲区的地址，使得使用deque时像一片连续的内存空间

 deque容器的迭代器也支持随机访问的
 ## 179、deque容器构造函数
 - 描述：deque容器构造

 函数原型
 - deque<T>;`默认构造形式`
 - deque(beg,end);`构造函数将（beg,end)区间中的元素拷贝给本身`
 - deque(n,elem);`构造函数将n个elem拷贝给本身`
 - deque(const deque &deq);`拷贝构造函数`
 ```c++
 #include<iostream>
using namespace std;
#include<deque>
//deque容器构造函数
void printdeque(deque<int>&d)
{
	for (deque<int>::iterator it = d.begin();it != d.end();it++)
	{
		cout << *it << " ";
	}
	cout << endl;
}
void test01()
{
	deque<int>d1;
	for (int i = 0;i < 10;i++)
	{
		d1.push_back(i);
	}
	printdeque(d1);

	//区间
	deque<int>d2(d1.begin(), d1.end());
	printdeque(d2);
	//n个elem
	deque<int>d3(10, 100);
	printdeque(d3);
	//拷贝构造
	deque<int>d4(d3);
	printdeque(d4);

}
int main()
{

	test01();
	return 0;
}
- 总结：deque和vector构造方式几乎一样，灵活运用即可
 ```
 ## 180、deque赋值操作
 - 描述：给deque容器赋值

 函数原型
 - deque& operator=*(const deque &dep);`重载等号操作符`
 - assign(beg,end);`将beg end区间中的数据拷贝赋值给本身`
 - assign(n,elem);`将n个elem拷贝赋值给本身`
 ```c++
 #include<iostream>
using namespace std;
#include<deque>
//deque赋值操作
void printdeque(deque<int>& d)
{
	for (deque<int>::iterator it = d.begin();it != d.end();it++)
	{
		cout << *it << " ";
	}
	cout << endl;
}
void test01()
{
	deque<int>d1;
	for (int i = 0;i < 10;i++)
	{
		d1.push_back(i);
	}
	printdeque(d1);

	//operator=赋值
	deque<int>d2;
	d2 = d1;
	printdeque(d2);

	//assign
	deque<int>d3;
	d3.assign(d1.begin(), d1.end());
	printdeque(d3);

	//n个elem
	deque<int>d4;
	d4.assign(10, 100);
	printdeque(d4);
}
int main()
{

	test01();
	return 0;
}
 ```
 ## 181、deque大小操作
 - 描述：对deque容器的大小进行操作

 函数原型
 - deque.empty();`判断容器是否为空`
 - deque.size();`返回容器中元素个数`
 - deque.resize(num);`重新指定容器长度为num，若容器变长，则以默认值填充新位置。如果容器变短，则末尾超出容器长度的元素被删除`
 - deque.resize(num,elem);`重新指定容器长度为num，若容器变长，则以elem值填充新位置。如果容器变短，则末尾超出容器长度的元素被删除`
 ```c++
 #include<iostream>
using namespace std;
#include<deque>
//deuqe容器大小操作
void printdeque(deque<int>& d)
{
	for (deque<int>::iterator it = d.begin();it != d.end();it++)
	{
		cout << *it << " ";
	}
	cout << endl;
}
void test01()
{
	deque<int>d1;
	for (int i = 0;i < 10;i++)
	{
		d1.push_back(i);
	}
	printdeque(d1);
	if (d1.empty())
	{
		cout << "d1为空" << endl;
	}
	else
	{
		cout << "d1不为空" << endl;
		cout << "d1大小" << d1.size() << endl;
		//deque没有容量概念
	}
	//重新指定大小
	//d1.resize(18);
	d1.resize(15, 8);
	printdeque(d1);

	d1.resize(5);
	printdeque(d1);
}
int main()
{

	test01();
	return 0;
}
- 总结：
- deque没有容器概念
- 判断---empy
- 返回元素个数---size
- 重新指定个数---resize
 ```
 ## 182、deque插入和删除
 - 描述：向deque容器中插入和删除数据

 函数原型
 - 两端插入操作
 - puch_back(elem);`在容器尾部添加一个数据`
 - puch_front(elem);`在容器头部插入数据`
 - pop_back();`删除容器最后一个数据`
 - pop_front();`删除容器第一个数据`

 指定位置操作
 - insert(pos,elem);`在pos位置插入一个elem元素拷贝，返回新数据的位置`
 - insert(pos,n,elem);`在pos位置插入n个elem数据，无返回值`
 - insert(pos,beg,end);`在pos位置插入（beg, end）区间数据，无返回值`
 - clear();`清空容器的所有数据`
 - erase(beg,end);`删除（beg end）区间的数据 返回下一个数据位置`
 - erase(pos);`删除pos位置的数据，返回下一个数据位置`
 ```c++
 #include<iostream>
using namespace std;
#include<deque>
void printdeque(deque<int>& d)
{
	for (deque<int>::iterator it = d.begin();it != d.end();it++)
	{
		cout << *it << " ";
	}
	cout << endl;
}

//两端操作
void test01()
{
	deque<int>d1;
	//尾插
	d1.push_back(10);
	d1.push_back(20);

	//头插
	d1.push_front(100);
	d1.push_front(200);
	printdeque(d1);

	//尾删
	d1.pop_back();
	printdeque(d1);

	//头删
	d1.pop_front();
	printdeque(d1);
}
void test02()
{
	deque<int>d1;
	d1.push_back(10);
	d1.push_back(20);
	d1.push_front(100);
	d1.push_front(200);
	//200  100 10 20
	printdeque(d1);

	//insert插入
	d1.insert(d1.begin(), 1000);
	//1000 200 100 10 20
	printdeque(d1);

	d1.insert(d1.begin(),2, 10000);
	//10000  10000 1000 100 10 20
	printdeque(d1);

	//按照区间插入
	deque<int>d2;
	d2.push_back(1);
	d2.push_back(2);
	d2.push_back(3);

	d1.insert(d1.begin(), d2.begin(), d2.end());
	printdeque(d1);
}

void test03()
{
	deque<int>d1;
	d1.push_back(10);
	d1.push_back(20);
	d1.push_front(100);
	d1.push_front(200);

	//删除
	deque<int>::iterator it = d1.begin();d1.end();it++;
	d1.erase(it);
	//200  10 20
	printdeque(d1);

	//区间方式删除
	d1.erase(d1.begin(), d1.end());
	//清空
	d1.clear();
	printdeque(d1);
}
int main()
{

	//test01();
	//test02();
	test03();
	return 0;
}
```
- 总结：
- 插入和删除提供的位置是迭代器
- 尾插----push_back
- 尾删----pop_back
- 头插----puch_front
- 头删----pop_front
## 183、deque数据存取
- 描述：对deque中数据的存取操作

函数原型
- ta(int idx);`返回索引idx所指的数据`
- operator[];`返回索引idx所指的数据`
- front();`返回容器中第一个数据元素`
- back();`返回容器中最后一个数据元素`
```c++
#include<iostream>
using namespace std;
#include<deque>
//deque数据存取
void test01()
{
	deque<int>d1;
	d1.push_back(10);
	d1.push_back(20);
	d1.push_back(30);
	d1.push_back(100);
	d1.push_back(200);
	d1.push_back(300);

	//通过[]方式访问
	for (int i = 0;i < d1.size();i++)
	{
		cout << d1[i] << " ";
	}
	cout << endl;
	//通过at方式访问
	for (int i = 0;i < d1.size();i++)
	{
		cout << d1.at(i) << " ";
	}
	cout << endl;

	cout << "第一个元素" << d1.front() << endl;
	cout << "最后一个元素" << d1.back() << endl;

}
int main()
{
	test01();
	return 0;
}
- 总结；
- 除了用迭代器获取deque容器中元素，[]和at也可以
- front 返回容器第一个元素
- back返回容器最后一个元素
```
## 184、deque排序
- 描述；利用算法实现对deque容器进行排序

算法；
- sort(iterator beg,iterator end);`对beg和end区间元素进行排序`
- 头文件：`#include<algorithm>`//标准算法头文件
- `sort(d.begin(), d.end());`
```c++
#include<iostream>
using namespace std;
#include<deque>
#include<algorithm>//标准算法头文件
void printdeque(deque<int>& d)
{
	for (deque<int>::iterator it = d.begin();it != d.end();it++)
	{
		cout << *it << " ";
	}
	cout << endl;
}
//deque排序
void test01()
{
	deque<int>d;
	d.push_back(10);
	d.push_back(20);
	d.push_back(30);
	d.push_front(400);
	d.push_front(500);
	d.push_front(600);
	printdeque(d);
	//排序  默认排序规则 从小到大 升序
	//对于支持随机访问的迭代器的容器，都可以利用sort算法直接对其进行排序
	//vector容器也可以利用sort进行排序
	sort(d.begin(), d.end());
	cout << "排序后" << endl;
	printdeque(d);
}
int main()
{
	test01();
	return 0;
}
- 总结；sort算法非常实用，使用时包含头文件algorithm即可
```
## 185、案例--评委打分
- 描述：有5名选手ABCD，10个评委分别对每一名选手打分，去除最高分，去除评委中最低分，取平均分

实现步骤；
- 1，创建5名选手放到vector容器中
- 2，遍历vector容器取出来每一个选手，执行for循环，可以把10个评分打分存到deque容器中
- 3，sort算法对deque容器中分数排序，去除最高和最低
- 4，deque 容器遍历一遍，累加总分
- 5，获取平均分
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<deque>
#include<algorithm>
//有5名选手ABCD，10个评委分别对每一名选手打分，去除最高分，去除评委中最低分，取平均分
//选手类
class phone
{
public:
	phone(string name ,int score)
	{
		this->m_Name = name;
		this->M_Score = score;
	}
	string m_Name;
	int M_Score;

};
void rintvector(vector<phone>&v)
{
	string nameSeed = "ABCDE";
	for (int i = 0;i < 5;i++)
	{
		string name = "选手";
		name += nameSeed[i];

		int score = 0;
		
		phone p(name, score);
		//将创建的phone对象放入到容器中
		v.push_back(p);
	}
}
//打分
void setScore(vector<phone>&v)
{
	for (vector<phone>::iterator it = v.begin();it != v.end();it++)
	{
		//将评委的分数，放入到deque容器中
		deque<int>d;
		for (int i = 0;i < 10;i++)
		{
			int score = rand() % 41 + 60;
			d.push_back(score);
		}
		
		//排序
		sort(d.begin(), d.end());

		//去除最高和最低
		d.pop_back();
		d.pop_front();

		//取平均分
		int sum = 0;
		for (deque<int>::iterator dit = d.begin();dit != d.end();dit++)
		{
			sum += *dit;//累加每个评委分数
		}
		int ave = sum / d.size();

		//将平均分赋值给选手
		it->M_Score = ave;
     }
}
void showScore(vector<phone>&v)
{
	for (vector<phone>::iterator it = v.begin();it != v.end();it++)
	{
		cout <<"姓名； "<< it->m_Name << "平均分； " << it->M_Score << endl;
	}

}
int main()
{
	//随机数种子
	srand((unsigned int)time(NULL));
	
	//1、创建5名选手
	vector<phone>v;//存放选手容器
	rintvector(v);

	//测试
	/*for (vector<phone>::iterator it = v.begin(); it != v.end();it++)
	{
		cout <<"姓名； "<< (*it).m_Name <<"分数；  "<< (*it).M_Score << endl;
	}*/
	
	//2、给5名选手打分
	
	setScore(v);
	

	//3、显示最后得分
	showScore(v);

	return 0;
}
```
## stack容器
概念：stack容器是一种先进后出的数据结构，它只有一个出口


 栈中只有顶端的元素才可以被外界使用，因此栈不允许有遍历行为
 - 栈中进入数据称为---入栈`push`
 - 栈中弹出数据称为---出栈`pop`
 ## 186、stack容器常用接口
 - 描述：栈容器常用的对外接口

 构造函数
 - stack<T>stk;`stack采用模板实现，stack对象的默认构造形式`
 - stack(const stack &stk);`拷贝构造函数`

 赋值操作
 -stack& operator=(const stack &stk);`重载等号操作符`

 数据存取
 - push(elem);`向栈顶添加元素`
 - pop();`从栈顶移除第一个元素`
 - top();`返回栈顶元素`

 大小操作
 - empty();`判断对象`
 - size();`返回栈大小` 
 ```c++
 #include<iostream>
using namespace std;
#include<stack>
//栈stack常用接口
void test01()
{
	//特点 先进后出
	stack<int>s;
	//入栈
	s.push(10);
	s.push(20);
	s.push(30);

	//只要栈不为空，查看数据，并且出栈
	while (!s.empty())
	{
		//查看栈顶的元素
		cout << "栈顶元素为；" << s.top() << endl;

		//出栈
		s.pop();
	}
	cout << "栈的大小" << s.size() << endl;
}
int main()
{
	test01();

	return 0;
}
- 总结：
- 入栈--push
- 出栈--pop
- 返回栈顶--top
- 判断栈是否为空--empty
- 返回栈大小--size
 ```
 ## 187、queue容器
 - 概念：queue是一种先进先出的数据结构，它有两个出口

- 队列容器允许从一端新增元素，从另一端移除元素
- 队列中只有队头和队尾才可以被外界使用，因此队列不允许有遍历行为
- 队列中进数据称为--入队`push`
- 队列中出数据称为--出队`pop`
#### queue容器常用接口
- 描述：栈容器常用的对外接口

构造函数
- queue<T>que;`queue采用模板类实现，queue对象的默认构造形式`
- queue(const queue &que);`拷贝构造函数`

赋值操作
- queue& operator=(const queue &que);`重载等号操作符`

数据存取
- push(elem);`尾部添加元素`
- pop();`从对头移除一个元素`
- back();`返回最后一个元素`
- front();`返回第一个元素`

大小操作
- empty();`判断堆栈是否为空`
- size();`返回栈的大小`
```c++
#include<iostream>
using namespace std;
#include<queue>
//队列queue
class phone
{
public:
	phone(string name,int age)
		{
		this->m_Name = name;
		this->m_Age = age;
		}
	string m_Name;
	int m_Age;
};
void test01()
{
	//创建队列
	queue<phone>q;
	//准备数据
	phone p("哦标", 19);
	phone p1("流程", 29);
	phone p2("伊萨", 16);
	phone p3("鱼白", 94);

	//入队
	q.push(p);
	q.push(p1);
	q.push(p2);
	q.push(p3);

	
	//判断只要队列不为空，查看队头，队尾,出队
	while(!q.empty())
	{
		//查看队头
		cout << "队头元素---姓名" << q.front().m_Name << endl;
		cout << "队头元素---年龄" << q.front().m_Age << endl;
		//查看队尾
		cout << "队尾元素---姓名" << q.back().m_Name << endl;
		cout << "队尾元素---年龄" << q.back().m_Age << endl;
	//出队操作
		q.pop();
	}
	cout << "队列大小" << q.size() << endl;

}
int main()
{
	test01();

	return 0;
}
- 总结；
- 入队--push
- 出队--pop
- 返回队头元素--front
- 返回队尾元素--back
- 判断队是否为空--empty
- 返回队列大小--size
```
## 189、list容器
- 描述：将数据进行链式存储

链表（slist）：是一种物理存储单元上非连续的存储结构，数据元素的逻辑顺序是通过链表中的指针链表实现的

链表的组成：链表由一系列节点组成

结点组成：一个是存储数据元素的`数据域`，另一个是存储下一个节点地址的`指针域`

STL中的链表是一个双向循环列表

链表优缺点
- 优点：可以对任意位置进行快速插入的删除元素
- 缺点；容器遍历速度没有数组快。占用空间比数组大

由于链表的存储方式并不是连续的内存空间，因此链表list中的迭代器只支持前移和后移，属于`双向迭代器`

list的优点；
- 采用动态存储分配，不会造成内存浪费和溢出
- 链表执行插入和删除操作十分方便，修改指针即可，不需要移动大量元素

list的缺点；
- 链表灵活，但是空间（指针域）和（遍历）额外耗费较大
- list有一个重要的性质，插入操作和删除都不会造成原有的list迭代器的失效，这在vector是不成立的

总结：STL中`list和vector是两个最常使用的容器`,各有各的优势
## 190、list构造函数
- 创建；list容器

函数原型
- list<T>lis:`list采用模板类实现，对象的默认构造形式`
- list（beg，end):`构造函数将（beg,end）区间中的元素拷贝给本身`
- list(n,elem);`构造函数将n个elem拷贝给本身`
- list(const list &lis);`拷贝构造函数`
```c++
#include <iostream>
using namespace std;
#include<list>
void printlist(const list<int>&l)
{
	for (list<int>::const_iterator it = l.begin();it != l.end();it++)
	{
		cout << *it << " ";
	}
	cout << endl;
}
void test01()
{
	//创建list容器
	list<int>l1;//默认构造
	//添加数据
	l1.push_back(10);
	l1.push_back(20);
	l1.push_back(30);
	l1.push_back(40);
	l1.push_back(50);

	//遍历容器
	printlist(l1);
	//区间方式构造
	list<int>l2(l1.begin(), l1.end());
	printlist(l2);

	//拷贝构造
	list<int>l3(l2);
	printlist(l3);

	//n个elem
	list<int>l4(10, 1000);
	printlist(l4);
}
int main()
{
	
	test01();

		return 0;
}
- 总结：list容器同其他几个STL常用容器基本一致，熟练掌握即可
```
## 191、list赋值和交换
- 描述：给list容器进行赋值，以及交换list容器

函数原型：
- assing(beg,end);`将(beg end)区间中数据拷贝赋值自身`
- assing(n,elelm);`将n个elem拷贝赋值给本身`
- list& oerator=(const list &lis);`重载等号操作符`
- swap(lst);`将lst与本身的元素互换`
```c++
#include <iostream>
using namespace std;
#include<list>
//list赋值和交换
void printlist(list<int>& l)
{
	for (list<int>::iterator it = l.begin();it != l.end();it++)
	{
		cout << *it <<" ";

	}
	cout << endl;
}
//赋值
void test01()
{
	list<int>l1;
	l1.push_back(10);
	l1.push_back(20);
	l1.push_back(30);
	l1.push_back(40);

	printlist(l1);

	list<int>l2;
	l2 = l1;//oerator=方式赋值
	printlist(l2);

	list<int>l3;
	l3.assign(l2.begin(),l2.end());
	printlist(l3);

	list<int>l4;
	l4.assign(10, 100);
	printlist(l4);
}
//交换
void test02()
{

	list<int>l1;
	l1.push_back(10);
	l1.push_back(20);
	l1.push_back(30);
	l1.push_back(40);

	list<int>l2;
	l2.assign(10, 100);

	cout << "交换前" << endl;
	printlist(l1);
	printlist(l2);

	l1.swap(l2);
	cout << "交换后" << endl;
	printlist(l1);
	printlist(l2);
}
int main()
{
	//test01();
	test02();
	return 0;
}
```
## 192、list大小操作
- 描述：对list容器的大小进行操作

函数原型
- size();`返回容器中元素的个数`
- empty();`判断容器是否为空`
- resize(num);`重新指定容器对象为num，若容器变长，则以默认值填充新位置，如果变短就会删除末尾超出容器长度的元素`
- resize(num,elem);`重新指定容器对象为num，若容器变长，则以elem填充新位置，如果变短就会删除末尾超出容器长度的元素`
```c++
#include <iostream>
using namespace std;
#include<list>
void printlist(list<int>& l)
{
	for (list<int>::iterator it = l.begin();it != l.end();it++)
	{
		cout << *it << " ";
	}
	cout << endl;
}
void test01()
{
	list<int>l1;
	l1.push_back(10);
	l1.push_back(20);
	l1.push_back(30);
	l1.push_back(40);
	printlist(l1);

	cout <<"元素个数；"<< l1.size() << endl;
	//判断容器是否为空
	if(l1.empty())
	{
		cout << "元素为空" << endl;
	}
	else 
	{
		cout << "元素不为空" << endl;
	}
	
	//重新指定大小
	l1.resize(10,1000);
	printlist(l1);



}
int main()
{
	test01();
	
	return 0;
}
```
## 193、list插入和删除
- 描述：对list容器进行数据的插入和删除

函数原型
- push_back(elem);`尾部加入元素`
 - pop_back();`删除容器中最后一个元素`
 - push_front(elem);`在容器开头插入一个元素`
 - pop_front();`从容器开头移除第一个元素`
 - insert(pos,elem);`在pos位置插elem元素拷贝，返回新数据的位置`
 - insert(  pos,n,elem);`在pos位置插入n个elem数据，无返回值`
 - insert( pos,beg,end);`在pos插入（beg end）区间数据，无返回值`
 - clear();`移除容器的所有数据`
 - erase(beg,end);`删除(beg end)区间的数据，返回下一个数据位置`
 - erase(pos);`删除pos位置的数据，并返回下一个数据位置`
 - remove(elem);`删除容器中所有与elem值匹配的元素`
 ```c++
 #include <iostream>
using namespace std;
#include<list>
//list容器插入和删除

void printlist(list<int>& l)
{
	for (list<int>::iterator it = l.begin();it != l.end();it++)
	{
		cout << *it <<" ";
	}
	cout << endl;
}
void test01()
{
	list<int>l;

	//尾插
	l.push_back(10);
	l.push_back(20);
	l.push_back(30);
	//头插
	l.push_front(100);
	l.push_front(200);
	l.push_front(300);

	//300 200 100 10 20 30
	printlist(l);

	//尾删
	l.pop_back();
	printlist(l);
	//头删
	l.pop_front();
	printlist(l);

	//insert插入
	list<int>::iterator it = l.begin();
	l.insert(++it, 1, 1000);
	printlist(l);

	//删除
	it = l.begin();
	l.erase(++it);
	printlist(l);

	//移除
	l.push_back(10000);
	printlist(l);
	l.remove(10000);
	printlist(l);

	//清空
	l.clear();
	printlist(l);

}
int main()
{
	test01();
	
	return 0;
}
 ```
 - 总结：
 - 尾插--push_back
 - 尾删--pop_back
 - 头插--push_front
 - 头删--pop_front
 - 插入--insert
 - 移除--remove
 - 清空--clear
 - 
 ## 194、数据存取
 - 描述；对list容器中数据进行存取

 函数原型
 - front();`返回第一个元素`
 - back();`返回最后一个元素`
 ```c++
 #include <iostream>
using namespace std;
#include<list>

//容器数据获取
void test01()
{
	list<int>l1;
	l1.push_back(10);
	l1.push_back(20);
	l1.push_back(30);
	l1.push_back(40);
	
	//l1[0]不可以用[]方式访问容器中元素
	//l1.at(0)不可以用at方式访问list容器中元素
	//	原因是list本质是链表，每个数据不是用连续的线性空间存储数据，迭代器也是不支持随机访问的
	cout << "第一个元素为；" << l1.front() << endl;
	cout << "最后一个元素为； " << l1.back() << endl;

	//验证迭代器不支持随机访问
	list<int>::iterator it = l1.begin();
	it++;//支持双向
	//it+1;不支持随机访问
}
int main()
{
	test01();
	
	return 0;
}
 ```
 ## 195、list反转和排序
 - 描述；将容器中的元素反转，以及将容器中的数据进行排序

 函数原型；
 - reverse();`反转链表`
 - sort();`链表顺序`
 ```c++
 #include <iostream>
using namespace std;
#include<list>
#include<algorithm>
//list容器的反转和排序
void printlist(const list<int>& L)
{
	for (list<int>::const_iterator it = L.begin();it != L.end();it++)
	{
		cout << *it << " ";
	}
	cout << endl;
}
void test01()
{
	
	//反转
	list<int>L1;
	L1.push_back(30);
	L1.push_back(10);
	L1.push_back(40);
	L1.push_back(20);

	cout << "反转前" << endl;
	printlist(L1);

	//反转后
	L1.reverse();
	cout << "反转后" << endl;
	printlist(L1);
	
}

bool myCompare(int V1,int V2)
{
//降序 就让第一个数>第二个数
	return V1 > V2;

}
//排序
void test02()
{
	list<int>L1;
	L1.push_back(30);
	L1.push_back(10);
	L1.push_back(40);
	L1.push_back(20);
	//排序前
	cout << "排序前" << endl;
	printlist(L1);

	//所有不支持随机访问迭代器的容器，不可以用标准算法
	//不支持随机访问迭代器的容器，内部会提供对应的算法
	//sort(L1.begin(), L1.end());
	L1.sort();//默认排序规则 从小到大 升序
	cout << "排序后" << endl;
	printlist(L1);

	L1.sort(myCompare);
	printlist(L1);
}
int main()
{
	//test01();
	test02();
	return 0;
}
```
## 196、list排序案例
- 描述;将person自定义随机类型排序，person中属性有姓名，年龄，身高
- 排序规则：按照年龄进行升序，如果年龄相同按照身高继续降序
```c++
#include<iostream>
using namespace std;
#include<list>
#include<algorithm>
//list容器 排序案例 对于自定义数据类型 做排序
//排序规则：按照年龄进行升序，如果年龄相同按照身高继续降序
class person
{
public:
	person(string name,int age,int height)
	{
		this->m_Name = name;
		this->m_Age = age;
		this->m_Height = height;
	}
	string m_Name;
	int m_Age;
	int m_Height;

};
//指定排序规则
bool  myComer(person &p1,person &p2)
{
	//按照年龄升序
	if (p1.m_Age == p2.m_Age)
	{
		//年龄相同按照身高降序
		return p1.m_Height > p1.m_Height;
	}
	else
	{
		return p1.m_Age < p2.m_Age;
	}
}
void test01()
{
	list<person>L1;
	//准备数据
	person p1("刘备", 35, 175);
	person p2("关羽", 44, 200);
	person p3("张飞", 54, 160);
	person p4("马超", 63, 180);
	person p5("李白", 35, 190);
	person p6("孙权", 35, 170);
	//插入数据
	L1.push_back(p1);
	L1.push_back(p2);
	L1.push_back(p3);
	L1.push_back(p4);
	L1.push_back(p5);
	L1.push_back(p6);
	for (list<person>::iterator it=L1.begin();it!=L1.end();it++)
	{
		cout <<"姓名； "<< (*it).m_Name <<"年龄； "<< (*it).m_Age << "身高； "<<(*it).m_Height << endl;
	}
	//排序
	cout << "----------" << endl;
	cout << "排序后" << endl;
	L1.sort(myComer);
	for (list<person>::iterator it = L1.begin();it != L1.end();it++)
	{
		cout << "姓名； " << (*it).m_Name << "年龄； " << (*it).m_Age << "身高； " << (*it).m_Height << endl;
	}
}
int main()
{
	test01();
	return 0;
}
```
- 总结：
- 对于自定义数据类型，必须要指定排序规则，否则编译器不知道如何进行排序
 - 高级排序只是在排序规则上在进行一次逻辑规则制定
# set/multiset容器
set容器基本概念
- 简介：所有元素都会在插入时自动被排序

本质；
- set/multiset`属于关联式容器`，底层结构是用`二叉树`实现

set和multiset区别
- set不允许容器中有重复的元素
- multiset允许容器中有重复的元素
## 197、set构造和赋值
- 描述：创建set容器以及赋值

构造
- set<T>st;`默认构造函数`
- set(const set &st);`拷贝构造函数`

赋值
- set oerator=(const set &st);`重载等号赋值`
```c++
#include<iostream>
using namespace std;
#include<set>
//set容器构造和赋值
void printset(set<int>&s)
{
	for (set<int>::iterator it = s.begin();it != s.end();it++)
	{
		cout << *it << " ";
	}
	cout << endl;

}
void test01()
{
	set<int>s1;
	//插入数据只能用insert
	s1.insert(10);
	s1.insert(40);
	s1.insert(30);
	s1.insert(20);
	s1.insert(30);
	//遍历容器
	//set容器特点：所有元素插入时会自动排序 且不允许有重复元素
	printset(s1);
	//拷贝构造
	set<int>s2(s1);
	printset(s2);
	//赋值
	set<int>s3;
	s3 = s2;
	printset(s3);
}
int main()
{
	test01();

	return 0;
}
- 总结：
- set容器插入时要用insert
- set容器插入时会自动排序
```
## 198、set大小和交换
- 描述：条件set容器大小以及交换

函数原型
- size();`返回容器中元素的数目`
- empty();`判断容器是否为空`
- swap();`交换两个集合容器`
```c++
#include<iostream>
using namespace std;
#include<set>
void printset(set<int>&s)
{
	for (set<int>::const_iterator it = s.begin();it != s.end();it++)
	{
		cout << *it <<" ";
	}
	cout << endl;
}
//大小
void test01()
{
	set<int>s1;
	//插入数据
	s1.insert(10);
	s1.insert(30);
	s1.insert(50);
	s1.insert(40);
	s1.insert(20);
	//打印容器
	printset(s1);
	
	cout << "s1的大小为； " << s1.size() << endl;
	//判断是否为空
	if (!s1.empty())
	{
		cout << "s1不为空" << endl;
	}
	else
	{
		cout << "s1为空" << endl;
	}

	
}
//交换
void test02()
{
	set<int>s1;

	//插入数据
	s1.insert(10);
	s1.insert(30);
	s1.insert(50);
	s1.insert(40);
	s1.insert(20);

	set<int>s2;

	//插入数据
	s2.insert(100);
	s2.insert(300);
	s2.insert(500);
	s2.insert(400);
	s2.insert(200);
	cout << "交换前" << endl;
	printset(s1);
	printset(s2);

	cout << "交换后" << endl;
	s1.swap(s2);
	printset(s1);
	printset(s2);
}
int main()
{
	//test01();
	test02();
	return 0;
}
-总结
统计大小--size
判断是否为空--empty
交换--swap
```
## 199、set插入和删除
- 描述：set容器进行插入和删除

函数原型
- insert(elem);`在容器中插入数据`
- clear();`清除所有元素`
- erase(pos);`删除pos迭代器所指的元素，返回下一个元素迭代器`
- erase(beg end);`删除区间（beg end）的所有元素，并返回下一个元素的迭代器`
- erase(elem);`删除·容器中值为elem的元素`
```c++
#include<iostream>
using namespace std;
#include<set>
void printset(set<int>& s)
{
	for (set<int>::iterator it = s.begin();it != s.end();it++)
	{
		cout << *it <<" ";
	}
	cout << endl;
}
void test01()
{
	set<int>s1;
	s1.insert(10);
	s1.insert(30);
	s1.insert(40);
	s1.insert(20);
	//遍历
	printset(s1);

	//删除
	s1.erase(s1.begin());
	printset(s1);

	//删除重载版本
	s1.erase(20);
	printset(s1);

	//清空
	s1.clear();
	printset(s1);
}
int main()
{
	test01();
	
	return 0;
}
```
## 200、set查找和统计
- 描述：对set容器进行查找数据和统计数据

函数原型
- find(key);`查找key是否存在，返回该键的元素的迭代器，如果不存在，返回set,end();`
- count(key);`统计key的元素个数`
```c++
#include<iostream>
using namespace std;
#include<set>
void test01()
{
	set<int>s;
	//插入
	s.insert(10);
	s.insert(30);
	s.insert(20);
	s.insert(40);
	//查找
	set<int>::iterator pos=s.find(40);
	if (pos != s.end())
	{
		cout << "找到元素" <<*pos<< endl;
	}
	else
	{
		cout << "未找到" << endl;
	}
	

}
//统计
void test02()
{

	set<int>s;
	//插入
	s.insert(10);
	s.insert(30);
	s.insert(20);
	s.insert(40);
	s.insert(30);
	s.insert(30);
	//统计30的个数
	int num = s.count(30);
	//对于set而已 统计结果要么是0 要么是1
	cout << "num= " << num << endl;
}
int main()
{
	//test01();
	test02();

	return 0;
}
```
## 201、set和mulitset的区别
区别：
- set不可以插入重复数据，而mulitset可以
- set插入数据时会返回插入结果，表示插入是否成功
- mulitset不会检测数据，因此可以重复插入数据
```c++
#include<iostream>
using namespace std;
#include<set>
//set和mulitset区别
void test01()
{
	set<int>s1;
	pair<set<int>::iterator,bool>ret=s1.insert(10);
	if (ret.second)
	{
		cout << "第一次插入成功" << endl;
	}
	else
	{
		cout << "插入失败" << endl;
	}
	ret=s1.insert(10);
	if (ret.second)
	{
		cout << "第二次插入成功" << endl;
	}
	else
	{
		cout << "插入失败" << endl;
	}

	multiset<int>ms;
	//允许插入重复的值
	ms.insert(10);
	ms.insert(10);
	ms.insert(10);
	for (multiset<int>::iterator it = ms.begin();it != ms.end();it++)
	{
		cout << *it << endl;
	}
}
int main()
{
	test01();
	return 0;
}
 总结；
 如果不允许重复插入数据可以用set
 如果需要插入就用multiset
```
## 202、pair对组创建
- 描述：成对出现的数据，利用对组可以返回两个数据

两种创建方式
- pair<type,type>p,(value1,value2);
- pair<type,type>p=make_pair(value1,value2);
```c++
#include<iostream>
using namespace std;
//pair对组的创建
void test01()
{
	//第一种
	pair<string, int>p("刘备", 93);
	cout << "姓名； " << p.first << "年龄" << p.second << endl;

	//第二种
	pair<string, int>p2 = make_pair("jhsd", 30);
	cout << "姓名； " << p2.first << "年龄" << p2.second << endl;
}
int main()
{
	test01();
	return 0;
}
总结；两种都可以创建对组，记住一种即可
```
## 203、setr容器排序1内置数据
主要技术点；
- 利用仿函数，可以改变排序规则
- 示例；Set存放内置数据类型
```c++
#include<iostream>
using namespace std;
#include<set>
#include<algorithm>

class phone
{
public:
	bool  operator()( int v1, int v2)const
	{
		return v1 > v2;
	}

};
void test01()
{
	set<int>s1;

	s1.insert(10);
	s1.insert(40);
	s1.insert(30);
	s1.insert(20);

	for (set<int>::iterator it = s1.begin();it != s1.end();it++)
	{
		cout << *it << endl;
	}
	//指定排序规则从大到小

	set<int,phone>s2;

	s2.insert(100);
	s2.insert(400);
	s2.insert(300);
	s2.insert(200);
	for (set<int,  phone>::iterator it = s2.begin();it != s2.end();it++)
	{
		cout << *it << endl;
	}

}
int main()
{
	test01();
	return 0;
}
总结；利用仿函数可以指定set容器的排序规则
```
## 204、set容器排序2自定义数据类型
- 利用仿函数，可以改变排序规则
示例；set存放自定义数据类型
```c++
#include<iostream>
using namespace std;
#include<set>

class person
{
public:
	person(string name, int age)
	{
		this->m_Name = name;
		this->m_Age = age;
	}
	string m_Name;
	int m_Age;
};
class phone
{
public:
	bool operator()(const person &p1,const person &p2)const
	{
		//按照年龄降序
		return p1.m_Age > p2.m_Age;
	}
};
void test01()
{
	//自定义数据类型，都会指定排序规则
	set<person,phone>s;
	//创建erson对象
	person p1("刘备", 37);
	person p2("关羽", 35);
	person p3("张飞", 40);
	person p4("赵云", 25);
	person p5("马超", 30);

	s.insert(p1);
	s.insert(p2);
	s.insert(p3);
	s.insert(p4);
	s.insert(p5);
	for (set<person,phone>::iterator it = s.begin();it != s.end();it++)
	{
		cout << "姓名； " << it->m_Name <<"年龄； "<< it->m_Age << endl;
		
	}
}
int main()
{
	test01();
	return 0;
}
```
# map/multimap容器
简介：
- 1、map中所有元素都是pair
- 2、pair中第一个元素为key（链值），起到索引作用，第二个元素为value(实值)

本质
- map/multimap容器属于`关联式容器`，底层结构式用二叉树实现

优点
- 可以根据key值快速找到value值

map/multiset区别
- map不允许容器中有重复key值元素
- multimap允许容器中有重复key值元素
## 205、map构造和赋值
- 描述：对map容器进行构造和赋值

函数原型
- map<T1,T2>mp;`map默认构造函数`
- map(const map &mp);`拷贝构造函数`

赋值
- map& operator=(const map &mp);`重载等号操作符`
```c++
#include<iostream>
using namespace std;
#include<map>
void printmap(map<int,int>&m)
{
	for (map<int, int>::iterator it = m.begin();it != m.end();it++)
	{
		cout << "key值= " << (*it).first << "value= " << (*it).second <<" ";
	}
	cout << endl;
}
void test01()
{
	//创建map容器
	map<int,int>m;
	m.insert(pair<int,int>(1,10));
	m.insert(pair<int,int>(3, 30));
	m.insert(pair<int,int>(2, 20));
	m.insert(pair<int,int>(4, 40));

	printmap(m);

	//拷贝构造
	map<int, int>m1(m);
	printmap(m1);

	//赋值构造
	map<int, int>m2;
	m2 = m1;
	printmap(m2);

}
int main()
{
	test01();
	return 0;
}
总结；map容器中所有元素都是成对出现，插入数据时要使用对组
```
## 206、map大小和交换
- 描述：统计map容器大小以及交换map容器

函数原型
- size();`返回容器中元素的数目`
- empty();`判断容器是否为空`
- swap();`交换两个集合容器`
```c++
#include<iostream>
using namespace std;
#include<map>

//大小
void test01()
{
	map<int, int>m;
	m.insert(pair<int,int>(2, 20));
	m.insert(pair<int, int>(4, 40));
	m.insert(pair<int, int>(1, 10));
	m.insert(pair<int, int>(3, 30));
	
	if (m.empty())
	{
		cout << "map为空" << endl;
	}
	else
	{
		cout << "不为空" << endl;
		cout <<"元素个数= "<< m.size() << endl;
	}
}
void printmap(map<int, int>& m)
{
	for (map<int, int>::iterator it = m.begin();it != m.end();it++)
	{
		cout << "key= " << it->first << "value= " << it->second << endl;
	}
	cout << endl;
}
//交换
void test02()
{
	map<int, int>m;
	m.insert(pair<int, int>(2, 20));
	m.insert(pair<int, int>(4, 40));
	m.insert(pair<int, int>(1, 10));
	m.insert(pair<int, int>(3, 30));

	map<int, int>m2;
	m2.insert(pair<int, int>(5, 500));
	m2.insert(pair<int, int>(7, 700));
	m2.insert(pair<int, int>(6, 600));
	m2.insert(pair<int, int>(8, 800));
	cout << "交换前 ;" << endl;
	printmap(m);
	printmap(m2);

	m.swap(m2);
	cout << "交换后 ；" << endl;
	printmap(m);
	printmap(m2);
	

}
int  main()
{
	//test01();
	test02();
	return 0;
}
```
## 207、map插入和删除
- 描述：map容器进行插入数据和删除数据

函数原型
- insert(elem);`在容器中插入数据`
- clear();`清除所有元素`
- erase(pos);`删除pos迭代器所指的元素，返回下一个元素的迭代器`
- erase(beg eng);`删除区间(beg,end)的所有元素，并返回下一个元素的迭代器`
- erase(ley);`删除容器中值为key的元素`
```c++
#include<iostream>
using namespace std;
#include<map>
void printmap(map<int, int>& m)
{
	for (map<int, int>::iterator it = m.begin();it != m.end();it++)
	{
		cout <<"key"<< it->first <<"value"<< it->second <<" ";
	}
	cout << endl;
}
void test01()
{
	map<int, int>m;
	//插入
	//第一种
	m.insert(pair<int, int>(1, 10));
	//第二种
	m.insert(make_pair(2, 20));
	//第三种
	m.insert(map<int, int>::value_type(3, 30));
	//第四种
	m[4] = 40;
	//[]不建议使用 ，用途 可以利用key访问value
	//cout << m[4] << endl;
	printmap(m);

	//删除
	m.erase(m.begin());
	printmap(m);

	m.erase(3);//按照key删除
	printmap(m);

	m.erase(m.begin(), m.end());
	printmap(m);

	m.clear();
	printmap(m);


}
int main()
{
	test01();
	return 0;
}
```
## 208、map容器查找和统计
- 描述：对map容器进行查找数据以及统计数据

函数原型
- find(key);`查找key是否存在，若存在，返回该键的元素迭代器，若不存在，返回set.end()`
- count(key);`统计key的元素个数`
```c++
#include<iostream>
using namespace std;
#include<map>
void test02()
{
	map<int, int>m;
	m.insert(make_pair(1, 10));
	m.insert(make_pair(3, 30));
	m.insert(make_pair(3, 30));
	m.insert(make_pair(2, 20));
	//查找
	map<int, int>::iterator pos = m.find(3);
	if (pos != m.end())
	{
		cout << "key找到元素= " << (*pos).first << "value= " << (*pos).second << endl;
	}
	else
	{
		cout << "没找到" << endl;
	}
	//统计
	//map容器不允许插入重复的key元素,count统计而言，要么是0，要么是1
	//multimap统计可能大于1
	int num=m.count(3);
	cout << num << endl;
}
int main()
{
	
	test02();
	return 0;
}
```
## 209、map容器排序
- 目标；map容器排序规则为按照key值进行从小到大排序，掌握如何改变排序规则

主要；利用仿函数，可以改变排序规则
```c++
#include<iostream>
using namespace std;
#include<map>
class myCom
{
public:
	bool operator()(int v1, int v2)const
	{
		//降序
		return v1 > v2;
	}
};
//map容器排序
void test02()
{
	map<int, int,myCom>m;
	m.insert(make_pair<int, int>(1, 10));
	m.insert(make_pair<int, int>(3, 30));
	m.insert(make_pair<int, int>(4, 40));
	m.insert(make_pair<int, int>(2, 20));

	for (map<int, int, myCom>::iterator it = m.begin();it != m.end();it++)
	{
		cout <<"key="<< it->first <<"value= "<< it->second << endl;
	}
	
}
int main()
{
	
	test02();
	return 0;
}
总结；利用仿函数可以指定map容器的排序规则
对于自定义数据类型，map必须要指定排序规则，同set容器
```
## 210、STL--案例2员工分组
案例描述
- 公司招聘10个员工（ABCDEFGHIJK），10名员工进入公司后，需要指派员工在哪个部门工作
- 员工信息有：姓名，工资组成；部门分为策划，美术，研发
- 随机给员工分配部门和工资
- 通过multimap进行信息插入 key(部门编号)value(员工)
- 分部门显示员工信息

实现步骤
-， 1、创建10名员工，放到vector
- 2、遍历vector容器，取出每个员工，进行随机分配
- 3、分组后，将员工部门编号作为key，具体员工工作为value，放入multimap容器中
- 4、分部门显示员工信息
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<map>
#define CEHUA 0
#define MEISHU 1
#define YANFA 2
class Person
{
public:
	
	string m_Name;
	int m_Wage;

};
void printperson(vector<Person>&v)
{
	string nameSeed = "ABCDEFGHIJ";
	for (int i = 0;i < 10;i++)
	{
		Person p;
		p.m_Name = "员工";
		p.m_Name += nameSeed[i];

		p.m_Wage = rand() % 10000 + 10000;//10000~19999
		//将员工放到容器中
		v.push_back(p);
	}
	
}
//员工分组
void setGroup(vector<Person>&v,multimap<int ,Person>&m)
{
	for (vector<Person>::iterator it = v.begin();it != v.end();it++)
	{
		//产生随机部门编号
		int deptId = rand() % 3;//产生0~2
		//将员工插入到分组中
		m.insert(make_pair(deptId, *it));//key代表部门编号，value代表具体员工
	}
}
//分组显示
void showWork(multimap<int,Person>&m)
{
	//0   A  B  C  E  2  F  G...
	cout << "策划部门; " << endl;
multimap<int,Person>::iterator pos=m.find(CEHUA);
int count = m.count(CEHUA);//统计策划部门总共多少人
int index = 0;
for (;pos != m.end() && index<count;pos++,index++)
{
	cout << "姓名； " << pos->second.m_Name << "工资； " << pos->second.m_Wage << endl;
}
cout << "----------------" << endl;
cout << "美术部门；" << endl;
pos = m.find(MEISHU);
count = m.count(MEISHU);//统计美术部门总共多少人
 index = 0;
for (;pos != m.end() && index < count;pos++, index++)
{
	cout << "姓名； " << pos->second.m_Name << "工资； " << pos->second.m_Wage << endl;
}
cout << "-----------------" << endl;
cout << "研发部门； " << endl;
pos = m.find(YANFA);
count = m.count(YANFA);//统计研发部门总共多少人
index = 0;
for (;pos != m.end() && index < count;pos++, index++)
{
	cout << "姓名； " << pos->second.m_Name << "工资； " << pos->second.m_Wage << endl;
}

}
int main()
{
	srand((unsigned int)time(NULL));
	//1、创建员工
	vector<Person>v1;
	printperson(v1);
	//2、员工分组
	multimap<int,Person>mperson;
	setGroup(v1, mperson);
	//3、分组显示
	showWork(mperson);
	
	return 0;
}
```
# STL-函数对象
概念：
- 重载`函数调用操作符`的类，其对象常称为`函数对象`
- `函数对象`使用重载的()时，行为类似函数调用，也叫`仿函数`

本质
- 函数对象（仿函数）是一个类，不是一个函数
## 211、函数对象使用
特点；
- 函数对象在使用时，可以像普通函数那样调用，可以有参数，可以有返回值
- 函数对象超出普通函数的概念，函数对象可以有自己状态
- 函数对象可以作为参数传递
```c++
#include<iostream>
using namespace std;
//函数对象(仿函数)
//1、函数对象在使用时，可以像普通函数那样调用，可以有参数，可以有返回值
class MyAdd
{
public:
	int operator()(int v1,int v2)const
	{
		return v1 + v2;
	}
};
void test01()
{
	MyAdd myadd;//函数对象
	cout <<myadd(10, 10)<<endl;
}


//2、函数对象超出普通函数的概念，函数对象可以有自己状态
class MyPrint
{
public:
	MyPrint()
	{
		this->count = 0;
	}
	void operator()(string test)
	{
		cout << test << endl;
		this->count++;
	}
	int count;//记录内部状态
};
void test02()
{
	MyPrint myprint;
	myprint("hello world");
	myprint("hello world");
	myprint("hello world");
	myprint("hello world");
	myprint("hello world");
	cout << "MyPrint调用次数为； " << myprint.count << endl;
}


//3、函数对象可以作为参数传递
void doprint(MyPrint &mp,string test)
{
	mp(test);
}
void test03()
{
	MyPrint myprint;
	doprint(myprint, "hello c++");

}
int main()
{
	//test01();
	//test02();
	test03();
	return 0;
}
总结
仿函数非常灵活，可以作为参数进行传递
```
## 212、谓词
概念 
- 返回bool类型的仿函数称为`谓词`
- 如果operator()接受一个参数，那么叫做一元谓词
- 如果operator()接受两个参数，那么叫做二元谓词
```c++
#include <iostream>
using namespace std;
#include<vector>
#include<algorithm>
//返回bool类型的仿函数称为`谓词`
//一元谓词
class phone
{
public:
	bool operator()(int val)
	{
		return val > 5;
	}
};
void test01()
{
	vector<int>v;
	for (int i = 0;i < 10;i++)
	{
		v.push_back(i);
	}
	//查找容器中 有没有大于5的数字
	//phone()匿名对象
	vector<int>::iterator it =find_if(v.begin(), v.end(),phone());
	if (it == v.end())
	{
		cout << "未找到" << endl;
	}
	else
	{
		cout << "找到了大于5的数字" << *it << endl;
	}
}
int main()
{

	test01();
	return 0;
}
```
## 213、二元谓词
-  如果operator()接受两个参数，那么叫做二元谓词
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<algorithm>
//二元谓词
class person
{
public:
	bool operator()(int v1, int v2)
	{
		return v1 > v2;
	}
};
void test01()
{
	vector<int>v1;
	v1.push_back(10);
	v1.push_back(50);
	v1.push_back(30);
	v1.push_back(20);
	v1.push_back(40);

	sort(v1.begin(),v1.end());
	for (vector<int>::iterator it = v1.begin();it != v1.end();it++)
	{
		cout << *it << " ";
	}
	cout << endl;
	//使用函数对象  改变算法策略 变为排序规则从大到小
	sort(v1.begin(), v1.end(), person());
	cout << "----------------" << endl;
	for (vector<int>::iterator it = v1.begin();it != v1.end();it++)
	{
		cout << *it << " ";
	}
	cout << endl;
}
int main()
{
	test01();
	return 0;
}
总结；参数只有两个的谓词称为二元谓词
```
## 内建函数对象
概念； 
- STL内建了一种函数对象

分类
- 算数仿函数
- 关系仿函数
- 逻辑仿函数

用法
- 这些仿函数函数所产生的对象，用法和普通函数用法完全相同
- 这些内建函数对象，需要引用头文件`#include<functional`
## 214、算数仿函数
描述； 
- 实现四则运算
- 其中negate是一元运算，其他都是二元运算

仿函数原型
- template<class T>T plus<T>`加法仿函数`
- template<class T>T minus<t>`减法仿函数`
- template<class T>T multiplies<T>`乘法仿函数`
- template<class T>T divides<T>`除法仿函数`
- template<class T>T modulus<T>`取模仿函数`
- template<class T>T negate<T>`取反仿函数`
```c++
#include<iostream>
using namespace std;
#include<functional>//内建函数对象头文件
//内建函数对象 算数仿函数
//negate 一元仿函数 取反仿函数
void test01()
{
	negate<int>n;
	n(50);
	cout << n(50) << endl;

}
//plus 二元仿函数 加法
void test02()
{
	plus<int>p;
	cout << p(10, 59) << endl;
}
int main()
{
	test01();
	test02();
	return 0;
}
```
## 215、关系仿函数
- 描述：实现关系化对比

仿函数原型
- temalate<class T>bool equal_to<t>`等于`
temalate<class T>bool not_equal_to<T>`不等于`
temalate<class T>bool greater<T>`大于`
temalate<class T>bool greater_equal<T>`大于等于`
temalate<class T>bool less<T>`小于`
temalate<class T>bool less_equal<t>`小于等于`
```c++
#include<iostream>
using namespace std;
#include<functional>
#include<vector>
#include<algorithm>
//内建函数对象 仿函数
//大于gerator
class person
{
public:
	bool operator()(int v1, int v2)
	{
		return v1 > v2;
	}
};
void test01()
{
	vector<int>v;
	v.push_back(10);
	v.push_back(30);
	v.push_back(50);
	v.push_back(20);
	v.push_back(40);
	for (vector<int>::iterator it = v.begin();it != v.end();it++)
	{
		cout << *it << " ";
	}
	cout << endl;
	//降序
	//sort(v.begin(), v.end(),person());
	//greater()内建函数对象
	sort(v.begin(), v.end(), greater<int>());
	for (vector<int>::iterator it = v.begin();it != v.end();it++)
	{
		cout << *it << " ";
	}
}
int main()
{
	test01();
	return 0;
}
总结；关系仿函数最常用的是`gerater<>大于`
```
## 216、逻辑仿函数
描述：实现逻辑运算

函数原型
- temlate<class T> bool logical_and<T>`逻辑与`
temlate<class T> bool logical_or<T>`逻辑或`
temlate<class T> bool logical_not<T>`逻辑非`
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<functional>
#include<algorithm>
//内建函数对象 逻辑仿函数
//逻辑非 logical_n

void test01()
{
	vector<bool>v;
	v.push_back(true);
	v.push_back(false);
	v.push_back(true);
	v.push_back(false);

	for (vector<bool>::iterator it = v.begin();it != v.end();it++)
	{
		cout << *it << " ";
	}
	cout << endl;

	//利用逻辑非  将容器v搬运到容器v2中，并执行取反操作
	vector<bool>v2;
	v2.resize(v.size());
	transform(v.begin(), v.end(), v2.begin(),logical_not<bool>());
	for (vector<bool>::iterator it = v2.begin();it != v2.end();it++)
	{
		cout << *it << " ";
	}
	cout << endl;
}
int main()
{
	test01();

	return 0;
}
```
# 常用算法
概述；
- 算法主要是由头文件<algorithm>,<functional>,<numeric>
- <algorithm>在所有STL头文件中最大的一个，范围涉及到比较，交换，查找，遍历操作，复制，修改等等
- <numeric>体积很小，只包括几个序列上面进行简单数学运算的模板函数
- <functional>定义了一些模板类，用以声明函数对象
.
## 217、常用遍历算法
- 学习目标
- 掌握常用的遍历算法

算法简介
- for_each`遍历容器`
- transform`搬运容器到另一个容器中`
#### for_each

- for_each(iterator beg,iterator end,_func)
- 遍历算法 遍历容器元素
- beg 开始迭代器
- end 结束迭代器
- _func 函数或者函数对象
```c++
#include<iostream>
using namespace std;
#include<algorithm>
#include<vector>
//普通函数
void print01(int val)
{
	cout << val << " ";
	
}
//仿函数
class print02
{
	public:
		void operator()(int val)
		{
			cout << val << " ";
			
		}
	
};
void test01()
{
	vector<int>v;
	
	for (int i = 0;i < 10;i++)
	{
		v.push_back(i);
	}
	for_each(v.begin(), v.end(), print01);
	cout << endl;
	for_each(v.begin(), v.end(), print02());
	cout << endl;

}
int main()
{
	test01();
	return 0;
}
总结：for_each在实际开发中是最常用的遍历算法，需要熟练掌握
```
## 218、transform
描述;搬运容器到另一个容器中

函数原型
- transform(iterator beg1,iterator end1,tierator beg2,_func)
- beg1`原容器开始迭代`
- end1`源容器结束迭代`
- beg2`目标容器开始迭代`
- _func`函数或者函数对象`
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<algorithm>
class print01
{
public:
	int operator()(int v)
	{
		return v+100;
	}
};

class print02
{
public:
	void operator()(int val)
	{
		cout << val << " ";
}
};
void test01()
{
	vector<int>v;
	for (int i = 0;i < 10;i++)
	{
	v.push_back(i);
	}
	vector<int>v2;//目标容器
	v2.resize(v.size());//目标容器需要提前开辟空间
	transform(v.begin(), v.end(), v2.begin(),print01());
	for_each(v2.begin(), v2.end(), print02());
	cout << endl;
}
int main()
{
	test01();
	return 0;
}
搬运目标容器必须提前开辟新空间，否则无法运行
```
# 常用查找算法
算法简介
- find`查找元素`
- find_if`按条件查找元素`
- adjacend_find`查找相邻重复元素`
- binary_search`二分查找法`
- count`统计元素个数`
- count_if`按条件查找元素个数`
## 219、find
描述；查找指定元素，找到返回指定元素迭代器，找不到返回结束迭代器

函数原型
- find(tireator beg,iterator end,value)
beg`开始迭代器`
end`结束迭代器`
value`查找的元素`
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<algorithm>
//常用查找算法
//find
//查找内置数据类型
void test01()
{
	vector<int>v;
	for (int i = 0;i < 10;i++)
	{
		v.push_back(i);
	}
	//查找容器是否有5
	vector<int>::iterator it=find(v.begin(), v.end(), 5);
	if (it == v.end())
	{
		cout << "未找到 " << endl;
	}
	else
	{
		cout << "找到了;"<<*it << endl;
	}
}


class person
{
public:
	person (string name,int age)
	{
		this->m_Name = name;
		this->m_Age = age;
	}
	//重载== 底层find知道如何对比person数据类型
	bool operator==(const person& p)
	{
		if (this->m_Name == p.m_Name && this->m_Age == p.m_Age)
		{
			return true;
		}
		else
		{
			return false;
		}
	}
	string m_Name;
	int m_Age;
};
//查找自定义数据类型
void test02()
{
	vector<person>p;
	//创建数据
	person p1("aa", 10);
	person p2("bb", 20);
	person p3("cc", 40);
	person p4("dd", 30);
	//放入容器
	p.push_back(p1);
	p.push_back(p2);
	p.push_back(p3);
	p.push_back(p4);

	person pp("bb", 20);
	vector<person>::iterator it=find(p.begin(), p.end(), pp);
	if (it == p.end())
	{
		cout << "未找到" << endl;
	}
	else
	{
		cout << "找到了姓名；" << it->m_Name<<"年龄；" << it->m_Age << endl;
	}


}
int main()
{
	//test01();
	test02();
	return 0;
}
总结：利用返回值find可以在容器中找到指定元素，返回值是迭代器
```
## 220、find_if
描述；按条件查找元素

函数原型
- find_if(iterator beg,tierator end,_pred)
- 按值查找元素，找到返回值指定位置迭代器，找不到返回结束迭代器位置
- beg`开始迭代器`
- end`结束迭代器`
- _pred`函数或者谓词（返回bool类型的仿函数）`
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<algorithm>
//内置数据类型
class persons
{
public:
	bool operator()(int val)
	{
		return val > 5;
	}
};
void test01()
{
	vector<int>v;
	for (int i = 0;i < 10;i++)
	{
		v.push_back(i);
	}
	vector<int>::iterator it = find_if(v.begin(), v.end(), persons());
	if (it == v.end())
	{
		cout << "未找到" << endl;
	}
	else
	{
		cout << "找到元素" << *it << endl;
	}
}
//自定义数据类型
class person
{
public:
	person(string name,int age)
	{
		this->m_Name = name;
		this->m_Age = age;
	}
	string m_Name;
	int m_Age;
};
class print
{
public:
	bool operator()(person &p)
	{
		return p.m_Age > 20;
	}
};
void test02()
{
	vector<person>v;
	person p1("aa", 10);
	person p2("bb", 20);
	person p3("cc", 30);

	v.push_back(p1);
	v.push_back(p2);
	v.push_back(p3);
	//找到年龄>20
	vector<person>::iterator it=find_if(v.begin(), v.end(), print());
	if (it == v.end())
	{
		cout << "未找到" << endl;
	}
	else
	{
		cout << "找到姓名； " << it->m_Name << "年龄; " << it->m_Age << endl;
	}
}
int main()
{
	//test01();
	test02();
	return 0;
}
```
## 221、adjacent_find
- 描述：查找相邻重复元素

函数原型
- adjacent_find(iterator beg,iterator end);
- 查找相邻重复元素，返回相邻元素的第一个位置的迭代器
- beg`开始迭代器`
- end`结束迭代器`
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<algorithm>
void test01()
{
	vector<int>v;
	v.push_back(0);
	v.push_back(1);
	v.push_back(3);
	v.push_back(3);
	v.push_back(2);
	v.push_back(0);
	vector<int>::iterator pos = adjacent_find(v.begin(), v.end());
	if (pos == v.end())
	{
		cout << "未找到相邻重复元素" << endl;
	}
	else
	{
		cout << "找到相邻重复元素；" <<*pos<< endl;
	}
}
int main()
{
	test01();
	return 0;
}
查找相邻元素用STL中的adjacent_find算法
```
## 222、binary_search
描述；找到指定元素是否存在

函数原型
- bool binary_search(iterator beg,iterator end,vaue)
- 查找指定元素，查到返回true否则返回false
- 注意无序序列中不可以
- beg`开始迭代器`
- end`结束迭代器`
- value`查找的元素`
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<algorithm>
//常用查找算法
void test01()
{
	vector<int>v;
	for (int i = 0;i < 10;i++)
	{
		v.push_back(i);
	}
	//v.push_back(2); 如果是无序序列 结果未知！
	//查找容器中是否有9
	//注意;容器必须有序序列
	bool ret=binary_search(v.begin(), v.end(), 9);
	if (ret)
	{
		cout << "找到" << endl;
	}
	else
	{
		cout << "未找到" << endl;
	}
}
int main()
{
	test01();
	return 0;
}
总结：二分查找效率很高，但是查找容器必须有序序列
```
## 223、count
描述：统计元素个数

函数原型
- count(iterator beg,iterator end,value)
- 统计元素出现次数
- beg`开始迭代器`
- end`结束迭代器`
- value`查找的元素`
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<algorithm>
//统计内置数据类型
void test01()
{
	vector<int>v;
	v.push_back(10);
	v.push_back(20);
	v.push_back(40);
	v.push_back(40);
	v.push_back(20);
	int num=count(v.begin(), v.end(), 40);
	cout <<"40的元素个数为；"<< num << endl;
}
//统计自定义数据类型
class person
{
public:
	person(string name,int age)
	{
		this->m_Name = name;
		this->m_Age = age;
	}
	bool operator == (const person & v)
	{
		if (this->m_Age == v.m_Age)
		{
			return true;
		}
		else
			return false;
	}
	string m_Name;
	int m_Age;
};
void test02()
{
	vector<person>v;
	person p1("刘备",20);
	person p2("关羽",30);
	person p3("诸葛亮", 40);
	person p4("张飞", 20);
	person p5("赵云", 30);

	v.push_back(p1);
	v.push_back(p2);
	v.push_back(p3);
	v.push_back(p4);
	v.push_back(p5);

	person p("李白", 20);
	int num = count(v.begin(), v.end(),p );
	cout << "和李白同岁的人有； " << num << endl;
}
int main()
{
	//test01();
	test02();
	return 0;
}
统计自定义数据类型的时候需要配合重载operator==
```
## 224.count_if
- 描述：按照条件统计元素个数

函数原型
- count_if(iterator beg,iterator end,_pred)
- 按条件统计元素出现次数
- beg`开始迭代器`
- end`结束迭代器`
- _pread`谓词`
```c++
#include <iostream>
#include<vector>
#include<algorithm>
using namespace std;
//1、统计内置数据类型
class persons
{
public:
	bool operator()(int val)
	{
		return val > 20;
	}
	
};
void test01()
{
	vector<int>v;
	v.push_back(10);
	v.push_back(40);
	v.push_back(20);
	v.push_back(30);
	v.push_back(20);
	int num=count_if(v.begin(), v.end(), persons());
	cout << num << endl;
}
//2、统计自定义数据类型

class person
{
public:
	person(string name,int age)
	{
		this->m_Name = name;
		this->m_Age = age;
	}
	string m_Name;
	int m_Age;

};
class person1
{
public:
	bool operator()(const person& v)
	{
		return v.m_Age > 20;
	}
};
void test02()
{
	vector<person>v;
	person p1("刘备", 40);
	person p2("开始", 30);
	person p3("隐士", 40);
	person p4("难怪", 30);
	person p5("zgf", 50);

	v.push_back(p1);
	v.push_back(p2);
	v.push_back(p3);
	v.push_back(p4);
	v.push_back(p5);
	//统计大于20的人员个数
	int num=count_if(v.begin(), v.end(), person1());
	cout << "大于20的人员有；" << num << endl;
}
int main()
{
	//test01();
	test02();
	return 0;
}
```
# 常用排序算法
算法简介
- sort`对容器内元素进行排序`
- rand_shuffle`洗牌指定范围内的元素数据调整次序`
- merge`容器元素合并，并存储到另一个容器中`
- reverse`反转指定范围的元素`
## 225、sort
描述：对容器内元素进行排序

函数原型
- sort(iterator beg iterator end,_pred)
- 按值查找元素，找到并返回指定位置迭代器，找不到符号结束迭代器位置
- beg`开始迭代器`
- end`结束迭代器`
- _pread`谓词`
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<algorithm>
#include<functional>
void person(int val)
{
	cout << val << endl;
};
void test01()
{

	vector<int>v;
	v.push_back(40);
	v.push_back(10);
	v.push_back(30);
	v.push_back(20);
	v.push_back(50);
	//利用sort进行排序
	sort(v.begin(), v.end());
	for_each(v.begin(), v.end(), person);
	cout << endl;
	//改变为降序
	sort(v.begin(), v.end(), greater<int>());
	for_each(v.begin(), v.end(), person);
	cout << endl;
}
int main()
{
	test01();
	return 0;
}
sort是最常用的算法之一，需要熟练掌握
```
## 226、random_shuffle
- 描述;指定范围内的元素随机调整次序

函数原型
- rand_shuffle(iterator beg,iterator end)
- 指定范围内的元素随机调整次序
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<algorithm>
void person(int val)
{
	cout << val <<" ";
}
void test01()
{
	srand((unsigned int)time(NULL));
	vector<int>v;
	for (int i = 0;i < 10;i++)
	{
		v.push_back(i);
	}
	//利用洗牌打乱顺序
	random_shuffle(v.begin(), v.end());
	for_each(v.begin(), v.end(), person);
	cout << endl;
}
int main()
{
	
	test01();
	return 0;
}
```
## 227、merge
- 描述：两个元素容器合并，并存储到另一个容器

函数原型
- mergr(iterator beg1,tierator end1,iterator beg2,tierator end2,iterator dest)
- 注意：两个容器必须是有序
- beg1`容器1开始迭代器`
- end1`容器1结束迭代器`
- beg2`容器2开始迭代器`
- end2`容器2结束迭代器`
- dest`目标容器开始迭代器`
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<algorithm>
void person(int val)
{
	cout << val <<" ";
}
void test01()
{
	
	vector<int>v1;
	vector<int>v2;
	for (int i = 0;i < 10;i++)
	{
		v1.push_back(i);
		v2.push_back(i + 1);
	}
	//目标容器
	vector<int>vperson;
	//提前给目标内存分配空间
	vperson.resize(v1.size() + v2.size());

	merge(v1.begin(), v1.end(),v2.begin(), v2.end(),vperson.begin());

	for_each(vperson.begin(), vperson.end(),person);
	cout << endl;
}
int main()
{
	
	test01();
	return 0;
}
```
## 228、reverse
函数原型
- reverse(iterator beg,iterator end)
- 反转指定元素
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<algorithm>
void person(int v1)
{
	cout << v1 << " ";
}
void test01()
{
	vector<int>v;
	v.push_back(10);
	v.push_back(30);
	v.push_back(40);
	v.push_back(20);
	v.push_back(50);
	
	cout << "反转前" << endl;
	for_each(v.begin(), v.end(), person);
	cout << endl;
	cout << "反转后" << endl;
	reverse(v.begin(), v.end());
	for_each(v.begin(), v.end(), person);
	cout << endl;
}
int main()
{
	
	test01();
	return 0;
}
```
# 常用拷贝算法
- 算法简介
- copy`容器内指定范围的元素拷贝到另一个容器中`
- replace`将容器内指定范围的旧元素修改为新元素`
- replace_if`容器内指定范围满足条件的元素替换为新元素`
- swap`互换两个容器的元素`
## 229、copy
描述：容器内指定范围的元素拷贝到另一容器中

函数原型
- copy(iterator beg,iterator end,tierator dest)
- 按值查找元素，找到返回指定位置迭代器，找不到返回结束迭代器位置
- beg`开始迭代器`
- end`结束迭代器`
- dest`目标起始迭代器`
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<algorithm>
void erson(int val)
{
	cout << val << " ";
}
void test01()
{
	vector<int>v1;
	for (int i = 0;i < 10;i++)
	{
		v1.push_back(i);
	}
	vector<int > v2;
	v2.resize(v1.size() + v2.size());
	copy(v1.begin(), v1.end(),v2.begin( ));
	for_each(v2.begin(), v2.end(),erson);
	cout << endl;
}
int main()
{
	test01();
	return 0;
}
利用copy算法时提前开辟空间
```
## 230、repalce
描述：将容器内所指定范围的旧元素修改为新元素

函数原型·
- repalce(iterator beg,iterator end,oldvalue,nemvalue)
- oldvalue`旧元素`
- newvalue`新元素`
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<algorithm>
void erson(int val)
{
	cout << val << " ";
}
void test01()
{
	vector<int>v;
	v.push_back(10);
	v.push_back(10);
	v.push_back(30);
	v.push_back(30);
	v.push_back(40);
	v.push_back(50);
	v.push_back(20);
	cout << "替换前" << endl;
	for_each(v.begin(), v.end(), erson);
	cout << endl;
	//20替换成2000
	replace(v.begin(), v.end(), 30, 2000);
	for_each(v.begin(), v.end(), erson);
	cout << endl;
}
int main()
{
	test01();
	return 0;

}
relace会替换区间满足条件的元素
```
## 231、realce_if
描述：将区间内满足条件的元素，替换成指定元素

函数原型
- repalce_if(iterator beg,iterator end,_pred,newvalue)
- _perd`谓词`
- nevalue`替换的元素`
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<algorithm>
class person
{
public:
	void operator()(int val)
	{
		cout << val << " ";
	}
};
class myprint
{
public:
	bool operator()(int val)
	{
		return val > 30;
	}
};
void test01()
{
	vector<int>v;
	v.push_back(10);
	v.push_back(30);
	v.push_back(40);
	v.push_back(20);
	v.push_back(50);
	v.push_back(60);
	cout << "替换前" << endl;
	for_each(v.begin(), v.end(), person());
	cout << endl;
	//将大于30的替换成3000
	replace_if(v.begin(), v.end(), myprint(),3000);
	cout << "替换后" << endl;
	for_each(v.begin(), v.end(), person());
	cout << endl;
}
int main()
{
	test01();
	return 0;
}
总结：repalce_if按条件查找，可以利用仿函数灵活帅选满足的条件
```
## 232、swap
- 描述：互换两个容器的元素

函数原型
- swap(container c1,container c2);
- `互换两个容器的元素`
- c1`容器1`
- c2`容器2`
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<algorithm>
void person(int val)
{
	cout << val << " ";
}
void test01()

{
	vector<int>v1;
	vector<int>v2;
	for (int i = 0;i < 10; i++)
	{
		v1.push_back(i);
		v2.push_back(i + 100);
		
	}
	cout << "交换前" << endl;
	for_each(v1.begin(), v1.end(), person);
	cout << endl;
	for_each(v2.begin(), v2.end(), person);
	cout << endl;

	cout << "----------" << endl;
	cout << "交换后" << endl;

	swap(v1, v2);
	for_each(v1.begin(), v1.end(), person);
	cout << endl;
	for_each(v2.begin(), v2.end(), person);
	cout << endl;

}
int main()
{
	test01();
	return 0;
}
```
# 常用算术生成算法
注意；
- 算术生成算法属于小型算法，使用时包含头文件#incude<numeric>

算法简介
- accumulate`计算容器元素总和`
- fill`向容器添加元素`
## 233、accmulate
描述：计算区内 容器累计求和

函数原型
- accumulate(iteerator beg,iterator end,value);
- 计算容器元素总和
- beg`开始迭代器`
- end`结束迭代器`
- valu`起始值`
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<numeric>
void person(int val)
{
	cout << val << " ";
}
void test01()

{
	vector<int>v1;
	for (int i = 0;i <= 100;i++)
	{
		v1.push_back(i);
	}
	//参数3 起始累加值
	int ret=accumulate(v1.begin(), v1.end(),0);
	cout << "ret=" << ret << endl;
}
int main()
{
	test01();
	return 0;
}
总结；accumulate使用时头文件注意是#include<nameric>,这个算法很实用
```
## 234、fill
- 向容器填充指定元素

函数原型
- fill(tierator beg,iterator end,valu)
- 向容器填充元素
- beg`开始迭代器`
- end`结束迭代器`
- value`填充的值`
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<algorithm>
void person(int val)
{
	cout << val << " ";
}
void test01()

{
	vector<int>v;
	v.resize(10);
	//后期重新填充
	fill(v.begin(), v.end(), 20);
	for_each(v.begin(), v.end(), person);
	cout << endl;
}
int main()
{
	test01();
	return 0;
}
利用fill可以将容器区间元素填充为指定的值
```
# 常用集合算法
- 掌握常用的集合算法

算法简介
- set_intersection`求两个容器的交集`
- set_union`求两个容器的并集`
- set_difference`求两个容器的差集`
## 235、set_intersection
描述：求两容器合计

函数原型
- set_intersection(iterator beg1,iterator end1,iterator beg2,iterator end2,iterator dest)
- 注意：两个集合必须是有序序列
- beg1`容器1开始迭代器`
- end1`容器1结束迭代器`
- beg2`容器2开始迭代器`
- end2`容器2结束迭代器`
- dest`目标容器开始迭代器`
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<algorithm>
void person(int val)
{
	cout << val << " ";
}
void test01()
{
	vector<int>v1;
	vector<int>v2;
	for (int i = 0;i < 10;i++)
	{
		v1.push_back(i);//0~9
		v2.push_back(i + 5);//5~14
	}
	vector<int>mubiao;
	//目标容器提前开辟空间
	//最特殊情况 大容器包含小容器  开辟空间 取小容器的size即可
	mubiao.resize(min(v1.size(), v2.size()));
	//获取交集
	vector<int>::iterator itEnd =set_intersection(v1.begin(), v1.end(), v2.begin(), v2.end(), mubiao.begin());
	for_each(mubiao.begin(), itEnd, person);
	cout << endl;
}
int main()
{
	test01();
	return 0;
}
总结
求交集的两个集合必须是有序序列
目标容器开辟空间需要从两个容器中取小值
set_intersection返回值纪实交集中最后一个元素的位置
```
## 236、set_union
描述;求两个集合并集

函数原型
- set_union(iterator beg1 iterator end1,iterator beg2 iterator end2,iterator dest)
- 注意;两个集合容器必须是有序序列
- beg1`容器1开始迭代器`
- end1`容器1结束迭代器`
- beg2`容器2开始迭代器`
- end2`容器2结束迭代器`
- dest`目标容器开始迭代器`
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<algorithm>
void person(int val)
{
	cout << val << " ";
}
void test01()
{
	vector<int>v1;
	vector<int>v2;
	for (int i = 0;i < 10;i++)
	{
		v1.push_back(i);
		v2.push_back(i + 5);
	}
	vector<int>mubiao;
	//提前开辟空间
	//最特殊情况 两个容器没有交集，并集就是两个容器size相加
	mubiao.resize(v1.size()+v2.size());
	vector<int>::iterator itEnd= set_union(v1.begin(), v1.end(), v2.begin(), v2.end(), mubiao.begin());
	for_each(mubiao.begin(),itEnd, person);
	cout << endl;
}
int main()
{
	test01();
	return 0;
}
总结
求并集的两个集合必须有序序列
目标容器开辟空间需要两个容器相加
set_union返回值是并集最后一个元素位置
```
## 237、set_difference
描述：求两个集合差集

函数原型
- set_difference(iterator beg1 iterator end1,iterator beg2 iterator end2,iterator dest)
- 注意：两个集合必须是有序序列
- beg1`容器1开始迭代器`
- end1`容器1结束迭代器`
- beg2`容器2开始迭代器`
- end2`容器2结束迭代器`
- dest`目标容器开始迭代器`
```c++
#include<iostream>
using namespace std;
#include<vector>
#include<algorithm>
void person(int val)
{
	cout << val << " ";
}
void test01()
{
	vector<int>v1;
	vector<int>v2;
	for (int i = 0;i < 10;i++)
	{
		v1.push_back(i);
		v2.push_back(i + 5);
	}
	vector<int>v3;
	//特殊情况 两个容器没有交集 取两个容器中的大size做目标容器开辟空间
	v3.resize(min(v1.size(), v2.size()));
	cout << "v1和v2的差集为；" << endl;
	vector<int>::iterator itEnd=set_difference(v1.begin(), v1.end(), v2.begin(), v2.end(), v3.begin());
	for_each(v3.begin(), itEnd, person);
	cout << endl;

	cout << "v2和v1的差集" << endl;
	itEnd = set_difference(v2.begin(), v2.end(), v1.begin(), v1.end(), v3.begin());
	for_each(v3.begin(), itEnd, person);
	cout << endl;
}
int main()
{
	test01();
	return 0;
}
总结
求差集的两个集合必须是有序序列
目标容器开辟空间需要从两个容器取较大值
set_difference返回值是差集中最后一个元素
```
## 238、演讲比赛流程系统
- 学校举行一场演讲比赛，12人参加。比赛共两轮，第一轮为淘汰赛，第二轮为决赛
- 每名选手都有编号：如1001，1002
- 比赛方式：分组比赛，每组6人
- 第一轮为2个小组，整体按选手编号进行抽签后顺序演讲
- 十个评委分别给每名选手打分，去除最高分去除最低分，求得平均分为本轮选手成绩
- 当小组演讲完后，淘汰组内最后三名，前三名进行下一轮
- 第二轮为决赛，前三名胜出
- 每轮比赛以后需要显示晋级选手信息
## 程序功能
- 开始演讲比赛：完成整届比赛流程。每个比赛阶段需要用户一个提示，用户按任意键继续下一阶段
- 查看往届记录：查看之前比赛前三名结果，每次比赛都会记录到文件中，文件用.csv后缀名
- 清空比赛记录：将文件中数据清空
- 退出比赛程序：可以退出当前程序

## 01、创建管理类
头文件
```c++
#pragma once
#include<iostream>
using namespace std;
//设计管理类
class SpeechManager
{
public:
    //构造函数
    SpeechManager();

    //析构函数
    ~SpeechManager();
};
```
源文件实现
```c++
#include"SpeechManager.h"
//构造函数
SpeechManager::SpeechManager()
{

}

//析构函数
SpeechManager::~SpeechManager()
{

}
```
## 02、菜单功能
- 在管理类SpeechManagere.h中添加成员函数`void show_Menu();`
- 在管理类SeechMManagere.cpp实现`show_menu()`函数
```c++
void show_Menu()
{
	cout << "*******************************" << endl;
	cout << "*******欢迎参加演讲比赛********" << endl;
	cout << "*******1、开始演讲比赛 ********" << endl;
	cout << "*******2、查看往届记录 ********" << endl;
	cout << "*******3、清空比赛记录 ********" << endl;
	cout << "*******0、退出比赛程序 ********" << endl;
	cout << "*******欢迎参加演讲比赛********" << endl;
}
```
- 在演讲比赛管理系统实现函数对象
```c++
#include<iostream>
using namespace std;
#include"speechManagr.h"
int main()
{
	//创建管理类对象
	SpeechManager sm;
	sm.show_Menu();
	return 0;
}
```

## 03、退出功能
- 在speechManager.h中提供系统的成员函数`void exitSystem()`
- 在speechManager.cpp中提供具体功能实现
```c++
void SpeechManager::exitSystem()
{
	cout << "欢迎下次使用" << endl;
	system("paues");
	exit(0);
}
```
## STL演讲比赛流程管理功能分析
- 抽签->开始比赛->显示第一轮比赛结果->
- 抽签->开始比赛->显示前三名结果->保存分数
## 04、创建选手类
- 选手类中的属性包含：选手姓名、分数
- 头文件中创建`speaker.h`文件，并添加代码
```c++
#pragma once
#include<iostream>
using namespace std;
class Sperker
{
public:
	string m_name;//姓名
	double m_Score[2];//分数 最多两轮得分
};
```
## 05、成员属性添加
- 在speechManager.h中添加属性
```c++
//成员属性
//保存第一轮比赛选手编号容器
vector<int>v1;
//第一轮晋级选手编号容器
vector<int>v2;
//胜出前三名选手编号容器
vector<int>vVictory;
//存放编号以及选手的容器
map<int, Sperker>m_Speaker;
//存放比赛轮数
int m_Index;
```
- 在speechManager.h中提供开始比赛的成员函数`void initSpeech`
- 在seechManager.cpp中实现`void initSpeech`
```c++
//初始化容器和属性
void SpeechManager::initSpeech()
{
//容器都制空
	this->v1.clear();
	this->v2.clear();
	this->vVictory.clear();
	this->m_Speaker.clear();

	//初始化比赛轮数
	this->m_Index = 1;
}
```
- speechManager构造函数中调用`void initSpeech();`
```c++
//构造函数
SpeechManager::SpeechManager()
{
	//初始化容器和属性
	this->initSpeech();
}
```
## 06、创建选手
- 在speechManager.h中提供开始比赛的成员函数`void createSpeaker()`
- 在speechManager.cpp中实现`void createSpeaker();`
```c++
void SpeechManager::createSpeaker()
{
	string nameSeed = "ABCDEFGHIJKL";
	for (int i = 0;i < nameSeed.size();i++)
	{
		string name = "选手";
		name += nameSeed[i];
		//创建具体选手
		Sperker sp;
		sp.m_name = name;
		for (int j = 0;j < 2;j++)
		{
			sp.m_Score[j] = 0;
		}
		//12名选手编号
		this->v1.push_back(i + 10001);

		//选手编号以及对应的选手 存放到map容器中
		this->m_Speaker.insert(make_pair(i + 10001, sp));
	}
}
```
- speechManager类中的构造函数调用`void createSpeaker`
```c++
SpeechManager::SpeechManager()
{
	//初始化容器和属性
	this->initSpeech();
	//创建12名选手
	this->createSpeaker();
}
```
## 07、开始比赛成员函数添加
- 在speechManager.h中提供开始比赛的成员函数`void startSpeech()`
```c++
//开始比赛-比赛流程
void startSpeech()
```
- 在speechManager.cpp中将stratSpeech的空实现先写入
- 我们可以将整个比赛流程写到函数中
```c++
void SpeechManager::startSpeech()
{
	//第一轮比赛
	//1、抽签
	this->speechDraw();
	//2、比赛

	//3、显示晋级结果

	//第二轮
	//1、抽签

	//2、比赛

	//3、显示最终结果

	//4、保存分数到文件中
}

}
```
## 08、抽签
- 在speechManager.h中提供抽签的成员函数`void speechDraw`
```c++
//抽签
void speechManager();
```
- 在speechManager.cppp中实现成员函数`void speechDraw()`
```c++
//抽签
void SpeechManager::speechDraw()
{
	cout << "第" << this->m_Index << ">>轮比赛选手正在抽签" << endl;
	cout << "------------------------------------" << endl;
	cout << "抽签后的演讲顺序如下; " << endl;
	if (this->m_Index == 1)
	{
		//第一轮
		random_shuffle(v1.begin(), v1.end());
		for (vector<int>::iterator it = v1.begin();it != v1.end();it++)
		{
			cout << *it << " ";
		}
		cout << endl;
	}
	else
	{
		//第二轮
		random_shuffle(v2.begin(), v2.end());
		for (vector<int>::iterator it = v2.begin();it!=v2.end();it++)
		{
			cout << *it << " ";
		}
		cout << endl;
	}
	cout << "----------------------" << endl;
	system("pause");
	cout << endl;
}
```
## 09、开始比赛
- 在seechManager.h中提供比赛的成员函数`void speechContest();`
- 在speechManager.cpp中实现成员函数`void speechContest();`
```c++
//比赛
void SpeechManager::speechContest()
{
	//准备临时容器 存放小组
	multimap<double, int, greater<double>>gourpScore;
	int num = 0;//统计人员个数6人一组

	cout << "-----------第" << this->m_Index << "轮比赛正式开始------------" << endl;
	vector<int>v_Src;//比赛人员容器
	if (this->m_Index == 1)
	{
		v_Src = v1;
	}
	else
	{
		v_Src = v2;
	}
	//遍历所有选手
	for (vector<int>::iterator it = v_Src.begin();it != v_Src.end();it++)
	{
		num++;
		//评委打分
		deque<double>d;
		for (int i = 0;i < 10;i++)
		{
			double score = (rand() % 401 + 600) / 10.f;
			//cout << score << " ";
			d.push_back(score);
		}
		//cout << endl;
		sort(d.begin(), d.end(), greater<double>());//排序
		d.pop_front();//去除最高分
		d.pop_back();//去除最低分
		double sum = accumulate(d.begin(), d.end(), 0.0f);//总分
		double avg = sum / (double)d.size();//平均分
		//打印平均分
		//cout << "编号；" << *it << "选手姓名； " << this->m_Speaker[*it].m_name << "平均分； " << avg << endl;
		//将平均分放到map容器中
		this->m_Speaker[*it].m_Score[this->m_Index - 1] = avg;
		//将数据放入临时容器中
		gourpScore.insert(make_pair(avg, *it));//key是得分 value是具体选手编号
		//每六人取出前三
		if (num % 6 == 0)
		{
			cout << "第" << num / 6 << "小组比赛名次； " << endl;
			for (multimap<double, int, greater<double>>::iterator it = gourpScore.begin();it != gourpScore.end();it++)
			{
				cout << "编号； " << it->second << "姓名； " << this->m_Speaker[it->second].m_name
					<< "成绩； "<< this->m_Speaker[it->second].m_Score[this->m_Index - 1]<<endl;
			}
			//取走前三名
			int count = 0;
			for (multimap<double, int, greater<double>>::iterator it = gourpScore.begin();it != gourpScore.end()&&count<3;it++,count++)
			{
				if (this->m_Index == 1)
				{
					v2.push_back((*it).second);
				}
				else
				{
					vVictory.push_back((*it).second);
				}
			}
			gourpScore.clear();//小组容器清空
			cout << endl;
		}
	}
	cout << "--------------第" << this->m_Index << "轮的比赛完毕------------" << endl;
	system("pause");
}
```
## 10、显示比赛分数
- 在speechManager.h中提供显示的成员函数`void showScore()`
- 在speechManager.cpp中实现成员函数`void showScore()`
```c++
//显示比赛结果
void SpeechManager::showScore()
{
	cout << "-----------第" << this->m_Index << "轮晋级选手信息如下---------" << endl;
	vector<int>v;
	if (this->m_Index == 1)
	{
		v = v2;
	}
	else
	{
		v = vVictory;
	}
	for (vector<int>::iterator it = v.begin();it != v.end();it++)
	{
		cout << "选手编号； " << *it << "姓名; " << m_Speaker[*it].m_name << "得分； " << m_Speaker[*it].m_Score[this->m_Index - 1] << endl;
	}
	cout << endl;
	system("pause");
	system("cls");
	this->show_Menu();
}
```
## 11、第二轮比赛
```c++
//开始比赛-比赛流程
void SpeechManager::startSpeech()
{
	//第一轮比赛
	//1、抽签
	this->speechDraw();
	//2、比赛
	this->speechContest();
	//3、显示晋级结果
	this->show_Menu();

	//第二轮
	this->m_Index++;
	//1、抽签
	this->speechDraw();
	//2、比赛
	speechContest();
	//3、显示最终结果
	this->show_Menu();
}
```
## 12、保存分数
- 在speechManager.h中添加保存记录的成员函数`void saveRecord();`
- 在speechManager.cpp中实现成员函数`void saveRecord();`
```c++
void SpeechManager::saveRecord()
{
	ofstream ofs;
	ofs.open("speech.csv", ios::out | ios::app);//用输出的方式打开文件
		//将每个人数据写到文件中
	for (vector<int>::iterator it = vVictory.begin();it != vVictory.end();it++)
	{
		ofs << *it << "," << this->m_Speaker[*it].m_Score[1] << ",";
		}
	ofs << endl;
	//关闭文件
	ofs.close();
	cout << "记录已保存" << endl;
}
//4、保存分数到文件中
this->saveRecord();
cout << "本届比赛完结" << endl;
system("pause");
```
## 12、查看记录
- 在speechManager.h中添加保存记录的成员函数`void loadRecord();`
- 添加判断文件是否为空的标志`bool fileIsEmpty;`
- 添加往届记录的容器`map<int,vector<string>>m_Record`
- 其中m_Record中的key代表第几届，value记录具体信息
```c++
//读取信息
void loadRecord();
//文件为空的标志
bool fileIsEmpty;
//往届记录
map<int,vector<string>>m_Record
```
- 在speechManager.cpp中实现成员函数`void loadRecord();`
```c++
void SpeechManager::loadRecord()
{
	ifstream ifs("speech.csv",ios::in);//输入对象流 读取文件

	if(!ifs.is_open())
	{
     this->fileIsEmpty=true;
     cout <<"文件不存在"<<endl;
     ifs.close();
	 return ;
	}
	char ch;
	ifs>>ch;
	if(ifs.eof())
	{
		cout <<"文件为空"<<endl;
		this->fileIsEmpty=true;
		ifs.close();
		return ;
	}
	//文件不为空
	this->fileIsEmpty=false;
	ifs.putback(ch);//读取的单个字符放回去
	string data;
	int index=0;
	while(ifs>>data)
	{
		//cout<<data<<endl;
		vector<string>v;
		int pos=-1;
		int start=0;
		while(true)
		{
			pos=data.find(",",start);//从0开始查找
			if(pos==-1)
			{
				break;//找不到break返回
			}
			string tmp=data.substr(start,pos-start);//找到了进行分割 参数1 起始位置 参数2 截取长度
			v.push_back(tmp);
			start=pos+1;
		}
		this->m_Record.insert(make_pair(index,v));
		index++;
	}
	ifs.close();
	
}
```

- 在speechManager.h添加保存记录的成员函数`void showRecord()`
```c++
//显示往届得分
void showRecord()
```
- 在speechManager.cpp中实现成员函数`void showRecord()`
```c++
void SpeechManager::showRecord()
{
	for(int i=0;i<this->m_Record.size();i++)
	{
		cout <<"第"<<i+1<<"届"
		<<"冠军编号"<<this->m_Record[i][0]<<"得分； "<<this->m_Record[i][1]<<" "
		"亚军编号"<<this->m_Record[i][2]<<"得分； "<<this->m_Record[i][3]<<" "
		"季军编号"<<this->m_Record[i][4]<<"得分："<<this->m_Record[i][5]<<endl;
	}
	system("pause");
	system("cls");
}
```
## 13、bug解决
- 查看往届记录，若文件为空，并不提示
- 解决方法；在showRecord函数中，开始判断文件状态并加以判断
```c++
if(this->fileIsEmpty)
{
	cout <<"文件不存在或者为空"<<endl;
}
```
- 若记录为空或者不存在，比赛后依然提示为空
- 解决方法；saveRecord中更新文件为空的标志
```c++
//有记录了，文件不为空
this->fileIsEmpty = false;
```
- 比完赛后查不到本届记录，没有实时更新
- 解决方法；比赛完毕后，所有数据重置
```c++
//重置比赛
//初始化属性
this->initSpeech();
//创建选手
this->createSpeaker();
//获取往届记录
this->loadRecord();

```
- 在初始化时，没有初始化容器
- 解决方法；initSpeech中添加初始化容器
```c++
//将记录容器清空
this->m_Record.clear();
```
- 每次记录都一样
- 解决方法； 在main函数一开始添加随机种子
```c++
srand((unsiged int)time(NULL));
```
## 14、清空记录
- 在speechManager.h中添加清空记录的成员函数`void clearRecord();`
- 在speechManager.cpp中实现成员函数
```c++
void SpeechManager::clearRecord()
{
	cout <<"确认清空"<<endl;
	cout <<"1、确认"<<endl;
	cout <<"2、返回"<<endl;

	int select=0;
	cin>>select;

	if(select==1)
	{
		//打开模式 ios::trunc 如果存在删除文件并重新创建
		ofstream ofs("speech.csv"),ios::trunc);
		ofs.close();
		//初始化属性
		this->initSpeech();
		//创建选手
		this->createSpeaker();
		//获取往届记录
		this->loadRecord();
		cout <<"清空成功"<<endl;
	}
	system("pause");
	system("cls");
}
```
## 机房预约系统
## 身份简介
- 分别有三种身份使用该程序
- 学生代表；申请使用机房
- 教师；审核学生的预约请求
- 管理员；给学生，教师创建账号
## 机房简介
- 1号机房----最大容量20人
- 2号机房---最多容量50人
- 3号机房---最多容量100人
## 申请简介 
- 申请的订单每周又管理员清空
- 学生可以预约未来一周的机房使用。预约的日期周一和周五，预约时需要选择预约时间段（上午或者下午）
- 教师来审核预约，依据实际情况审核预约通过或者不通过
## 系统具体要求
- 首先进入登陆界面，可选登陆身份有
- 学生代表 
- 教师
- 管理员
- 退出

每个身份都需要进行验证后，进入子菜单
- 学生输入；学号、姓名。登陆密码
- 教师需要输入；职工号、姓名。登陆密码
- 管理员需要输入；管理员姓名、登陆密码

学生具体功能实现
- 申请预约--预约机房
- 查看自身的预约--查看自己的预约状态
- 查看所有预约--查看所有预约信息和预约状态
- 取消预约--取消自身的预约，预约成功或者审核中的预约均可取消
- 注销登陆--退出登陆

教师具体功能实现
- 查看所有预约--查看全部预约信息和状态
- 审核预约--对学生的预约进行审核
- 注销登陆--退出登陆

管理员具体功能
- 添加账号--添加学生或者教师的账号，需要检测学生编号或者教师职工号是否重复
- 查看账号--可以选择查看学生或者教师的全部信息
- 查看机房--查看所有机房的信息
#### 创建主菜单
菜单实现
- 在主函数中添加代码
```c++
int main()
{
	int select = 0;//用于接受用户的选择
	while (true)
	{
			
	
	cout << "------------------" << endl;
	cout << endl << "请输入你的身份" << endl;
	cout << "\t\t|---------------------------|\n";
	cout << "\t\t|    1、学生代表            |\n";
	cout << "\t\t|    2、老师                |\n";
	cout << "\t\t|    3、管理员              |\n";
	cout << "\t\t|    0、退出                |\n";
	cout << "\t\t|---------------------------|\n";
	cout << "请输入你的选择" << endl;
	cin >> select;//接受用户选择
	switch (select)//根据用户选择来实现不同接口
	{
	case 1://学生代表
		break;
	case 2://老师
		break;
	case 3://管理员
		break;
	case 0://退出
		break;

	default:
		cout << "输入有误，请重新选择" << endl;
		system("pause");
		system("cls");
		break;
	}
	}

	system("pause");
	return 0;

}
```
## 退出功能
- 在main函数分支0中添加退出代码；
```c++
case 0://退出
	cout << "欢迎下次使用" << endl;
	system("pause");
	return 0;
```
## 创建身份类
- 在整个系统中，有三种身份，分别为：学生代表，教师以及管理员
- 三种身份有其共性也有特性，因此我们可以将三种身份抽性出一个身份基类`identity`
- 在头文件下创建`ldentity.h`文件
ldentity.h中添加代码
```c++
#pragma once
#include<iostream>
using namespace std;
//身份抽象类
class Identity
{
public:
	//操作菜单 纯虚函数
	virtual void operMan() = 0;

	string m_Name;//姓名
	string m_pwd;//密码

};
```
## 学生类
- 学生类的主要功能
- 显示学生操作的菜单页面
- 申请预约
- 查看自身预约
- 查看所有预约
- 取消预约
#### 类得创建
- 在头文件以及源文件下创建student.h和student.cpp文件
- student.h中添加如下代码
```c++
#pragma once
#include<iostream>
using namespace std;
#include"ldentity.h"
//学生类
class Studen: public Identity
{
public:
	//默认构造
	Studen();
	//有参构造
	Studen(int id, string name, string pwd);
	//菜单界面
	 void operMenu();
	//申请预约
	void applyOrder();
	//查看我的预约
	void showMyOrder();
	//查看所有预约
	void showAllOrder();
	//取消预约
	void cancelOrder();
	//学生学号
	int m_Id;
};
```
- 在studen.cpp中添加代码 做空实现
```c++
#include"student.h"
//默认构造函数
Student::Student()
{

}
//有参构造
Student::Student(int id,string name,string pwd)
{

}
//菜单界面
void Student::operMenu()
{

 }
//申请预约
void Student::applyOrder()
{

}
//查看我的预约
void Student::showMyOrder()
{

}
//查看所有预约
void Student::showAllOrder()
{

}
//取消预约
void Student::cancelOrder()
{

}

```
## 老师类
- 老师功能
- 显示教师操作的菜单页面
- 查看所有预约
- 审核预约
#### 类的创建
- 在头文件以及源文件下创建teacher.h和teacher.cpp文件
- teacher.h添加代码
```c++
#pragma once
#include<iostream>
using namespacce std;
#include"ldentity.h"


//教师类
class Teacher:public Identity 
{
	public:
		//默认构造
		Teacher();
		//有参构造
		Teacher(int id, string name, string pwd);
		//菜单界面
		 void operManu();
		//查看所有预约
		void showAllOrder();
		//审核预约
		void validOrder();
		//教师编号
		int m_EmpId;

};
```
- 在teacher.cpp中添加代码 做空实现
```c++
#include"teacher.h"
//默认构造
Teacher::Teacher()
{

}
//有参构造
Teacher::Teacher(int id, string name, string pwd)
{

}
//菜单界面
void Teacher::operManu()
{

 }
//查看所有预约
void Teacher::showAllOrder()
{

}
//审核预约
void Teacher::validOrder()
{

}
```
## 管理员类
管理员类主要时对学生老师账户进行管理，查看机房信息以及情况预约记录

管理员功能主要作用
- 显示管理员操作的菜单界面
- 添加账户
- 查看机房信息
- 情况预约记录
#### 类的创建
- 在头文件以及源文件下创建manager.h和manager.cpp文件
- 在manager.h中添加代码 做空实现
```c++
#pragma once
#include<iostream>
using namespace std;
#include"ldentity.h"
//管理员类
class Manager :public Identity
{
	//构造函数
	Manager();
	//有参构造
	Manager(string name, string pwd);
	//选择菜单
	 void operManu();
	 //添加账户
	 void addPerson();
	 //查看机房信息
	 void showComputer();
	 //清空预约记录
	 void cleanFile();
};
```
- 在manager.cpp中添加代码先做空实现
```c++
#include"manager.h"
//构造函数
Manager::Manager()
{

}
//有参构造
Manager::Manager(string name, string pwd)
{

}
//选择菜单
void Manager::operManu()
{

 }
//添加账户
void Manager::addPerson()
{

}
//查看机房信息
void Manager::showComputer()
{

}
//清空预约记录
void Manager::cleanFile()
{

}
```
## 登陆模块
#### 全局文件添加
- 不同的身份可能遇到不同的文件操作，我们可以将所有文件的文件名定义到一个全局文件中
- 在头文件添加 glbalFile.h文件
- 并添加代码
```c++
#pragma once

//管理员文件
#define ADMIN_FILE "admin.txt"
//学生文件
#define STUDENT_FILE "studet.txt"
//老师文件
#define TEACHER_FILE "tescher.txt"
//机房信息文件
#define COMPUTER_FILE "computerRoom.txt"
//订单文件
#define ORDER_FILE "order.txt"

```
## 登陆函数封装
- 根据用户的选择，进入不同的身份登陆
- 在预约系统的.cpp文件中添加全局函数`void LoginIn(string fileName,int type)`
- 参数
- fileName---操作的文件名
- type---登陆身份（1代表学生，2代表老师，3代表管理员）

Loginln中添加如下代码
```c++
#include"ldentity.h"
#include"fstream"
#include"globalFile.h"

//登陆功能 参数1 操作文件名 参数2  操作身份类型
void LoginIn(string fileName, int type)
{
	//父类指针，用于指向子类对象
	Identity* person = NULL;

	//读文件
	ifstream ifs;
	ifs.open(fileName, ios::in);
	//判断文件是否存在
	if (!ifs.is_open())
	{
		cout << "文件不存在" << endl;
		ifs.close();
		return;
	}
	//准备接收用户信息
	int id = 0;
	string name;
	string pwd;
	//判断身份
	if (type == 1)//学生身份
	{
		cout << "请输入你的学号" << endl;
		cin >> id;
	}
	else if(type==2)
	{
		cout << "请输入你的职工号" << endl;
		cin >> id;
	}
	cout << "请输入用户名字" << endl;
	cin >> name;
	cout << "请输入密码" << endl;
	cin >> pwd;
	if (type == 1)
	{
		//学生身份验证

	}
	else if (type == 2)
	{
		//教师身份验证

	}
	else if (type == 3)
	{
		//管理员身份验证
	}
	cout << "验证登陆失败" << endl;
	system("pause");
	system("cls");
	return;
}
```
## 学生登陆实现
- 在student.txt中添加两条学生信息，用于测试
- 添加信息
- 张三 123 李四 123456

- 其中
- 第一列 代表学号
- 第二列代表学生姓名
- 第三列 代表密码
- 在Login函数的学生分支中加入一下代码
```c++
//学生身份验证
int fId;//从文件中读取的id号
string fName;//从文件中读的姓名
string fPwd;//从文件获取的密码
while (ifs>>fId&&ifs>>fName &&ifs>>fPwd )
{
	//与用户输入的信息做对比
	if (fId == id && fName == name && fPwd == pwd)
	{
		cout << "学生的验证成功" << endl;
		system("pause");
		system("cls");
		person = new Student(id, name, pwd);
		//进入学生身份的子菜单

		return;
	}
}
```
## 教师登陆实现
- 在teacher.txt中添加老师信息
- 添加信息
- 1 老王  123

其中
- 第一列 代表 教师职工号
- 第二列 代表老师姓名
- 第三列 代表老师密码
```c++
//教师身份验证
int fId;
string fName;
string fPwd;
while (ifs >> fId && ifs >> fName && ifs >> fPwd)
{
	if ( fId ==id && fName == name && fPwd == pwd)
	{
		cout << "教师验证成功" << endl;
		system("pause");
		system("cls");
		person = new Teacher(id, name, pwd);
		return;
	}
}
```
## 管理员登陆实现
- 在admin.txt文件中添加一条管理信息，由于我们只有一个管理员，因此本案例中没有添加管理员功能
- 添加；admin 123

其中；admmin代表管理员用户名 123代表密码
```c++
//管理员身份验证
string fName; // 从文件中读的姓名
	
string fPwd;//从文件获取的密码
while (ifs >> fName && ifs >> fPwd)
{
	if (fName == name && fPwd == pwd)
	{
		cout << "管理员登陆成功" << endl;
		system("pause");
		system("cls");
		person = new Manager(name, pwd);
		//进入管理员子菜单

		return;
	}
}
```
## 管理员登陆和注销
- 在Manager类的构造函数中，初始化管理员信息，
```c++
//有参构造
Manager::Manager(string name,string pwd)
{
	this->m_Name=name;
	this->_Pwd=pwd;
}
```
## 管理员子菜单
- 在机房预约系统.cpp中，当用户登陆的是管理员，统计管理员菜单接口

将不同的分支提供出来
- 添加账户
- 查看账号
- 查看机房
- 清空预约
- 注销登陆
- 实现注销功能

添加全局函数`void managerMenu(Identity*&manager)`,代码如下
```c++
void managerMenu(Identity*&manager)
{
	while(true)
	{
		//管理员菜单
		manager->operMenu();

		Manager*man=(Manager*)manager;
		int select=0;
		cin>>select;
		if(select==1)//添加账号
		{
          cout <<"添加账号"<<endl;
		  man->addPerson();
		}
		else if(select==2)
		{
			cout <<"查看账户"<<endl;
			man->showPerson();
		}
		else if(select==3)
		{
			cout <<"查看机房"<<endl;
			man->showComputer();
		}
		else if(select==4)
		{
			cout <<"清空预约"<<endl;
			man->cleanFile();
		}
		else
		{
			delete manager;
			cout <<"注销成功"<<endl;
			system("pause");
			system("cls");
			return ;
		}
	}
}
```
#### 接口对接
- 管理员成功登陆后，调用管理员子菜单页面
- 在管理员登陆验证分支中，添加代码
```c++
//进入管理员子菜单
managerMenu(person);
```
#### 添加账号
描述；
- 给学生或者老师添加新账号
要求
- 添加学生学号不能重复，老师职工号不能重复
#### 添加功能实现
- 在Manager中的addPerson成员函数中，实现添加新账号功能，代码如下
```c++
//添加账号
void Manager::addPerson()
{
	cout<<"请输入账号类型"<<endl;
	cout<<"1、添加学生"<<endl;
	cout<<"2、添加老师"<<endl;

	string fileName;
	string tip;
	ofstream ofs;

	int select=0;
	cin>>select;
	if(select==1)
	{
		fileName=STUDENT_FILE;
		tip="请输入学号; ";
	}
	else
	{
		fileName=TEACHER_FILE;
		tip="请输入职工号; ";
	}
	ofs.open(fileName,ios::out|ios::app);
	int id;
	string name;
	string pwd;
	cout <<"请输入姓名"<<endl;
	cin>>name;
	cout <<"请输入密码"<<endl;
	cin>>pwd;
	ofs<<id<<" "<<name<<" "<<pwd<<" "<<endl;
	cout <<"添加成功"<<endl;
	system("pause");
	system("cls");
	ofs.close();
}
```
## 去重操作
描述；添加新账户时，如果重复的学生编号，或是重复的教师职工编号，提示有误

读取信息
- 要去除重复的账号，首先要先将学生和老师1的账号信息获取到程序中，方可检测
- 在manager.h中，添加两个容器，由于存放学生和老师信息
 - 添加一个新的成员函数`void initVector()`初始化容器
 ```c++
 //初始化容器
 void initVector();
 //学生容器
vector<Student>vStu;
 //老师容器
 vector<Teacher>Tea;
 ```
 - 在Manager的有参构造中，获取目前的学生和老师信息
 - 代码如下
 ```c++
//初始化容器
void Manager::initVector()
{
	//确保容器清空
	vStu.clear();
	vTea.clear();
	//读取信息  学生
	ifstream ifs;
	ifs.open(STUDENT_FILE, ios::in);
	if (ifs.is_open())
	{
		cout << "文件读取失败" << endl;
		return;
	}
	Student s;
	while (ifs >> s.m_Id && ifs >> s.m_Name && ifs >> s.m_Pwd)
	{
		vStu.push_back(s);
	}
	cout << "当前学生数量为多少"<<vStu.size() << endl;
	ifs.close();
	//读取信息  老师
	ifs.open(TEACHER_FILE, ios::in);
	Teacher t;
	while (ifs >> t.m_EmpId && ifs >> t.m_Name && ifs >> t.m_Pwd)
	{
		vTea.push_back(t);
	}
	cout << "当前老师数量为多少" << vTea.size() << endl;
	ifs.close();
}
 ```
 ## 去重函数封装
 - 在mamager.h文件中添加成员函数`bool checkReeat(int id,int type)`
 ```c++
 //检测重复 参数（传入id,传入类型）返回值；（true代表有重复性，false代表没有重复）
 bool checkRepeat(int id,int type)
 ```
 - 在manager.cpp中实现成员函数`bool checkReeat(int id,int type)`
 ```c++
//检测重复
bool  Manager::checkReeat(int id, int type)
{
	if (type == 1)
	{
		for (vector<Student>::iterator it = vStu.begin();it != vStu.end();it++)
		{
			if (id == it->m_Id)
			{
				return true;
			}
		}
	}
	else
	{
		for (vector<Teacher>::iterator it = vTea.begin();it != vTea.end();it++)
		{
			if (id == it->m_EmpId)
			{
				return true;
			}
		}
	}
	return false;

}
 ```
 ## bug解决
 bug描述； 
 虽然可以检测重复的账号，但是刚添加的账号由于没有更新到容器中，因此不会做检测
 - 导致刚加入的学生号或职工号，再次添加依然可以重复

 解决方案
 - 在每次添加新账号时初始化容器
 ```c++
 //调用初始化容器接口，从新获取文件中的数据
this->initVector();
```
## 显示账号
- 在Manager的showPerson成员函数中，实现显示账号功能
```c++
//查看账号
void Manager::showPerson()
{
	cout << "请选择查看的内容" << endl;
	cout << "1、查看所有的学生" << endl;
	cout << "2、查看所有的老师" << endl;

	int select = 0;//接受用户选择
	cin >> select;
	if (select == 1)
	{
		//查看学生
		cout << "所有学生信息如下" << endl;
		for_each(vStu.begin(), vStu.end(), preintStudent);
	}
	else
	{
		//查看老师
		cout << "所有老师信息如下" << endl;
		for_each(vTea.begin(), vTea.end(),preintTeacher );
	}
	system("pause");
	system("cls");
}

```
## 查看机房
- 案例要求中，机房一个有三个，其中1号机房容量20台，2号50台，3号100台
- 我们可以将信息录入到computerRoom.txt中
- 在头文件下创建新的文件夹`computerRoom.h`
```c++
#pragma once
#include<iostream>
using namespace std;
//机房类
class ComputerRoom
{
public:
	int m_Comid;//机房号
	int m_MaxNum;//机房最大容量
};
```
#### 初始化机房信息
- 在Manager管理员下，添加机房的容器，用于保存机房信息
```c++
//机房容器
vector<ComputerRoom>vCom;
```
在Manager因此构造函数中，追加如下代码，初始化机房信息
```c++
ifstream ifs;
ifs.open(COMPUTER_FILE,ios::in);

ComputerRoom c;
while(ifs>>c.m_ComId&&ifs.m_MaxNum)
{
	vCom.push_back(c);
}
cout <<"当前机房数量为"<<vCom.size()<<endl;
ifs.close();
```
#### 显示机房信息
- 在Manager类中的showComputer成员函数中添加如下代码
```c++
//查看机房信息
void Manager::showComputer()
{
	cout << "机房的信息如下" << endl;
	for (vector<ComputerRoom>::iterator it = vCom.begin();it != vCom.end();it++)
	{
		cout << "机房编号" << it->m_Comid << "机房最大容量" << it->m_MaxNum << endl;
	}
	system("pause");
	system("cls");
}
```
#### 清空预约
描述；清空生成的order.txt
- 在Manager的cleanFile成员函数中添加如下代码
```c++
//清空预约记录
void Manager::cleanFile()
{
	ofstream ofs(ORDER_FILE, ios::trunc);
	ofs.close();
	cout << "清空成功" << endl;
	system("pause");
	system("cls");
}
```
#### 学生登陆和注销
- 在Student类的构造函数中，初始化学生信息代码如下
```c++
//有参构造
Student::Student(int id, string name, string pwd)
{
	//初始化属性
	this->m_Id = id;
	this->m_Name = name;
	this->m_Pwd = pwd;
}
```

#### 管理员子菜单
- 在机房预约系统.cpp中，当用户登陆的是学生，添加学生菜单接口
- 将不同得分支提供出来
- 申请预约
- 查看我的预约
- 取消预约
- 注销登陆
- 添加全局函数`void studentMenu(Identity*&manager)`代码如下
```c++
//学生菜单
void studentMenu(Identity*&student)
{
	while(true)
	{
		//学生菜单
		student->operMenu();
		Student*stu=(Student*)student;
		int select=0;

		cin>>select;

		if(select==1)//审核预约
		{
			stu->applyOrder();
		}
		else if(select==2)//查看自身预约
		{
			stu->showMyOrder();
		}
		else if(select==3)//查看所有预约
		{
			stu->showAllOrder();
		}
		else if(select==4)
		{
			stu->cancelOrder();
		}
		else
		{
			delete student;
			cout <<"注销成功"<<endl;
			system("pause");
			system("cls");
			return ;
		}
		
	}
}
```
## 申请预约
- 在申请预约时，学生可以看到机房信息，因此我们需要让学生获取到机房得信息
- 在student.h中添加新得成员函数如下；
```c++
//机房容器
vector<ComputerRoom>vCom;
```
- 在学生得有参构造函数追加如下代码
```c++
//获取机房信息
ifstream ifs;
ifs.open(COMPUTER_FILE,ios::in)

ComputerRoom c;
while(ifs>>c.m_Comid&&ifs>>c.m_MaxNum)
{
	vCom.push_back(c);
}
ifs.close();
```
- 预约功能实现
- 在student.cpp中实现`void Student::applyOrder()`
```c++
//申请预约
void Student::applyOrder()
{
	cout << "机房开放时间为周一到周五" << endl;
	cout << "请输入申请预约得时间" << endl;
	cout << "1、周一" << endl;
	cout << "2、周二" << endl;
	cout << "3、周三" << endl;
	cout << "4、周四" << endl;
	cout << "5、周五" << endl;
	int date = 0;//日期
	int interval = 0;//时间
	int room = 0;//机房编号
	while (true)
	{
		cin >> date;
		if (date >= 1 && date <= 5)
		{
			break;
		}
		cout << "输入有误，请重新输入" << endl;
	}
	cout << "请输入申请预约时间段" << endl;
	cout << "1、上午" << endl;
	cout << "2、下午" << endl;
	while (true)
	{
		cin >> interval;
		if (interval >= 1 && interval <= 2)
		{
			break;
		}
		cout << "输入有误，请重新输入" << endl;
	}
	cout << "请选择机房" << endl;
	cout << vCom[0].m_Comid << "号机房容量为； " << vCom[0].m_MaxNum << endl;
	while (true)
	{
		cin >> room;
		if (room >= 1 && room <= 3)
		{
			break;
		}
		cout << "输入有误" << endl;
	}
	cout << "预约成功，审核中" << endl;
	ofstream ofs;
	ofs.open(ORDER_FILE, ios::app);

	ofs << "date; " << date << " ";
	ofs << "interval" << interval << " ";
	ofs << "stuid; " << this->m_Id << " ";
	ofs << "stuName;" << this->m_Name << " ";
	ofs << "stuPwd;" << this->m_Pwd << " ";
	ofs << "room; " << room << " ";
	ofs << "status; " << 1 << endl;
	ofs.close();

	system("pause");
	system("cls");

}
```
## 显示预约
#### 创建预约类
- 在头文件以及源文件下分别创建`orderFile.h`和`orderFile.cpp`文件
- orderFile.h代码如下
```c++
#pragma once
#include<iostream>
using namespace std;
#include<map>
#include"globalFile.h"

class OrderFile
{
	public:
		//构造函数
		OrderFile();
		//更新预约记录
		void updatOrder();
		//记录得容器 key---记录得条数 value--具体记录得建值对信息
		map<int, map<string, string>>m_orderDete;
		//预约记录条款
		int m_Size;
};
```
- 更新预约记录得成员函数`updateOrder`代码如下
```c++
void OrderFile::updateOrder()
{
	if(this->m_Size==0)
	{
		return ;
	}
	ofstream ofs(ORDER_FILE,ios::out|ios::trunc);
	for(int i=0；i<m_Size;i++)
	{
		ofs<<"dete; "<<this->m_orderDete[i]["date"]<<" ";
		ofs<<"intervall; "<<this->m_orderDete[i]["intervall"]<<" ";
		ofs<<"stuId; "<<this->m_orderDete[i]["stuId"]<<" ";
		ofs<<"stuName; "<<this->m_orderDete[i]["stuName"]<<" ";
		ofs<<"roomId; "<<this->m_orderDete[i]["roomId"]<<" ";
		ofs<<"status; "<<this->m_orderDete[i]["status"]<<endl;
	}
	ofs.close();
	system("pause");
system("cls");
}
```
## 显示自身预约
- 首先我们添加几条预约记录，可以用程序添加或者直接修改order.txt文件
- order.txt文件内容如下：比如我们有三个同学产生了三条预约记录
- 在student类的`void Student::showMyOrder()`成员函数中，添加如下代码
```c++
void Student::showMyOrder()
{
	OrderFile of;
	if (of.m_Size == 0)
	{
		cout << "无预约记录" << endl;
		system("pause");
		system("cls");
		return;
	}
	for (int i = 0;i < of.m_Size;i++)
	{
		if (atoi(of.m_orderDete[i]["stuId"].c_str()) == this->m_Id)
		{
			cout << "预约日期； 周" << of.m_orderDete[i]["date"];
			cout << "时段； " << (of.m_orderDete[i]["interval"] == "1" ? "上午" : "下午");
			cout << "机房；" << of.m_orderDete[i]["rooId"];
			string status = "状态; ";
			if (of.m_orderDete[i]["stetus"] == "1")
			{
				status += "审核中";
			}
			else if (of.m_orderDete[i]["stetus"] == "2")
			{
				status += "预约成功";
			}
			else if (of.m_orderDete[i]["stetus"] == "-1")
			{
				status += "审核未通过,预约失败";
			}
			else
			{
				status += "预约已取消";
			}
			cout << status << endl;
		}
	}
	system("pause");
	system("cls");
}
```
## 取消预约
- 在student类的`void Student::cancelOrder`成员函数中，添加以下代码；
```c++
//取消预约
void Student::cancelOrder()
{
	OrderFile of;
	if (of.m_Size = 0)
	{
		cout << "无预约" << endl;
		system("pause");
		system("cls");
		return;
	}
	cout << "审核中或预约成功的纪录可以取消，请输入取消的记录" << endl;
	vector<int>v;//存放最大容器的下标编号
	int index = 1;
	for (int i = 0;i < of.m_Size;i++)
	{
		//先判断自身的学号
		if (this->m_Id == atoi(of.m_orderDete[i]["stuId"].c_str()))
		{
			//在筛选状态  审核中或预约成功的
			if (of.m_orderDete[i]["status"] == "1" && of.m_orderDete[i]["status"] == "2")
			{
				v.push_back(i);
				cout << index++ <<"、";
				cout << "预约日期； " << of.m_orderDete[i]["date"];
				cout << "预约时间段； " << (of.m_orderDete[i]["interval"] == "1" ? "上午" : "下午");
				cout << "机房编号； " << of.m_orderDete[i]["roomId"];
				string status = "状态； ";
				if (of.m_orderDete[i]["status"] == "1")
				{
					status += "审核中";
				}
				else if (of.m_orderDete[i]["status"] == "2")
				{
					status += "预约成功";
				}
				cout << status << endl;
			}
		}
	}
	cout << "请输入取消的记录，0代表返回" << endl;
	int select = 0;
	while (true)
	{
		cin >> select;
		if (select >= 0 && select <= v.size())
		{
			if (select == 0)
			{
				break;
			}
			else
			{
				of.m_orderDete[v[select - 1]]["status"] = "0";
				of.updatOrder();

				cout << "已经取消预约" << endl;
				break;
			}
		}
		cout << "输入有误，请重新输入" << endl;

	}
	system("pause");
	system("cls");
}

```
## 教师的登陆和注销
- 在构造函数Teacher类中，初始化教师信息，代码如下；
```c++
//有参构造函数（职工编号，姓名，密码）
Teacher::Teacher(int empId,string name,string pwd)
{
	//初始化属性
	this->m_EmpId=empId;
	this->M_Name=name;
	this->m_Pwd=pwd;
}
```
## 教师子菜单
- 在机房预约系统.cpp中，当用户登陆的是教师，添加教师登陆接口
- 将不同得分支提供出 
- 查看所有预约
- 审核预约
- 注销登陆
- 实现注销功能
- 添加全局函数`void TeacherMenu(person*&teacher)`代码如下：
```c++
//进入教师得子菜单界面
void teacherMenu(Identity*&teacher)
{
	while (true)
	{
		//调用子菜单界面
		teacher->operMenu();
		Teacher* tea = (Teacher*)teacher;

		int select = 0;//接受用户得选择
		cin >> select;
		if (select == 1)//查看所有得预约
		{
			tea->showAllOrder();

		}
		else if (select == 2)///审核预约
		{
			tea->validOrder();
		}
		else
		{
			delete teacher;
			cout << "注销成功" << endl;
			system("pause");
			system("cls");
			return;
		}
	}
}
```
## 接口对接
- 登陆成功后，调用教师得子菜单界面
- 在教师登陆分支中，添加代码
```c++
//进入教师子菜单
TeacherMenu(person);
```
#### 教师类查看所有预约
- 在Teacher.cpp中实现成员函数`void Teacher::showAllOrder`
```c++
//查看所有预约
void Teacher::showAllOrder()
{
	OrderFile of;
	if (of.m_Size == 0)
	{
		cout << "无预约记录" << endl;
		system("pause");
		system("cls");
		return;
	}
	for (int i = 0;i < of.m_Size;i++)
	{
		cout << i + 1 << "、 ";
		cout << "预约日期；  周" << of.m_orderDete[i]["dete"];
		cout << "时间段； " << (of.m_orderDete[i]["interval"]=="1"?"上午":"下午");
		cout << "学号； " << of.m_orderDete[i]["stuId"];
		cout << "姓名； " << of.m_orderDete[i]["stuName"];
		cout << "机房编号； " << of.m_orderDete[i]["roomId"];
		string status = "状态";
		//1 审核中  2 已预约 -1预约失败  0 取消预约
		if (of.m_orderDete[i]["status"] == "1")
		{
			status += "审核中";
		}
		else if (of.m_orderDete[i]["status"] == "2")
		{
			status += "预约成功";
		}
		else if (of.m_orderDete[i]["status"] == "3")
		{
			status += "预约失败";
		}
		else
		{
			status += "预约取消";
		}
		cout << status << endl;
	}
	system("pause");
	system( "cls" );
}
```
#### 审核功能实现
- 在Teacher.cpp中实现成员函数`void Teacher::validOrder()`
- 代码如下； 
```c++
//审核预约
void Teacher::validOrder()
{
	OrderFile of;
	if (of.m_Size == 0)
	{
		cout << "无预约记录" << endl;
		system("pause");
		system("cls");
		return;
	}
	cout << "待审核得记录如下" << endl;
	vector<int>v;
	int intdex = 0;
	for (int i = 0;i < of.m_Size;i++)
	{
		if (of.m_orderDete[i]["status"] == "1")
		{
			v.push_back(i);
			cout << "预约日期； 周" << of.m_orderDete[i]["date"];
			cout << "时段" << (of.m_orderDete[i]["interval"] == "1" ? "上午" : "下午");
			cout << "机房； " << of.m_orderDete[i]["roomId"];
			string status = "状态";
			if (of.m_orderDete[i]["status"] == "1")
			{
				status += "审核中";
			}
			cout << status << endl;

		}
	}
	cout << "请输入审核的预约记录。0代表返回" << endl;
	int select = 0;
	int ret = 0;
	while (true)
	{
		cin >> select;
		if (select >= 0 && select <= v.size())
		{
			if (select == 0)
			{
				break;
			}
			else
			{
				cout << "请输入审核结果" << endl;
				cout << "1、通过" << endl;
				cout << "2、不通过" << endl;
				cin >> ret;
				if (ret == 1)
				{
					of.m_orderDete[v[select - 1]]["status"] = "2";
				}
				else
				{
					of.m_orderDete[v[select - 1]]["status"] = "-1";
				}
				of.updatOrder();
				cout << "审核完毕" << endl;
				break;
			}
		}
		cout << "输入有误请重新输入" << endl;
	}
	system("pause");
	system("cls");
}
```
