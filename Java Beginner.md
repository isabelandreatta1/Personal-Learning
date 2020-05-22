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
