# Java Lambda Expressions
Lambda Expression is a short block of code which takes in parameters and returns a value. Lamda expressions are similar to methods, but they do not need a name and can be implemented right in the body of a method

## Syntax
```
parameter -> expression
```

```
param1, param2, param3) -> expression
```

- `expressions` are limited. 
- They have to immediately return a value, and cannot contains variables, assignments or statements such as `if` or `for`
- In order to do a more complex operation, a code block can be used with `{}`

```
(param1, param2) -> { code block}
```

### Example:
1. Use a lambda expression in the `ArrayList's forEach()` method:
```java
import java.util.ArrayList;
public class Main {
  public static void main (String[] args) {
    ArrayList<Integer> numbers = new ArrayList<Integer>();
      numbers.add(5);
      numbers.add(9);
      numbers.add(8);
      numbers.forEach((n) -> {System.out.println(n);});
  }
}

```
