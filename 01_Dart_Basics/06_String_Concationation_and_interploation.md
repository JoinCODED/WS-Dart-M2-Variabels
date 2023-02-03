In the previous lesson, we declared a lot of variables, let's print them out:

```dart
void main() {
    String name = 'Salem';
    int age = 24;
    double height = 1.78;
    bool lovesCoding = true;
    print(name);
    print(age);
    print(height);
    print(lovesCoding);
}
```

Wouldn't it be nice if we can join those variables into a single `string` and `print` them all in one `print` statement?

We want to achieve this output:

```
My name is Salem, I'm 24 years old, I'm 1.78 meters tall, and do I love coding? thats true!
```

Let's replace all of our `print` statements with one only:

```dart
void main() {
    String name = 'Salem';
    int age = 24;
    double height = 178.2;
    bool lovesCoding = true;
    print("My name is");
}
```

Now, we need to inject our variable in here, let's try the following:

```dart
void main() {
    String name = 'Salem';
    int age = 24;
    double height = 1.78;
    bool lovesCoding = true;
    print("My name is name");
}
```

So... Did it work? nope, Dart thinks `name` is a string. How can we tell it that's it's a variable?

There are two ways:

### String concatenation:

To concatenate two strings you can use the `+` sign like this:

```dart
void main() {
    String name = 'Salem';
    int age = 24;
    double height = 178.2;
    bool lovesCoding = true;
    print("My name is " + name);
}
```

### String interpolation:

This one is much nicer, let's see how it works:

```dart
void main() {
    String name = 'Salem';
    int age = 24;
    double height = 178.2;
    bool lovesCoding = true;
    print("My name is $name");
}
```

We have to add a `$` sign before the variable and Dart will know that this is a variable.

We can do the same for the rest of our variables:

```dart
void main() {
    String name = 'Salem';
    int age = 24;
    double height = 178.2;
    bool lovesCoding = true;
    print("My name is $name, I'm $age years old, I'm $height meters tall, and do I love coding? thats $lovesCoding!");
}
```

But what if I want to print my age + 1 as an arithmetic? (we will talk about it later).

```dart
print("My $age + 1");
```

Hmm, Dart thinks that `+ 1` is a string. To fix the issue, we can use curly braces:

```dart
print("My ${age + 1});
```

By surrounding `age + 1` in curly braces, we are telling Dart that this is an expression that needs to be computed, this is not a string.
