using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace ConsoleApplication1
{
    class Program
    {
        static void Main(string[] args)
        {
            List<int> szamok = new List<int>();
            Random veletlen = new Random();
            for (int i = 0; i < 20; i++)
            {
                szamok.Add(veletlen.Next(1, 100));
                Console.Write("{0},", szamok[i]);

            }
            Console.WriteLine();
            Console.WriteLine("A lista páros elemei: ");
            foreach (int item in szamok)
            {
                if (item % 2 == 0)
                {
                    Console.Write("{0},", item);
                }
            }
            Console.ReadKey();

        }
    }
}
