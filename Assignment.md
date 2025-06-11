# แบบฝึกหัดที่ 1
## ข้อ 1 ให้ใช้ AI สร้างโปรแกรมที่มีความสามารถต่อไปนี้ ใน Polyglot notebook
- นับเลข 1 – 100
 // แสดงเลขคู่ 1-100
Console.WriteLine("เลขคู่ 1-100:");
for (int i = 1; i <= 100; i++)
{
    if (i % 2 == 0)
        Console.Write($"{i} ");
}
Console.WriteLine("\n");

// แสดงเลขคี่ 1-100
Console.WriteLine("เลขคี่ 1-100:");
for (int i = 1; i <= 100; i++)
{
    if (i % 2 != 0)
        Console.Write($"{i} ");
}
Console.WriteLine("\n");

// แสดงจำนวนเฉพาะ 1-100
Console.WriteLine("จำนวนเฉพาะ 1-100:");
for (int i = 2; i <= 100; i++)
{
    bool isPrime = true;
    for (int j = 2; j <= Math.Sqrt(i); j++)
    {
        if (i % j == 0)
        {
            isPrime = false;
            break;
        }
    }
    if (isPrime)
        Console.Write($"{i} ");
}
Console.WriteLine();
เลขคู่ 1-100:
2 4 6 8 10 12 14 16 18 20 22 24 26 28 30 32 34 36 38 40 42 44 46 48 50 52 54 56 58 60 62 64 66 68 70 72 74 76 78 80 82 84 86 88 90 92 94 96 98 100 

เลขคี่ 1-100:
1 3 5 7 9 11 13 15 17 19 21 23 25 27 29 31 33 35 37 39 41 43 45 47 49 51 53 55 57 59 61 63 65 67 69 71 73 75 77 79 81 83 85 87 89 91 93 95 97 99 

จำนวนเฉพาะ 1-100:
2 3 5 7 11 13 17 19 23 29 31 37 41 43 47 53 59 61 67 71 73 79 83 89 97 

## ข้อ 2 ให้ใช้ AI สร้างโปรแกรมที่มีความสามารถต่อไปนี้ ใน Polyglot notebook
- รับค่าอายุทางคีย์บอร์ด
  // See https://aka.ms/new-console-template for more information
Console.Write("กรุณากรอกอายุ: ");
int age = int.Parse(Console.ReadLine());

if (age >= 1 && age <= 12)
{
    Console.WriteLine("เด็ก");
}
else if (age >= 13 && age <= 19)
{
    Console.WriteLine("วัยรุ่น");
}
else if (age >= 20 && age <= 50)
{
    Console.WriteLine("วัยผู้ใหญ่");
}
else if (age >= 51)
{
    Console.WriteLine("วัยชรา");
}
else
{
    Console.WriteLine("กรุณากรอกอายุที่ถูกต้อง");
}
