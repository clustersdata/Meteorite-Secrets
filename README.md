# Meteorite-Secrets

Meteorite Secrets

Description

公元11380年，一颗巨大的陨石坠落在南极。于是，灾难降临了，地球上出现了一系列反常的现象。当人们焦急万分的时候，一支中国科学家组成的南极考察队赶到了出事地点。经过一番侦察，科学家们发现陨石上刻有若干行密文，每一行都包含5个整数： 
1 1 1 1 6 
0 0 6 3 57 
8 0 11 3 2845 
著名的科学家SS发现，这些密文实际上是一种复杂运算的结果。为了便于大家理解这种运算，他定义了一种SS表达式： 
1．	SS表达式是仅由'{'，'}'，'['，']'，'（'，'）'组成的字符串。 
2．	一个空串是SS表达式。 
3．	如果A是SS表达式，且A中不含字符'{'，'}'，'['，']'，则(A)是SS表达式。 
4．	如果A是SS表达式，且A中不含字符'{'，'}'，则[A]是SS表达式。 
5．	如果A是SS表达式，则{A}是SS表达式。 
6．	如果A和B都是SS表达式，则AB也是SS表达式。 


例如 
()(())[] 
{()[()]} 
{{[[(())]]}} 
都是SS表达式。 
而 
()([])() 
[() 
不是SS表达式。 

一个SS表达式E的深度D(E)定义如下： 
 
例如(){()}[]的深度为2。 

密文中的复杂运算是这样进行的： 
设密文中每行前4个数依次为L1，L2，L3，D，求出所有深度为D，含有L1对{}，L2对[]，L3对()的SS串的个数，并用这个数对当前的年份11380求余数，这个余数就是密文中每行的第5个数，我们称之为?神秘数?。 
密文中某些行的第五个数已经模糊不清，而这些数字正是揭开陨石秘密的钥匙。现在科学家们聘请你来计算这个神秘数。

Input

共一行，4个整数L1，L2，L3，D。相邻两个数之间用一个空格分隔。 
（0 <= L1 <= 10，0 <= L2 <= 10，0 <= L3 <= 10，0 <= D <= 30）

Output

共一行，包含一个整数，即神秘数。

Sample Input

1 1 1 2

Sample Output

8
