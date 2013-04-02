SqlGenerate
===========

SQL Generate é uma ferramenta para auxiliar na geração de SQL a partir de uma Entidade.


Exemplo

public class Product
{
    public string Id {get; set;}
    public string Name {get;set;}
}

class Program
{
    static void Main(string[] args)
    {
        Console.WriteLine(SqlGenerate.SQLSelect<Product>());
        //Result: SELECT * FROM Product
    }
}
