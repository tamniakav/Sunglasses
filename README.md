using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Sunglasses
{
    class Program
    {
        static void Main(string[] args)
        {
            int n = int.Parse(Console.ReadLine());

            Console.WriteLine("{0}{1}{0}", new string('*', 2 * n), new string(' ', n));

            for (int i = 0; i < n - 2; i++)
            {
                char simbol = ' ';
                
                if ((n - 1) / 2 - 1 == i)
                {
                    simbol = '|';
                }
                Console.WriteLine("*{0}*{1}*{0}*", new string('/', (n * 2)- 2), new string(simbol, n));
            }

            Console.WriteLine("{0}{1}{0}", new string('*', 2 * n), new string(' ', n));
        }
    }
}
