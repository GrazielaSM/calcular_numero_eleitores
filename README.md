# calcular_numero_eleitores
 /*Escreva um algoritmo para ler o número total de eleitores de um município, o número de votos brancos, nulos e válidos.Calcular e escrever o percentual que cada um representa em relação ao total de eleitores.*/
using System;
namespace calcular_numero_eleitores

{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello!");

            Console.WriteLine("Informe a quantidade de eleitores:");
            double eleitores = double.Parse(Console.ReadLine());

            Console.WriteLine("Informe quantidade de votos branco:");
            double brancos = double.Parse(Console.ReadLine());

            Console.WriteLine("Informe quantidade de votos nulos:");
            double nulos = double.Parse(Console.ReadLine());

            double porbranco = (brancos * 100) / eleitores;
            double  porcnulo = (nulos * 100) / eleitores;
            double porcvalido = eleitores - (brancos + nulos);


            Console.WriteLine("\nVotos Branco:" + porbranco + "%");
            Console.WriteLine("\nVotos Nulos:"+ porcnulo + "%");
            Console.WriteLine("\nVotos validos:" + porcvalido * 100 / eleitores + "%");
             
          Console.WriteLine();


        }
    }
}
