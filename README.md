# Convers-o-de-Temperatura
Entregar até 18/10/24

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
            string Temperatura;
            decimal º;

            Console.WriteLine("Informe a Temperatura em Celsius: ");
            Temperatura = Convert.ToDouble(Console.ReadLine());
            Fahrenheit = (Celsius * 9/5) + 32;
            Kelvin = (Celsius + 273.15);
            Console.WriteLine("Exiba o resultado " + Celsius + "para" + Fahrenheit + Kelvin);

            if ( Temperatura <= 0ºC)
                {
                Console.WriteLine("Muito Fria");
            }
            else if ( Temperatura entre 0ºC e 30ºC)
                {
                Console.WriteLine("Moderada");
            }
            else ( Temperatura >= 30ºC)
                {
                Console.WriteLine("Muito Quente");
            }


            Console.ReadKey();
        }
    }
}
