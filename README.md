# C#

知らなかった機能：<br>
- goto文


<br>

```
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
 
namespace Test
{
    class Program
    {
        static void Main(string[] args)
        {
            int a = 10; 
            int b = 20;
            Console.WriteLine("Max : {0}, Min : {1}, Size : {2}", uint.MaxValue, uint.MinValue, sizeof(uint));
            Console.WriteLine("{0} + {1} = {2}", a, b, a + b);
            Console.WriteLine("a < b = {0}", a < b);

            object obj = null;
            string str = "";
            Console.WriteLine("hello");

            if(a > b)
            {
                Console.WriteLine("a>b");
            }
            else if(a == b)
            {
                Console.WriteLine("a==b");
            }
            else
            {
                Console.WriteLine("a<b");
            }

            switch (a)
            {
                case 10:
                {
                    Console.WriteLine("10");
                    break;
                }
                case 20:
                {
                    Console.WriteLine("20");
                    continue;
                }
                default:
                {
                    Console.WriteLine("null");
                    break;
                }
            }

            while(true)
            {
                Console.WriteLine("a : {0}", a++);
                if (a >= 15)
                    break;
            }

            do
            {
                Console.WriteLine("a : {0}", a--);
            }
            while (a > 10);

            for(int i = 0; i < 5; i++)
            {
                Console.WriteLine("i : {0}", i);
            }
            test:

            int[] arr = {1, 2, 3, 4};
            foreach(int i in arr)
            {
                Console.WriteLine("arr : {0}",i);
            }
            
            goto test;
        }
    }
}
```
