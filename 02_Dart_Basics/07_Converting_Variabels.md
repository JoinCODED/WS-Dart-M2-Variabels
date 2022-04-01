In this lesson we will learn how to convert variables types.

Let's start with this main method:

```dart
void main() {
int attendance = 200;
}
```

You have learned a lot of string methods, let's try to apply the `replaceAll` method to replace all zeros to ones:

```dart
void main() {
int attendance = 200;
print(attendance.replaceAll('0','1'));
}
```

Oops, dart is complaining, we can't apply a string method to an integer 😥, let's convert this variable to a string:

```dart
void main() {
int attendance = 200;
attendance = attendance.toString();
print(attendance.replaceAll('0','1'));
}
```

The `.toString()` method turns an integer to a string, but we can't assign the result to the variable `attendance`, why 🤔?

Because we converted `200` to a `string` we can't assign it to a variable with the type `int`, so we have to create a new variable of type `string` and assign it to it:

```dart
void main() {
int attendance = 200;
String attendanceAsString = attendance.toString();
print(attendance.replaceAll('0','1'));
}
```

Then, apply the `.replaceAll()` method on the new variable we just created:

```dart
void main() {
int attendance = 200;
String attendanceAsString = attendance.toString();
print(attendanceAsString.replaceAll('0','1'));
}
```

Output:

```
211
```

We can do this in a shorter way, which is called chaining 🔗 methods, calling a method after a method after a method etc:

```dart
void main() {
int attendance = 200;
print(attendance.toString().replaceAll('0','1'));
}
```

There's also a `toInt` and `toDouble` methods that works the same way, for example:

```dart
void main() {
double height = 1.78;
print(height.toInt());
}
```

Output:

```
1
```

But for strings, not all strings can be converted to a double or an integer, for example you can't:

```dart
"hello".toDouble();
```

For dart to be able to check a string if it can be converted or not, we use `parsing` in a such way:

```dart
double.parse("hello");
```

If it can be converted to a double dart will do that for us, and if it's not, like the case above the output will be nothing.

```dart
double.parse("hello"); // outputs nothing
double.parse("17.2"); // outputs 17.2
```
