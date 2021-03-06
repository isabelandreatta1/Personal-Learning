# Java Level 1 

## Types of variables
```java script
public class Application {

	public static void main(String[] args) {
		int myNumber = 88; //for integer numbers, 32 bit **most used** 
		short myShort = 847; //typically for shorter numbers, 16 bit
		long myLong = 9778; //typically for longer numbers, 64 bit 
		double myDouble = 7.23484; //for extra precision **most used**
		float myFloat = 243.3f; //similar to float 
		char myChar = '@'; //short for characters, use single quotes, unicode 
		boolean myBoolean = true; 
		String myString = "I like to stroke cat's bellies in my spare time"; 
		//uses "S" because is a class 

		byte myByte = 127; 
		
		System.out.println(myNumber);
		System.out.println(myShort);
		System.out.println(myLong);
		System.out.println(myDouble);
		System.out.println(myFloat);
		System.out.println(myChar);
		System.out.println(myBoolean);
		System.out.println(myByte); 
		System.out.println(myString); 
	}
}
```
**Most important variables for IB Java:** 

1. String
2. Integer 
3. Double
4. Boolean
5. Char 

We want to make sure we are using the right variable for what it will contain. This is so our value will just fit in. Code does work if you use a variable that is larger, but it is a waste and we want faster programs. 

The difference between String and other variables (such as int) is that String is a class and other are primitive. Primitive means that it is already built in Java and is like a box that contains values. A class is more like an address or a reference to something. This is conveninent since we don't know exactly how much a our text will be for our String. 

## String
```javascript
public class Application {
	public static void main(String[] args) {
		int myInt= 69; 
		
		System.out.println("Hello"+" "+"Isabel"+ myInt);
	//adding on strings is called concatenation 
		double myDouble = 420.69;
		System.out.println("My number is:" + myDouble +".");
	}
}
```
## While loops
```javascript

public class Application {
	public static void main(String[] args) {
		
		int value = 0; 
		
		while(value < 10) //condition is in brackets
		{ //what's inside curly brackets is when the loop will stop 
			System.out.println("Hello" + value );
			
			value = value + 1;
		}
	}
}
```
**Difference between for loops and while loops:**


format for loops: for([Initial expression];[condition];[incrementExpression])
This is good for when you know already how many loops you want


for while loops: 
This is good for when you don't know how many loops you want 

## For loops

```javascript
public class Application {
	public static void main(String[] args) {
  
  /*first section contains code before loop, second section contains
  condition so it will happen (also can be considered as limit in this case, third section condition
  once after iteration of loop*/
  
		for(int i = 1; i < 6; i = i + 1 ) { 
			System.out.println(i + "bear");
		}
	}
}
```
**Printf**
```javascript
public class Application {
	public static void main(String[] args) {
		
		for(int i = 1; i < 6; i = i + 1 ) { //first semicolon is what is before the code and second is condition
			System.out.printf(i + " Days without an accident: %d\n", i);
		}	
	}
	
}
```

- printf uses arguments
- first argument is string (format specifier) which uses special symbols and will be replaced with our variables
- %d -> print this integers but replace with the variable after the comma
- Printf does not have new lines, replace this by using /n 

## If Conditions 

```javascript

public class Application {
	public static void main(String[] args) {
		
		int myInt = 15;
		
		if(myInt > 30) {
			System.out.println("That's true brotha");
		}
		
		else if(myInt < 10){ 
			System.out.println("That ain't true brotha");
		}
		
		else {
			System.out.println("Nah nothing ain't real");
		}
		/* != means not equal to 
		 = one = means assigning, while == means testing 
		else if is an alternative, only happens if top is true*/
	}
}
```
**If conditions with while loops**
```javascript
public class Application {
	public static void main(String[] args) {
		int loop = 0;
		while(true) {
			System.out.println("yuh");
			
		if(loop == 5){
			break;
			}
		loop ++; 
		
		System.out.println("add 1 brudda");
		}
	}
}
```
## User Input 
**With String**
```javascript
import java.util.Scanner;

public class Application {
	public static void main(String[] args) {
		
		//create scanner object
		Scanner input = new Scanner(System.in); 
		
		//output prompt
		System.out.println("What's your name:");
		
		//wait for the user to enter a line 
		String line = input.nextLine();
		
		//Tell them what they entered 
		System.out.println("Welcome Back " + line);
	}
}

```
**With float**
```javascript
import java.util.Scanner;

public class Application {
	public static void main(String[] args) {
		
		//create scanner object
		Scanner input = new Scanner(System.in); 
		
		//output prompt
		System.out.println("Enter a floating point value");
		
		//wait for the user to enter a line 
		double value = input.nextDouble();
		
		//Tell them what they entered 
		System.out.println("Number " + value);
	}
}
```
## Do...While 
```javascript
import java.util.Scanner;

public class Application {
	public static void main(String[] args) {
		
		Scanner scanner = new Scanner(System.in); 
		
		/*
		System.out.println("Enter a number:");
		
		int value = scanner.nextInt();
		
		while(value!= 5) {
			System.out.println("Enter different number:");
			value = scanner.nextInt(); 
		}
		*/ 
		int value = 0; 
		
		do {
			System.out.println("Enter a number:");
			value = scanner.nextInt(); 
		}
		while(value != 5); 
			
		System.out.println("Got 5!");
	}
}
``` 
## Switch
```javascript
import java.util.Scanner;

public class Application {
	public static void main(String[] args) {
		
		Scanner input = new Scanner(System.in); 
		
		System.out.println("Enter command");
		String text = input.nextLine();
		
		switch(text) {
		
		case "start":
			System.out.println("Machine started dawg");
			break; 
			
		default:
			System.out.println("Password not recognised");
					
		}	
	}	
}
```
## Arrays
```javascript

import java.util.Scanner;

public class Application {
	public static void main(String[] args) {
		
	//bucket 
	int value = 7; 
	
	//reference 
	int[] values; 
	values = new int[3]; 
	
	System.out.println(values[0]);
	
	values[0] = 10; 
	values[1] = 20;
	values[2] = 30;
	
	System.out.println(values[0]);
	System.out.println(values[1]);
	System.out.println(values[2]);
	
	for(int i = 0; i < values.length; i ++ ) {
		System.out.println(values[i]);
		
		}
	
	int[]numbers = {5,6,7}; 
	
	for(int i = 0; i < numbers.length; i ++) 
		System.out.println(numbers[i]);
	}	 
}
```
## String Arrays 
```javascript
public class Application {
	public static void main(String[] args) {	
		String[] words = new String[3];
		
		words[0] = "Hello";
		words[1] = "to";
		words[2] = "you";
		
		System.out.println(words[2]);
		
		String[] fruits = {"apple", "orange", "banana"};
		
		for(String fruit: fruits) {
			System.out.println(fruit);
		}
		
		//defaults 
		int value = 0; 
		
		String text = null;
		
		System.out.println(text);
		
		String[] texts = new String[2]; 
		
		System.out.println(texts[0]);
		
		texts[0] = "one";
	}
}
```
## Multi-Dimmensional Arrays 
```javascript
public class Application {
	public static void main(String[] args) {
		
		int[][] grid = {
				{3,5,2344},//row 0
				{2,488}, //row 1
				{1,2,3,4}	//row 2
		}; 
		
		System.out.println(grid[1][0]); //[row][column]
		System.out.println(grid[0][2]);
		
		String[][]texts = new String[2][3];
		
		texts[0][1]= "Hello there";
		
		System.out.println(texts[0][1]);
		
		for(int row = 0; row<grid.length; row++) {
			for(int col = 0; col<grid[row].length; col++) {
				System.out.print(grid[row][col] + "\t");
			}
			System.out.println();
		}
	}
}
```
## Concept of Classes and Objects 
A class can be seen as a blueprint to create an object. 
```javascript
class Person{
	
	//Instance variables (data or "state")
	String name; 
	int age; 
	String sex; 
	
	/* classes can obtain
	 1. Data / State 
	 2.Subroutines (Methods)
	 */
}

class Book{
	String title; 
	String author; 
	int pagenb; 
	int published;
	
}

public class Application {
	public static void main(String[] args) {
		
	Person person1 = new Person(); 
	
	person1.name = "Karen White"; 
	person1.age = 43; 
	person1.sex = "Female"; 
	
	Person person2 = new Person(); 
	 
	person2.name = "Chad Bigboi"; 
	person2.age = 19; 
	person2.sex = "Male"; 
	
	System.out.println(person1.name + " " + person1.age);
	
	Book book1 = new Book(); 
	book1.title = "Don Quixote"; 
	book1.author = "Miguel de Cervantes"; 
	book1.pagenb = 992; 
	book1.published = 1605; 
		
		
		
	}
}
```
## Methods
```javascript
class Person{
	
	//Instance variables (data or "state")
	String name; 
	int age; 
	String sex; 
	
	/* classes can obtain
	 1. Data / State 
	 2.Subroutines (Methods)
	 */
	void speak() { //can be considered as a behaviour of the object
		for(int i=0; i<3; i++) {
			System.out.println("My name is: " + name + " and I am " + age + " years old.");
		
		}
	}
	
	void gender() {
		if(sex == "female") {
			System.out.println("My sex is " + sex + " and I'm a feminist");
		}
		
		else {
			System.out.println("yuh, brudda. I am a " + sex);
		}
	}
}
public class Application {
	public static void main(String[] args) {
		
	Person person1 = new Person(); 
	
	person1.name = "Karen White"; 
	person1.age = 43; 
	person1.sex = "female"; 
	person1.speak();
	person1.gender(); 
	
	Person person2 = new Person(); 
	 
	person2.name = "Chad Bigboi"; 
	person2.age = 19; 
	person2.sex = "male"; 
	person2.speak();
	person2.gender(); 
	}
}
```
