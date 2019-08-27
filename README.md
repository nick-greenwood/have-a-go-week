# Have a Go Week 2019 - C#

## Exercise One - Calculations
### Have a go
https://dotnetfiddle.net/WtLx0V
### The code
```csharp
using System;

public class Program
{
	public static void Main(string[] args)
	{
		var calculator = new Calculator();
		
		Console.WriteLine(string.Format("Addition: {0}", calculator.Add(7,3)));
		Console.WriteLine(string.Format("Subtraction: {0}", calculator.Subtract(8,4)));
		Console.WriteLine(string.Format("Multiplication: {0}", calculator.Multiply(9,3)));
		Console.WriteLine(string.Format("Division: {0}", calculator.Divide(12,3)));
	}
	
	public class Calculator
	{
		public int Add(int numberOne, int numberTwo)
		{
			return 0;
		}
		
		public int Subtract(int numberOne, int numberTwo)
		{
			return 0;
		}
		
		public int Multiply(int numberOne, int numberTwo)
		{
			return 0;
		}
		
		public int Divide(int numberOne, int numberTwo)
		{
			return 0;
		}
	}
}
```
### Expected output
```
Addition: 10
Subtraction: 4
Multiplication: 27
Division: 4
```
## Exercise Two
### Have a go
https://dotnetfiddle.net/Bwyjl5
### The code
```csharp
using System;
					
public class Program
{
	public static void Main()
	{
		var fizzBuzz = new FizzBuzz();
		
		Console.WriteLine(string.Format("Say: 1. Speak: {0}", fizzBuzz.Say(1)));
		Console.WriteLine(string.Format("Say: 2. Speak: {0}", fizzBuzz.Say(2)));
		Console.WriteLine(string.Format("Say: 3. Speak: {0}", fizzBuzz.Say(3)));
		Console.WriteLine(string.Format("Say: 4. Speak: {0}", fizzBuzz.Say(4)));
		Console.WriteLine(string.Format("Say: 5. Speak: {0}", fizzBuzz.Say(5)));
	}
	
	public class FizzBuzz
	{
		public string Say(int number)
		{
			if(number % 3 == 0)
			{
				return "TODO";
			}
			
			return number.ToString();
		}
	}
}
```
### Expected output
```
Say: 1. Speak: 1
Say: 2. Speak: 2
Say: 3. Speak: Fizz
Say: 4. Speak: 4
Say: 5. Speak: Buzz
```
