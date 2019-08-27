# Have a Go Week 2019 - C#
## Introduction
Welcome to the Have a Go Week session for C#.

Each exercise is broken down into four parts:
1. **The exercise** - the explanation of the problem
1. **Expected output** - What you should expect the code to output if you code is correct
1. **Have a go** - The editor for your code. This is where you will see the code and change it. You can run the code at any point by clicking Run
1. **The code** - The code that will be changed to pass the exercise
## Exercise One - Calculations
### The exercise
Fix the below code so that the Add, Subtract, Multiply and Divide methods return the correct answers.
### Expected output
```
Addition: 10
Subtraction: 4
Multiplication: 27
Division: 4
```
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
## Exercise Two
### The exercise
Fix the below code so that you have built a FizzBuzz game.
### Expected output
```
Say: 1. Speak: 1
Say: 2. Speak: 2
Say: 3. Speak: Fizz
Say: 4. Speak: 4
Say: 5. Speak: Buzz
```
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
