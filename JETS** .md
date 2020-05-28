
# Important for IB JETS (Java Examination Tool Subset) 

## Operators 


| Type  | Operator | Description | Code | Result |
| ------------- | ------------- |------------- |------------- |------------- |
| Arithmetic  | + | Addition |  21 + 9 | 30 | 
| Arithmetic  | - | Subtraction | 30 - 9 | 21 | 
| Arithmetic  | * | Multiplication | 3 * 7 | 21 | 
| Arithmetic | / | Division| 21 / 3 | 7 | 
| Arithmetic | % | Modulus| 21%4 | 1 |  
| Relational | == | equal to | 3 == 4 | False | 
| Relational  | > | greater than | 3 > 4 | False | 
| Relational |  >= | greater or equal to| 4 >= 4 | True | 
| Relational  | <= | lesser or equal to | 4 <=5 | True | 
| Relational  | <= | lesser or equal to | 4 <=5 | True | 
| Relational  | != | not equal to| 4!=5 | True | 
| Content Cell  | ! | Logical NOT (opposite of Logical OR)| boolean a = true; boolean b = false; !(a && b)| True | 
| Content Cell  | && | Logical AND| boolean a = true ; boolean b = false; (a && b) | False | 
| Content Cell  | *two vertical lines* | Logical OR| boolean a = true; boolean b = false; (a *two vertical lines* b)| True | 


## String Methods

| Method | String1 | String2| Result | Notes 
| ------------- | ------------- | ------------- | ------------- | ------------- | 
| + | String s1 = "Hello"; String s2 = "my name is"; | System.out.println(s1 + s2); | Hello my name is"; | | 
| .subString(startPos, endPos)  | String s1 = "Hello my name is"; |String s2 = s1.substring(0,5); | Hello | Includes puncuation and spaces, default starts from 0 | 
| .length | String s1 = "Hello my name is";  | int s2 = s1.length; | 5 | Includes puncuation and spaces | 
| .toUpperCase | String s1 = "Hello my name is"; | String s2 = s1.toUpperCase(); | HELLO MY NAME IS | Remember brackets at end| 
| .toLowerCase | String s1 = "Hello my name is"; | String s2 = s1.toLowerCase(); | hello my name is |  Remember brackets at end| 
| .indexOf(String) | String s1 = "Hello my name is"; | int s2 = s1.indexOf('m'); | 5 | Includes puncuation and spaces, both chars and words (e.g. s1.indexOf("name"), default starts at 0,  to change default --> indexOf(String,pos) |
| .compareTo(String | String s1 = "Hello my name is"; String 2 = "Hello my name is Isabel" | int var = s1.compareTo(s2); | -6 | Compared the number of characters. If they are the same = 0, number is positive = larger than by, number is negative = smaller than by | 
| .equals(String) | String s1 = "Hello my name is"; String 2 = "Hello my name is not"; | s1.equals(s2); | False | This is case sensitive. There is the alternative .equalsIgnoreCase which is not case sensitive | 
