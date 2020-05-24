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
