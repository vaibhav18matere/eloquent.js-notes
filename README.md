# INTRODUCTION

1. programming is dynamic in nature and it cannot be managed using methods like best practices. Practice makes a good program
2. language adds structure to a program. It makes the program understandable and actionable to a developer
3. JavaScript was developed by Brendan Eich in 1995 to program web pages in Netscape Navigator
4. ECMAScript standard is the Universal standard for JavaScript
5. ECMAScript and JavaScript can be used interchangeably—they are two names for the same language.
6. typographic conventions - the monospace font is used for code snippets

# VALUES , TYPES AND OPERATORS

- console.log("Aardvark" < "Zoroaster")
 → true

- "Z" < "a"
→  true 

- uppercase letters are always “less” than lowercase ones

- console.log(NaN == NaN)
 → false

- NaN is supposed to denote the result of a nonsensical computation, and as such, it isn’t equal to the result of any other nonsensical computations.

- console.log(true && false)
// → false

- console.log(true && true)
// → true

- console.log(false || true)
// → true

- console.log(false || false)
// → false

- console.log(8 * null)
// → 0

- null  becomes 0

- console.log("5" - 1)
// → 4

- "5" becomes 5 (from string to number)

- console.log("5" + 1)
// → 51

- + tries string concatenation before numeric addition, so the 1 is converted to "1"
- if any one is String then it just concat

- console.log("five" * 2)
// → NaN

- When something that doesn’t map to a number in an obvious way (such as "five" or undefined) is converted to a number, you get the value NaN.

- console.log(false == 0)
// → true

- console.log(null == undefined);
// → true

- console.log(null == 0);
// → false

- console.log(null || "user")
// → user

- console.log("Agnes" || "user")
// → Agnes

- var a = 100;
var b = true;
a+b;
→ 101

- true+true
2

- num = 16;
num2= null;
num+num2;
16

- Operator return the value to its left when that can be converted to true and will return the value on its right otherwise

# PROGRAM STRUCTURE

- Expressions and statements :

1. Expression ⇒ A fragment of code that produces a value ⇒ ex.  18,    "Vaibhav";

2. Statement ⇒ A full sentence ex. var name = "Vaibhav";

- Variable / ( Binding ) ⇒ Container , to keep the value (var in above example)

1. can contain digits ex. var myFav5things = "abcde" ; ✅
    
    but can't start with digits ex var 5favThings = "abcde"; ❌ 
    
2. No punctuations except dollar signs ( $ ) and  underscore ( _ ) :  
    
    ex. var me$my_javascriptNotes = "abcd";
    
3. Also don't use reserved keywords for variable name 

```
break case catch class const continue debugger default
delete do else enum export extends false finally for
function if implements import interface in instanceof let
new package private protected public return static super
switch this throw true try typeof var void while with yield
```

1. We can change variables dynamically. (It's allowed)
    
    var name = " Vaibhav";
    var name = "Matere";
    
Excercise 1 : Star pattern (one star at first linehttps://amusing-freon-21f.notion.site/Values-Types-Operators-1-05baad4e34c84398b33b5d844536458d , 2 at second and so on)
[Solution](https://replit.com/@Vaibhav18Matere/star-pattern-do-while-loop)

# Function
- Function declarations are not part of the regular top-to-bottom flow of control.
    - Code works, even though the function is defined *below* the code that uses it
    
    ```jsx
    console.log("The future says:", future());
    function future() {
    
         return "You'll never have flying cars";
    }
    ```
    

**Arrow functions  ⇒** 

It expresses something like “this input (the parameters) produces this result (the body)”

- When there is only one parameter name, you can omit the parentheses around the parameter list.

```jsx
const square1 = (x) => { return x * x; };
const square2 = x => x * x;
```

JavaScript is extremely broad-minded about the number of arguments you pass to a function. If you pass too many, the extra ones are ignored. If you pass too few, the missing parameters get assigned the value `undefined`.

- **The call stack ⇒**
- **Optional Arguments ⇒**
- **Closure ⇒**

A function that calls itself is called *recursive*.

- **Growing functions ⇒**

**Give short and meaningful name to the function**
