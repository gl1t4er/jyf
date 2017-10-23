using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Matrix
{
    class Program
    {
        static void Main(string[] args)
        {

            List<List<int>> mas1 = new List<List<int>>();
            List<List<int>> mas2 = new List<List<int>>();
            List<List<int>> mas3 = new List<List<int>>();


            Console.WriteLine("Введите размер матриц: ");
            int x = Convert.ToInt32(Console.ReadLine());

            Random rand = new Random();
            for (int i = 0; i < x; i++)
            {

                var t = new List<int>();
                for (int j = 0; j < x; j++)
                {
                    t.Add(rand.Next(1, 99));
                }
                mas1.Add(t);
            }

            for (int i = 0; i < x; i++)
            {
                var v = new List<int>();
                for (int j = 0; j < x; j++)
                {
                    v.Add(rand.Next(1, 99));
                }
                mas2.Add(v);
            }

            foreach (var q in mas1)
                Console.WriteLine(q.Aggregate("", (e, n) => e + " " + n));

            Console.WriteLine(Environment.NewLine);

            foreach (var t in mas2)
                Console.WriteLine(t.Aggregate("", (e, n) => e + " " + n));


            for (int i = 0; i < x; i++)
            {
                List<int> q = new List<int>();
                for (int j = 0; j < x; j++)
                {
                    q.Add(0);
                }
                mas3.Add(q);
            }
            for (int i = 0; i < x; i++)
            {
                for (int j = 0; j < x; j++)
                {
                    {
                        for (int w = 0; w < x; w++)
                        {
                            mas3[i][j] = mas3[i][j] + (mas1[i][w] * mas2[w][j]);
                        }
                    }
                }
            }
            Console.WriteLine("Результат");
            PrintValue(mas3);
            Console.ReadKey();
        }
        private static void PrintValue(List<List<int>> mas1)
        {
            foreach (var t in mas1)
                Console.WriteLine(t.Aggregate("", (e, n) => e + " " + n));

            Console.WriteLine(Environment.NewLine);

     

        }
    }
}
