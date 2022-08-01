In this lesson, we will learn how to convert variable types.

Let's start with the main method:

```dart
void main() {
int attendance = 200;
}
```

You have learned a lot of string methods, let's apply the `.replaceAll` method to replace all zeros to ones:

```dart
void main() {
int attendance = 200;
print(attendance.replaceAll('0','1'));
}
```

Oops, Dart is complaining. We can't apply a string method to an integer type 😥. Let's convert this variable to a string:

```dart
void main() {
int attendance = 200;
attendance = attendance.toString();
print(attendance.replaceAll('0','1'));
}
```

The `.toString()` method turns an integer into a string, but we can't assign the result to the variable `attendance` again, why 🤔?

Because we converted `200` to a `string`, and we can't assign it to a variable with the type `int`, so we have to create a new variable of type `string` and assign `attendance.toString()` to it:

```dart
void main() {
int attendance = 200;
String attendanceAsString = attendance.toString();
print(attendance.replaceAll('0','1'));
}
```

Then, apply the `.replaceAll()` method to the new variable we just created:

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

We can do this in a shorter way, which is called chaining 🔗 methods. It is a mechanism of calling a method on another method in a single line instead of calling other methods with the same object reference separately:

```dart
void main() {
int attendance = 200;
print(attendance.toString().replaceAll('0','1'));
}
```

There are also `toInt` and `toDouble` methods that work the same way, for example:

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

Not all strings can be converted to a double or an integer. For example, you can't covert the following string to a double:

```dart
"hello".toDouble();
```

For Dart, to be able to check if a string can be converted or not, we use `parsing` as follows:

```dart
double.parse("hello");
```

If it can be converted into a double, Dart will do that for us. If it can't, like the case above, the output will be nothing.

```dart
double.parse("hello"); // outputs nothing
double.parse("17.2"); // outputs 17.2
```
