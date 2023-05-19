## 1.常用控制台方法

```c#
 Console.WriteLine("");	//光标空行
 Console.WriteJ("");	//光标不空行
 Console.ReadLine();
 char a = Console.ReadKey().KeyChar;	//readkey需要进行类型转换。
```

`Console.ReadKey(true).KeyChar;`如果往readkey中传入关键词true，那么在控制台中将

不会显示你输入的值。

## 2.控制台其它方法

```c#
Console.Clear();	//清空控制台显示的内容
```

```c#
//设置控制台大小
//窗口大小，缓冲区大小
//1、先设置窗口大小，再设置缓冲区大小
//2、缓冲区的大小不能小于窗口的大小
//3、窗口的大小不能大于控制台的最大尺寸
//窗口大小
Console.SetWindows(100,50);	//也可以通过右键控制台窗口通过修改属性进行修改
//缓冲区大小（可打印内容区域的宽高，通过白色的滑动条体现
Console.SetBufferSize(100,50);	
//设置光标的位置
//控制台左上角为原点0 0右侧是x轴正方向，下方是y轴正方向，是一个平面2维坐标系
//要注意：
//1.边界问题
//2.在视觉上横纵距离单位不同 1y=2x
==console.SetCursorPosition(0,1);==
```

```c#
//设置颜色相关
//文字颜色设置
Console.ForegroundColor = ConsoleColor.Red;	//设置后其后面的文字输出颜色都会改变
Console.WriteLine("123123123");
//背景颜色设置
Console.BackgroundColor = ConsoleColor.White;
//重置背景颜色过后，需要Clear一次才能把整个背景颜色改变
Console.Clear();
```

```c#
//光标显隐
Console.CursorVisible = false;	//控制台中无光标出现。
```

```c#
//关闭控制台（退出游戏的功能）
Enviroment.Exit(0);
```

```c#
//获取缓冲区的高和宽
Console.BufferWidth;	//获取缓冲区的宽
Console.BufferHeight;	//获取缓冲区的高
```



