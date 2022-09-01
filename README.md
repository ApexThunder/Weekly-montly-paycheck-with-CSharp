using System;

class Program
{
    static void Main(string[] args)
    {
        double myHours = 37.5;
        double myRate = 15.75;
        double grossPay = 0;
        grossPay = CalcPay(myHours, myRate);
        Console.WriteLine($"I worked {myHours} hours at {myRate} per hour");
        Console.WriteLine($"My Gross pay is {grossPay:C}");

    }
    private static double CalcPay(double hours, double rate)
    {
        double gross;
        gross = hours * rate;
        return gross;
    }
}
