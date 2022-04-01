In the previous lesson we declared a lot of variables, let's print them out:

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

Lets remove all our print statements and replace them with only one:

```dart
void main() {
    String name = 'Salem';
    int age = 24;
    double height = 178.2;
    bool lovesCoding = true;
    print("My name is");
}
```

Now we need to inject 💉 our variable in here, lets try this:

```dart
void main() {
    String name = 'Salem';
    int age = 24;
    double height = 1.78;
    bool lovesCoding = true;
    print("My name is name");
}
```

So.. did it work 😶‍🌫️? nope, dart thinks `name` is a string, how can we tell it that's a variable?

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

This one is much nicer, let's see how this works:

```dart
void main() {
    String name = 'Salem';
    int age = 24;
    double height = 178.2;
    bool lovesCoding = true;
    print("My name is $name");
}
```

We just have to add a `$` sign before the variable and dart will know that this is a variable!

And we can do the same for the rest of our sentence:

```dart
void main() {
    String name = 'Salem';
    int age = 24;
    double height = 178.2;
    bool lovesCoding = true;
    print("My name is $name, I'm $age years old, I'm $height meters tall, and do I love coding? thats $lovesCoding!");
}
```

But what if i want to print my age + 1, as an arithmetic (we will talk about it later).

```dart
print("My $age + 1");
```

hmm, dart thinks that `+ 1` is a string, to solve this we can:

```dart
print("My ${age + 1});
```

by surrounding `age + 1` in curly braces we are telling dart that this is an expression that needs to be computed, not a string.
