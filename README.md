# Area-of-figures
using System;

namespace Area_of_Figures
{
    class Program
    {
        static void Main(string[] args)
        {
            string figures = Console.ReadLine();
            double result = 0;
            double a = 0;
            double b = 0;

            if (figures == "square")
            {
                a = double.Parse(Console.ReadLine());
                result = a * a;
            }
            else if(figures == "rectangle")
            {
                a = double.Parse(Console.ReadLine());
                b = double.Parse(Console.ReadLine());
                result = a * b;
            }
            else if(figures == "circle")
            {
                a = double.Parse(Console.ReadLine());
                result = Math.PI * a * a;
            }
            else if(figures == "triangle")
            {
                a = double.Parse(Console.ReadLine());
                b = double.Parse(Console.ReadLine());
                result = (a * b) / 2;
            }

            Console.WriteLine("{0:F3}", result);
        }
    }
}
