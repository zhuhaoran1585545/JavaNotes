# 包装类
## 包装类简介
- Java语言提供了八种基本类型，六种数字类型（四个整数型，两个浮点型），一种字符类型，还有一种布尔型。
1. 整数：包括int,short,byte,long，初始值为0
2. 浮点型：float,double，初始值为0.0
3. 字符：char，初始值为空格，
4. 布尔：boolean，初始值为false  


    | 基本类别 | 大小 | 最小值 | 最大值 |
    | ------- | ---- | ----- | ------ |
    | boolean | ---- | ----- | ------ |
    | char    | 16bit | Unicode 0 | Unicode 2^16-1 |
    | byte    | 8bit | -128 | +127 |
    | short | 16bit | -2^15 | +2^15-1 |
    | int | 32bit | -2^31 | +2^31-1 |
    | long | 64bit | -2^63 | +2^63-1 |
    | float | 32bit | IEEE754 | IEEE754 |
    | double | 64bit | IEEE754 | IEEE754 | 
    | void 

- Java包装类中有，Integer,Long,Short,Byte,Character,Double,Float,Boolean,BigInterger,BigDecimal
- 其中，BigInterget,BigDecimal没有相对应的基本类型，主要应用于高精度的计算，BigInterget支持任意精度的整数，BigDecimal支持任意精度带小数点大的运算
### 包装类常用方法
查询JavaAPI
### 基本数据类型于包装类之间的转换
- 装箱
- 拆箱
```
    //1. 自动装箱
		int t1 = 2;
		Integer t2 = t1;
		// 2. 手动装箱
		Integer t3 = new Integer(3);
		// test
		System.out.println(t1);
		System.out.println(t2);
		System.out.println(t3);
		System.out.println("========================");
		// 拆箱
		// 1.自动拆箱
		int t4 = t3;
		// 2.手动拆箱
		int t5 = t2.intValue();
		// test
		System.out.println(t4);
		System.out.println(t5);
		double t6 = t2.doubleValue();
		System.out.println(t6);
```

```
		int t1 = 2;
		String t2 = Integer.toString(t1);
		System.out.println(t2);
		int t3 = Integer.parseInt(t2);
		int t4 = Integer.valueOf(t2);
		System.out.println(t3);
		System.out.println(t4);
```
## 注意


