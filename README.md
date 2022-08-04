//void Zadacha64()
{
//  Задача 64: Задайте значения M и N. Напишите программу, которая выведет 
// все натуральные числа в промежутке от M до N, кратные трём.
// M = 1; N = 5. -> ""1, 2, 3, 4, 5""
// M = 4; N = 8. -> ""4, 6, 7, 8""
Console.WriteLine("Введите чилло- М:");
int M = Convert.ToInt32(Console.ReadLine());
Console.WriteLine("Введите число- N:");
int N = Convert.ToInt32(Console.ReadLine());
Console.WriteLine($"Числа из промежутка от {M} до {N}: ");
AllNumbers(M, N);
Console.WriteLine();
}

void AllNumbers(int m, int n)
{
    if (m > n)
    {
        return;
    }
    if (m % 3 == 0)
    {
        Console.Write(m + "\t");
    }
    m++;
    AllNumbers(m, n);
}
//Zadacha64();
