using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _4.If_Anidados
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int op;
            double n1, n2, r;

            Console.WriteLine("-----MENU DE OPERACIONES BÁSICAS-----");
            Console.WriteLine("1. Suma");
            Console.WriteLine("2. Multimplicación");
            Console.WriteLine("3. División\n");
            Console.WriteLine("Elije una opción:");
            op = int.Parse(Console.ReadLine());

            if (op == 1)
            {
                Console.WriteLine("Valor del primer n1: ");
                n1 = double.Parse(Console.ReadLine());
                Console.WriteLine("Valor del primer n2: ");
                n2 = double.Parse(Console.ReadLine());
                r = n1 + n2;
                Console.WriteLine("la suma de {0}+{1}={2}", n1, n2, r);
            }
            if (op == 2)
            {
                Console.WriteLine("Valor del primer n1: ");
                n1 = double.Parse(Console.ReadLine());
                Console.WriteLine("Valor del primer n2: ");
                n2 = double.Parse(Console.ReadLine());
                r = n1 * n2;
                Console.WriteLine("la multiplicación de {0}*{1}={2}", n1, n2, r);
            }
            if (op == 3)
            {
                Console.WriteLine("Valor del dividendo: ");
                n1 = double.Parse(Console.ReadLine());
                Console.WriteLine("Valor del divisor: ");
                n2 = double.Parse(Console.ReadLine());
                if (n2 != 0)
                {
                    r = n1 / n2;
                    Console.WriteLine("la división de {0}/{1}={2}", n1, n2, r);
                }
                else {
                    Console.BackgroundColor = ConsoleColor.Red; 
                    Console.WriteLine("Indeterminado"); }
            }

            ///--- Hacer el diagrama de flujo de este programa
            Console.ReadKey();
        }
    }
}
