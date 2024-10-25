# ProjetoForIdade
Idem (25/10).

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ProjetoForIdade
{
    public class Program
    {
        static void Main(string[] args)
        {
            /*Solicite e receba o nome e o ano de nascimento do usuario e exiba
             * os dados informados e o calculo da idade. Faça esta repetição
             * para seis usuarios.
            */
            string nome;
            int anoNasc, idade;

            for (int i = 0; i < 6; i++)
            {
                Console.WriteLine("Informe seu nome: ");
                nome = Console.ReadLine();

                Console.WriteLine("Digite o ano de nascimento do usuario: ");
                anoNasc = Convert.ToInt32(Console.ReadLine());

                idade = DateTime.Now.Year - anoNasc;
                Console.WriteLine("Nome: " + nome);
                Console.WriteLine("Idade: " + idade);
            }
            Console.ReadKey();
        }
    }
}
