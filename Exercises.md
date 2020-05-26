## Print hello and your name on a separate lines

```javascript
import java.util.Scanner;

public class Application {
	public static void main(String[] args) {
		
		Scanner input = new Scanner(System.in); 
		
		System.out.println("Input your first name:");
		String text = input.next();
		System.out.println("Input your surname:");
		String text2 = input.next(); 
		
		System.out.println("Hello \n" + text + " "+ text2);
	
		}	
	}
```
## Four integers and tells you if they're equal
```javascript
import java.util.Scanner;

public class Application {
	public static void main(String[] args) {
		
		
		Scanner scanner = new Scanner(System.in);
		System.out.print("Input your first number");
		int num1 = scanner.nextInt(); 
		System.out.println("Input second number:");
		int num2 = scanner.nextInt();
		System.out.println("Input third number:");
		int num3 = scanner.nextInt(); 
		System.out.println("Input fourth number:");
		int num4 = scanner.nextInt();
			
		if(num1 == num2 && num2 == num3 && num3 == num4) {
			System.out.println("Numbers are equal");
		}
		
		else {
			System.out.println("Numbers are not equal");
		}
		
	}
}
```
## Simple Calculator 
```javascript
import java.util.Scanner;

public class App {
	public static void main(String[] args) {
		
		Scanner scanner = new Scanner(System.in); 

		System.out.println("Input first number:");
		double num1 = scanner.nextDouble(); 
		System.out.println("Input second number:");
		double num2 = scanner.nextDouble(); 
		
		System.out.println("Input calculation:");
		String text = scanner.next(); 
		System.out.println(text);
		
		switch(text) {
		
		case "addition":
			System.out.println(num1 + num2);
			break; 
		
		case "subtraction":
			System.out.println(num1 - num2);
			break; 
			
		case "division":
			System.out.println(num1/num2);
			break; 
		
		case "multiplication":
			System.out.println(num1 * num2);
			break; 	
		}
	}
}
```
## Tell if a number is odd or even
```javascript
import java.util.Scanner;
public class App {
	public static void main(String[] args) {
		Scanner input = new Scanner(System.in);
		
		System.out.println("Input number");
		int num = input.nextInt(); 
		
		//% is for modulus 
		if((num %2) == 0){
			System.out.println("It is an even number");
		}
		else {
			System.out.println("It is an odd number");
		}	
	}
}
``` 
