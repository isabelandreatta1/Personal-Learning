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
