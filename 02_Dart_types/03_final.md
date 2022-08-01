No, that's not the `final` lesson, it's the `final` keyword.

Sometimes, we want to declare and initialize a variable, and never change its value later. In simpler words, we want a variable to be `final` or `read-only`, hence we can use the `final` keyword.

```dart
void main() {
    var name="Mohammad";
    final age = 60;
    age = "young";
    var height = 1.84;
}
```

Here, we are telling Dart that the value of `age` is final, and can't be reassigned. That's why we have an error in the code above.

Maybe you are not convinced to use final, but once you start working on big projects, you will start to appreciate the `final` keyword as it shows us that this variable is meant to be `read-only` and saves us from catching weird bugs.

So prefer `final` over `var` whenever you could, and that's final!

You can still explicitly tell Dart the variable type and set it as `final`:

```dart
void main() {
    final String name="Mohammad";
    final int age = 60;
    var height = 1.84;
}
```
