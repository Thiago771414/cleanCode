# Clean Code
  A técnica "Clean Code" refere-se a práticas de desenvolvimento de software que enfatizam a legibilidade, manutenibilidade e organização do código.

Escolha nomes descritivos: Dê nomes significativos às variáveis, métodos e classes. Evite abreviações e nomes genéricos. Os nomes devem transmitir claramente a intenção e o propósito do código.

Mantenha métodos curtos: Divida seu código em métodos menores e mais focados. Cada método deve ter uma única responsabilidade e ser fácil de entender. Evite métodos muito longos e complexos.

Evite duplicação de código: Procure por trechos de código repetidos e extraia-os para métodos ou classes reutilizáveis. Dessa forma, você reduz a duplicação e facilita a manutenção futura.

Organize seu código em classes e namespaces: Agrupe seu código em classes de acordo com sua funcionalidade e responsabilidade. Use namespaces para organizar classes relacionadas. Isso tornará seu código mais estruturado e fácil de navegar.

Comente o código adequadamente: Use comentários para explicar partes do código que possam não ser óbvias. No entanto, é melhor ter um código autoexplicativo. Evite comentários excessivos e redundantes.

Limite o escopo das variáveis: Declare variáveis com o menor escopo possível. Isso ajuda a reduzir a complexidade do código e evita efeitos colaterais indesejados.

Escreva testes unitários: Desenvolva testes unitários para verificar o comportamento do seu código. Isso ajuda a garantir que o código seja confiável e facilita a detecção de problemas.

Refatore regularmente: Esteja disposto a refatorar seu código regularmente para melhorar sua qualidade. Identifique oportunidades de melhoria e faça ajustes contínuos.

```csharp
using System;

namespace CleanCodeExample
{
    class Program
    {
        static void Main()
        {
            var calculator = new Calculator();

            var result = calculator.Add(5, 7);
            Console.WriteLine($"The sum is: {result}");

            var isValid = InputValidator.Validate("OpenAI");
            Console.WriteLine($"Is valid input? {isValid}");

            Console.ReadLine();
        }
    }

    class Calculator
    {
        public int Add(int a, int b)
        {
            return a + b;
        }
    }

    class InputValidator
    {
        public static bool Validate(string input)
        {
            if (string.IsNullOrWhiteSpace(input))
            {
                return false;
            }

            return input.Length >= 5;
        }
    }
}
```

# Autor
Thiago Reis Lima
https://www.linkedin.com/in/thiago-lima-2a5896166/
