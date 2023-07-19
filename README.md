Задача 2: Напишите программу, которая на вход принимает два числа и выдаёт, какое число большее, а какое меньшее.
a = 5; b = 7 -> max = 7
a = 2 b = 10 -> max = 10
a = -9 b = -3 -> max = -3

Console.Write("Введите первое число: ");
int num1 = Convert.ToInt32(Console.ReadLine());
Console.Write("Введите второе число: ");
int num2 = Convert.ToInt32(Console.ReadLine());

if (num1 < num2 ){
     Console.WriteLine ("Первое число меньше второго");
} else if (num1 > num2 ){
     Console.WriteLine ("Первое число больше второго");
     }else{
     Console.WriteLine ("Числа равны");
 }


 Задача 4: Напишите программу, которая принимает на вход три числа и выдаёт максимальное из этих чисел. (Сравнить с каждым)

2, 3, 7 -> 7
44 5 78 -> 78
22 3 9 -> 22

int max = 0;

Console.Write("Введите первое число: ");
int num1 = Convert.ToInt32(Console.ReadLine());

Console.Write("Введите второе число: ");
int num2 = Convert.ToInt32(Console.ReadLine());

Console.Write("Введите третье число: ");
int num3 = Convert.ToInt32(Console.ReadLine());

if(num1 > max)
{
    max = num1;
}
if(num2 > max)
{
    max = num2;
}
if(num3 > max)
{
    max = num3;
}

Console.WriteLine("max = " + max);


Задача 6: Напишите программу, которая на вход принимает число и выдаёт, является ли число чётным (делится ли оно на два без остатка).

4 -> да
-3 -> нет
7 -> нет


Console.Write("Введите число: ");
int num = Convert.ToInt32(Console.ReadLine());

int rem = num % 2;

if(rem == 0)
{
    Console.WriteLine("Да");
}
else
{
    Console.WriteLine("Нет");
}


Задача 8: Напишите программу, которая на вход принимает число (N), а на выходе показывает все чётные числа от 1 до N.

5 -> 2, 4
8 -> 2, 4, 6, 8


Console.Write("Введите число: ");
int num1 = Convert.ToInt32(Console.ReadLine());

int num2 = 2;

if(num1 > 1)
{
    while(num2 <= num1)
    {
        Console.Write(num2 + " ");
        num2 = num2 + 2;
    }
}
