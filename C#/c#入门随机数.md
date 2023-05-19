## 1.产生随机数对象

固定写法：

`Random 随机数变量名 = new Random();`

```c#
Random r = new Random();
```

## 2.生成随机数

```c#
int i =r.Next();	//生成一个非负数的随机数
Console.WriteLine(i);
```

```c#
i=r.Next(100);	//生成一个0~99的随机数，左边始终是0，左包含，右边是100，右不包含
Console.WriteLine(i);
i=r.Next(5,100);	//生成一个5~99的随机数。
```



