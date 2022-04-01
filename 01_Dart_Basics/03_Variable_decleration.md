Start by removing the `print` statement we added in the previous lesson:

```dart
void main() {

}
```

Type this code in your `main` method:

```dart
void main() {
    String name = 'Salem';
    print(name);
}
```

Run your code, As you can see, it printed the name `Salem`.

But how does this code works? we told it to print `name` but instead we got `Salem`!

The idea here is that `name` is a variable that `contains` the value `Salem`. Imagine it as a box 📦 labeled as `name` 🏷️ and in that box there's a paper 📜 with `Salem` on it, and whenever we want to look or read `Salem` we refer to that box with its label.

![box](https://user-images.githubusercontent.com/84308096/157937649-0bebc386-c99f-406b-8c6f-2648d6d55d81.jpg)

Behind the scenes, Dart allocates some space in memory and stores `Salem` in it, and to refer to that value, we assigned a reference to that location in memory and we called it `name`.

Let's digest the line we have written:

![diagram](https://user-images.githubusercontent.com/84308096/157944541-83c1ab96-7d3b-4402-83f4-7a43d9776299.png)

When we declare a variable, we need to give it a `type` and in this case it's a `String` because it represents alphabetical letters (Don't worry we will talk about types later).
Then we need to give it a name, and in this case we named it `name`.
Then we initialize our variable by assigning `=` it a value `Salem`.
Finally to tell dart that we finished we add a terminator `;`.

But what's the difference between Variable `declaration` and `initialization`? 🤔

`declaration` is the process of defining a variable and giving it a name so we can refer it later.
`initialization` is the process of assigning an initial value to that variable.

Variable names has some rules we need to follow ☝️: 

1. Can be a combination of lowerCase and UpperCase letters as well as all digits from 0-9 and the `_` character.
2. The first character of variable name cannot be a digit.
3. Should follow the `camelCase` naming convention and this means you should always use lowercase letters and for each word after the first word starts with an upperCase letter.

### Challenge 👾: Can you spot the variable that follows our naming rules?

```
String VariableName;
String variableName;
String 9variableName;
String variablename;
```

### Solution 💡: 

```
String VariableName; ❌
String variableName; ✅
String 9variableName; ❌
String variablename; ❌
```

