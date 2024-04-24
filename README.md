using ExemplosFundamentos.Models;

string opcao;

while(true)
{
    Console.Clear();
    Console.WriteLine("Digite a sua opção");
    Console.WriteLine("1 - Cadastrar Cliente");
    Console.WriteLine("2 - Buscar Cliente");
    Console.WriteLine("3 - Apagar Cliente");
    Console.WriteLine("4 - Encerrar");

#pragma warning disable CS8600 // Conversão de literal nula ou possível valor nulo em tipo não anulável.
    opcao = Console.ReadLine();
#pragma warning restore CS8600 // Conversão de literal nula ou possível valor nulo em tipo não anulável.

    switch (opcao)
    {
        case "1":
             Console.WriteLine("Cadastro de cliente");
             break;
        case "2":
             Console.WriteLine("Busca de cliente");
             break;
        case "3":
             Console.WriteLine("Apagar cliente");
             break;
        case "4":
             Console.WriteLine("Encerrar");
             Environment.Exit(0);
             break;

        default:
            Console.WriteLine("Opção Inválida");
            break;     
    }                        
}
