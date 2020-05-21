**Types of variables**
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
		String myString = "I like to stroke cat's bellies in my spare time"; //uses "S" because is a class 

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
Most important variables for IB Java: 

1. String
2. Integer 
3. Double
4. Boolean
5. Char 

We want to make sure we are using the right variable for what it will contain. This is so our value will just fit in. Code does work if you use a variable that is larger, but it is a waste and we want faster programs. 


**Counting number of bears using for loop** 

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
