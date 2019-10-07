# Style Guidelines
When submitting PRs to Fabric Community projects, we ask that you format your projects with our style guides in mind. We do this so:
  - new code readers don't have difficulty reading our code
  - we don't change styles on a per-PR basis
  - time isn't wasted on reviews talking about style fixes
  
Our style is based off:
  - Fabric API
  - [Google Guidelines] (https://google.github.io/styleguide/javaguide.html)

When in doubt, search the google page. A brief rundown includes:

### Braces
Braces should begin on the same line as a conditional or block start, and end on a new line.
```java
if (myCondition) {
   myMethod();
}
```

### Separating Blocks
Keep a newline between each block on each level of indentation.
```java
if (myCondition) {
   myMethod();
}

if (mySeparateCondition) {
   myMethod();
}
```

When doing if-else statements, keep the `else` start at the end of the `if` closing brace:
```java
if (myCondition) {
   myMethod();
} else (mySeparateCondition) {
   myMethod();
}
```

### State Validation
When checking the state of a parameter passed into a method, leave a newline at the end.
```java
public void myMethod(MyObject obj) {
   assert (obj not null) [...]
 
   if(obj.getProperty()) [...]
```

### Identifiers
When registering content that has a two+ word name, connect the words with an underscore.
`Deadly Pickaxe` -> `deadly_pickaxe`

### Parameter Names
Method parameters in Fabric often have `_1` added on the end. Try to clean these up when possible.

### Method Naming
Method names should be descriptive and concise. This also applies to mixin methods.

### Tabs and Spaces
Use either 4 spaces or 1 tab when indenting a line.

### Trailing Whitespace
Please do not add whitespace between the following:
- Two braces with no content between them.
- Before the bottom or top braces of a class.
