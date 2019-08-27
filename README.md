# Have a Go Week 2019 - C#
## Introduction
Welcome to the Have a Go Week session for C#.

Each exercise is broken down into four parts:
1. **The exercise** - the explanation of the problem
2. **Expected output** - What you should expect the code to output if you code is correct
3. **Have a go** - The editor for your code. This is where you will see the code and change it. You can run the code at any point by clicking Run

![run](/.attachments/ide.png)

4. **The code** - The starting point for the code, before any changes are made
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

<iframe
  src="https://carbon.now.sh/embed?bg=rgba(171%2C%20184%2C%20195%2C%201)&t=seti&wt=none&l=text%2Fx-csharp&ds=true&dsyoff=20px&dsblur=68px&wc=true&wa=true&pv=56px&ph=56px&ln=false&fl=1&fm=Hack&fs=14px&lh=133%25&si=false&es=2x&wm=false&code=using%2520System%253B%250A%250Apublic%2520class%2520Program%250A%257B%250A%2509public%2520static%2520void%2520Main(string%255B%255D%2520args)%250A%2509%257B%250A%2509%2509var%2520calculator%2520%253D%2520new%2520Calculator()%253B%250A%2509%2509%250A%2509%2509Console.WriteLine(string.Format(%2522Addition%253A%2520%257B0%257D%2522%252C%2520calculator.Add(7%252C3)))%253B%250A%2509%2509Console.WriteLine(string.Format(%2522Subtraction%253A%2520%257B0%257D%2522%252C%2520calculator.Subtract(8%252C4)))%253B%250A%2509%2509Console.WriteLine(string.Format(%2522Multiplication%253A%2520%257B0%257D%2522%252C%2520calculator.Multiply(9%252C3)))%253B%250A%2509%2509Console.WriteLine(string.Format(%2522Division%253A%2520%257B0%257D%2522%252C%2520calculator.Divide(12%252C3)))%253B%250A%2509%257D%250A%2509%250A%2509public%2520class%2520Calculator%250A%2509%257B%250A%2509%2509public%2520int%2520Add(int%2520numberOne%252C%2520int%2520numberTwo)%250A%2509%2509%257B%250A%2509%2509%2509return%25200%253B%250A%2509%2509%257D%250A%2509%2509%250A%2509%2509public%2520int%2520Subtract(int%2520numberOne%252C%2520int%2520numberTwo)%250A%2509%2509%257B%250A%2509%2509%2509return%25200%253B%250A%2509%2509%257D%250A%2509%2509%250A%2509%2509public%2520int%2520Multiply(int%2520numberOne%252C%2520int%2520numberTwo)%250A%2509%2509%257B%250A%2509%2509%2509return%25200%253B%250A%2509%2509%257D%250A%2509%2509%250A%2509%2509public%2520int%2520Divide(int%2520numberOne%252C%2520int%2520numberTwo)%250A%2509%2509%257B%250A%2509%2509%2509return%25200%253B%250A%2509%2509%257D%250A%2509%257D%250A%257D"
  style="transform:scale(0.7); width:1024px; height:473px; border:0; overflow:hidden;"
  sandbox="allow-scripts allow-same-origin">
</iframe>

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
## Exercise Three
### The exercise
Change the code so that the output is correct.
### Expected output
```
Joe Bloggs. Engineer. 31 years old.
```
### Have a go
https://dotnetfiddle.net/x9uXNP
### The code
```csharp
using System;
					
public class Program
{
	public static void Main()
	{
		var human = new Human("Joe", "Bloggs", "Engineer", DateTime.Now.AddYears(-31).AddMonths(4));
		
		Console.WriteLine(string.Format("{0}. {1}. {2} years old.", human.FullName(), human.JobTitle(), human.Age()));
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
			return "";
		}
		
		public string JobTitle()
		{
			return "";
		}
		
		public int Age()
		{
			return 0;
		}
	}
}
```
