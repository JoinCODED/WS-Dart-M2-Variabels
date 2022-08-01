To understand what type interference is, define 3 variables with types: String, int, and double:

```dart
void main() {
    String name="Mohammad";
    int age= 60;
    double height = 1.84;
}
```

As we learned in the previous lesson, Dart is a statically typed language, and it can infer the type of variables that we declared.

Our first term to learn is `var` which stands for `variable` and we can declare variables using the following keyword:

```dart
void main() {
    var name="Mohammad";
    var age= 60;
    var height = 1.84;
}
```

Notice that we can run our code with no problems, that's because Dart can `infer` the type alone. For example, Dart knows that `name` is of type `String` because it was initialized with a string `Mohammad`. This also applies to the other variables, `age` and `height`.

Can we trust Dart? let's try to assign a string to the variable `age`:

```dart
void main() {
    var name="Mohammad";
    var age= 60;
    age = "young";
    var height = 1.84;
}
```

As you can see, Dart tells us that we can't assign a string to a variable of type int.
