# Have a Go Week 2019 - C#
## Contents
1. [Introduction](#introduction)
2. [Exercise One](#exercise-one---calculations)
3. [Exercise Two](#exercise-two---fizzbuzz)
4. [Exercise Three](#exercise-three---human)
## Introduction
Welcome to the Have a Go Week session for C#.

Each exercise is broken down into four parts:
1. **The exercise** - the explanation of the problem
2. **Expected output** - What you should expect the code to output if you code is correct
3. **Have a go** - The editor for your code. This is where you will see the code and change it. You can run the code at any point by clicking Run

![run](/.attachments/ide.png)

4. **The code** - The starting point for the code, before any changes are made
5. **Hints** - Any tips we think might be useful
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
https://dotnetfiddle.net/y9VZuC
### The code
```csharp
using System;

public class Program
{
	public static void Main(string[] args)
	{
		var calculator = new Calculator();
		
		Console.WriteLine($"Addition: {calculator.Add(7,3)}");
		Console.WriteLine($"Subtraction: {calculator.Subtract(8,4)}");
		Console.WriteLine($"Multiplication: {calculator.Multiply(9,3)}");
		Console.WriteLine($"Division: {calculator.Divide(12,3)}");
	}
	
	public class Calculator
	{
		public int Add(int numberOne, int numberTwo)
		{
			// Change the code here
			return 0;
		}
		
		public int Subtract(int numberOne, int numberTwo)
		{
			// Change the code here
			return 0;
		}
		
		public int Multiply(int numberOne, int numberTwo)
		{
			// Change the code here
			return 0;
		}
		
		public int Divide(int numberOne, int numberTwo)
		{
			// Change the code here
			return 0;
		}
	}
}
```
### Hints
```
What do the following symbols do?
* / + -
```
## Exercise Two - FizzBuzz
### The exercise
Fix the below code so that you have built a FizzBuzz game. Rules: https://en.wikipedia.org/wiki/Fizz_buzz
### Expected output
```
Say: 1. Speak: 1
Say: 2. Speak: 2
Say: 3. Speak: Fizz
Say: 4. Speak: 4
Say: 5. Speak: Buzz
```
### Have a go
https://dotnetfiddle.net/DX0lrZ
### The code
```csharp
using System;
					
public class Program
{
	public static void Main()
	{
		var fizzBuzz = new FizzBuzz();
		
		Console.WriteLine($"Say: 1. Speak: {fizzBuzz.Say(1)}");
		Console.WriteLine($"Say: 2. Speak: {fizzBuzz.Say(2)}");
		Console.WriteLine($"Say: 3. Speak: {fizzBuzz.Say(3)}");
		Console.WriteLine($"Say: 4. Speak: {fizzBuzz.Say(4)}");
		Console.WriteLine($"Say: 5. Speak: {fizzBuzz.Say(5)}");
	}
	
	public class FizzBuzz
	{
		public string Say(int number)
		{
			// Change the code in here
			
			if(number % 3 == 0)
			{
				return "TODO";
			}
			
			return number.ToString();
		}
	}
}
```
### Hints
```
% 3 == 0
Checks if a number divides by 3
```
## Exercise Three - Human
### The exercise
Change the code so that the output is correct.
### Expected output
```
Joe Bloggs. Engineer. 30 years old.
```
### Have a go
https://dotnetfiddle.net/Ug7weJ
### The code
```csharp
using System;
					
public class Program
{
	public static void Main()
	{
		var human = new Human("Joe", "Bloggs", "Engineer", DateTime.Now.AddYears(-31).AddMonths(4));
		
		Console.WriteLine($"{human.FullName()}. {human.JobTitle()}. {human.Age()}");
	}
	
	public class Human
	{
		private string _firstName;
		private string _surname;
		private string _jobTitle;
		private DateTime _dateOfBirth;
		
		public Human(string firstName, string surname, string jobTitle, DateTime dateOfBirth)
		{
			_firstName = firstName;
			_surname = surname;
			_jobTitle = jobTitle;
			_dateOfBirth = dateOfBirth;
		}
		
		public string FullName()
		{
			// Change the code in here
			return "";
		}
		
		public string JobTitle()
		{
			// Change the code in here
			return "";
		}
		
		public int Age()
		{
			// Change the code in here
			return 0;
		}
	}
}
```
### Hints
```csharp
//If you have a DateTime variable you can
variable.Year //To get the year part. E.g. 2019
variable.Month //To get the month part. E.g. 7 for July
variable.Day //To get the day part. E.g. 23

//If you want the current date time you can
var currentDate = DateTime.Now;
```
