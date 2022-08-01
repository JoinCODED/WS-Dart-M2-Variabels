Remove the `print` statement that we added in the previous lesson:

```dart
void main() {

}
```

Type the following code in your `main` method:

```dart
void main() {
    String name = 'Salem';
    print(name);
}
```

Run your code, as you can see, it prints the name `Salem`.

How did the code work? We told it to print `name` but instead, we got `Salem`!

The idea here is that `name` is a variable that `contains` the value `Salem`. Imagine it as a box 📦 labeled with `name` 🏷️, and in that box there's a paper 📜 with `Salem` on it. We refer to that box with its label whenever we want to read or look at`Salem`

![box](https://user-images.githubusercontent.com/84308096/157937649-0bebc386-c99f-406b-8c6f-2648d6d55d81.jpg)

Behind the scenes, Dart allocates some space in the memory and stores `Salem` in it. To refer to that value, we assigned a reference to that location in the memory and we called it `name`.

Let's digest the line we have written:

![diagram](https://user-images.githubusercontent.com/84308096/157944541-83c1ab96-7d3b-4402-83f4-7a43d9776299.png)

When we declare a variable, we have to give it a `type`, and in our case, it's a `String` because it represents alphabetical letters (Don't worry we will talk about types later).
Then, we need to give it a name, which in our case is `name`.
We initialize our variable by assigning it a value `Salem`.
Finally, we added a semi-colon `;` to tell Dart that we finished.

What's the difference between `declaring` and `initializing` a variable? 🤔

`declaration` is the process of defining a variable and giving it a name in order to be able to refer to it later.
While `initialization` is the process of assigning an initial value to that variable.

There are some rules for naming variables:

1. Can be a combination of lowerCase and UpperCase letters as well as all digits from 0 to 9 and the `_` character.
2. The first character of a variable name can't be a digit.
3. Should follow the `camelCase` naming convention, which means you should always use lowercase letters and the first letter of each word (except the first word) is capitalized.

### Challenge 👾: Can you spot a variable that follows our naming rules?

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
