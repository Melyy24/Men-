using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace menu
{
    class Program
    {
        static void Main(string[] args)

        {
        
            bool inf = false;
            String menu = "";
            while (inf == false)
            {
                Console.WriteLine("ingrese cualquier opcion: .1 Saludar .2 Fecha .3 cerrar");
                Conso
                menu = Console.ReadLine();
                switch (menu)
                {
                    case "1":
                        Console.WriteLine("ingrese su nombre:");
                        String n = Console.ReadLine();
                        Console.WriteLine("hola " + n + " como esta tu día?");
                        Console.ReadLine();
                        Console.Clear();

                        break;
                    case "2":
                        Console.WriteLine("la fecha de es 6/5/2025");
                        Console.ReadLine();
                        Console.Clear();

                        break;
                    case "3":
                        bool decision = false;
                        Console.WriteLine("ingrese si o no, si quiere cerrar el programa");
                        String P = Console.ReadLine();
                        if (P == "si" || P == "SI")
                        {
                            decision = true;
                        }
                        else if (P == "no" || P == "NO")
                        {
                            decision = false;
                        }
                        bool decisionF = cerrar(decision);
                        if (decisionF = true)
                        {
                            return;
                        }
                        break;
                        
                }
            }
        }
        
        static bool cerrar(bool d)
        {

            
            if (d == false)
            {
                Console.WriteLine("sigamos con el programa");
                Console.ReadLine();
                Console.Clear();
                return false;

            }
            else
            {

                Console.WriteLine("cerrando programa...");
                return true;
                
            }

        }
    }
}
