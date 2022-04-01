One big distinction between programming languages, is if they are statically typed or dynamically typed languages.

Some examples for statically typed languages are Java, Swift, and our beloved dart, while for example JavaScript and python are dynamically typed languages, but what does all that means?

Static: types are checked at compile time

Dynamic: types are checked during execution

And that means that any type error can be caught before execution in dart, not while our program is running, let's take and example:

```dart
void main() {
String name = "Laila";
print(name.toUpperCase());
}
```

If we try to change the `name` type to int:

```dart
void main() {
int name = "Laila";
print(name.toUpperCase());
}
```

As soon as we did that, dart tells us that you can't assign the string `Laila` to an int type variable `name` before we even run our code.

And once you assign a variable with a type, you can't reassign it a different type, for example:

```dart
void main() {
int name = "Laila";
name = 5;
print(name.toUpperCase());
```

the conclusion is, Dart enforces guarantees about variable types, and it does it at compile time, and won't let us run our program. And that's for our advantage as it helps us discover type-related bugs at compile time, makes our code more readable, more maintainable code and also more efficient code performance after compile.
