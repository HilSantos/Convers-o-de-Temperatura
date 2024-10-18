# Converter-Temperatura
Crie um programa que solicite ao usuario, uma temperatura em graus Celsius, e a converta em Fahrenheit e Kelvin. Utilize as formulas:
Fahrenheit = (Celsius * 9/5) + 32
Kelvin = Celsius + 273.15. Exiba os resultados no console e utilize if...else para exibir uma mensagem, dizendo se a temperatura está "Muito fria", "Moderada" ou "Muito quente":
Abaixo de 0 graus C:"Muito Fria"; Entre 0 graus C e 30 graus C:"Moderada"; Acima de 30 graus C:"Muito Quente"  
Entregar até 18/10/24
______________________________________________________________________________________________________________________________________________________________________________________________________
using System;
using System.Collections.Generic;
using System.Diagnostics.Eventing.Reader;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConversaoTemperatura
{
    public class Program
    {
        static void Main(string[] args)
        {
            Double Celsius, Fahrenheit, Kelvin;


                        Console.WriteLine("Informe a Temperatura em Celsius: ");
            Celsius = Convert.ToDouble(Console.ReadLine());

            Fahrenheit = (Celsius * 9/5) + 32;
            Kelvin = (Celsius + 273.15);


            Console.WriteLine("Exiba o resultado " + Celsius + "para" + Fahrenheit + Kelvin);

            if (Celsius <= 0)
            {
                Console.WriteLine("Muito Fria");
            }
            else if (Celsius >= 0 && Celsius < 30)
            {
                Console.WriteLine("Moderada");
            }
            else (Celsius > 30)
                {
                Console.WriteLine("Muito Quente");
            }


            Console.ReadKey();
        }
    }
}


            Console.ReadKey();
        }
    }
}
