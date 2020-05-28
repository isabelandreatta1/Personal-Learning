
### String Methods

For concatenation 

| Method | String1 | String2| Result | Notes 
| ------------- | ------------- | ------------- | ------------- | ------------- | 
| .subString(startPos, endPos)  | String s1 = "Hello my name is"; |String s2 = s1.substring(0,5); | Hello | Includes puncuation and spaces, default starts from 0 | 
| .length | String s1 = "Hello my name is";  | int s2 = s1.length; | 5 | Includes puncuation and spaces | 
| .toUpperCase | String s1 = "Hello my name is"; | String s2 = s1.toUpperCase(); | HELLO MY NAME IS | Remember brackets at end| 
| .toLowerCase | String s1 = "Hello my name is"; | String s2 = s1.toLowerCase(); | hello my name is |  Remember brackets at end| 
| .indexOf(String) | String s1 = "Hello my name is"; | int s2 = s1.indexOf('m'); | 5 | Includes puncuation and spaces, both chars and words (e.g. s1.indexOf("name"), default starts at 0,  to change default --> indexOf(String,pos) |
| .compareTo(String | String s1 = "Hello my name is"; String 2 = "Hello my name is Isabel" | int var = s1.compareTo(s2); | -6 | Compared the number of characters. If they are the same = 0, number is positive = larger than by, number is negative = smaller than by | 
| .equals(String) | String s1 = "Hello my name is"; String 2 = "Hello my name is not"; | s1.equals(s2); | False | This is case sensitive. There is the alternative .equalsIgnoreCase which is not case sensitive | 
