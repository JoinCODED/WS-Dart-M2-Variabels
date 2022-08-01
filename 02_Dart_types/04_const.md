There is another keyword in Dart that is more restrictive than `final` which is `const`.

`const` defines a `compile-time` constant.

Let's try to use `const` in this block of code:

```dart
void main() {
    const String name = "laila";
    String nameUpperCased = name.toUpperCase();
    print(nameUpperCased);
}
```

`const` stands for `constant`, which means that the value is constant and does not need to be computed, let's take some examples:

```dart
var name = "laila"; // this is a constant value
var sum = 5 + 7; // the computer needs to compute this expression and sum 5 + 7 to give us 12, so this is not a constant value
var nameUpperCased = name.toUpperCase(); // this is also needs to be computed and the computer is doing something on the `name` and making it upperCase, so this is not a constant
var age = 50; // this is a constant
var laila = name; // this is a constant
```

To summarize what we learned so far:

`var`: can be reassigned multiple times.

`final`: can be set only once.

`const`: for compile time constants.

You should prefer `const`>`final`>`var`.
