To understand what type interference is, define 3 variables with the types that we learned:

```dart
void main() {
    String name="Mohammad";
    int age= 60;
    double height = 1.84;
}
```

And as we learned in the previous lesson, dart is statically typed languages, and dart can infer the type of variables that we declared.

Our first term to learn is `var` which stand for `varaible` and we can declare variables using this keyword:

```dart
void main() {
    var name="Mohammad";
    var age= 60;
    var height = 1.84;
}
```

Notice that we can run our code with no problems, that's because dart can `infer` the type alone, for example, dart knows that `name` is of type `String` because it was initialized with a string `Mohammad` and this also applies on the other variables `age` and `height`.

Can we trust dart? let's try to assign a string to the variable `age`:

```dart
void main() {
    var name="Mohammad";
    var age= 60;
    age = "young";
    var height = 1.84;
}
```

As you see, dart tells us that we can't assign a string to a variable of type int.
