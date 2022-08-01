One big distinction between programming languages is if they are statically typed or dynamically typed languages.

Some examples of statically typed languages are Java, Swift, and our beloved Dart, while for example JavaScript and Python are dynamically typed languages, but what does all that mean?

Static: types are checked at compile time.

Dynamic: types are checked during execution.

And that means any type of error can be caught before execution in Dart, not while our program is running, let's take an example:

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

As soon as we do that, Dart tells us that you can't assign the string `Laila` to an int type variable `name` before we even run our code.

And once you assign a variable with a type, you can't reassign it a different type. For example:

```dart
void main() {
int name = "Laila";
name = 5;
print(name.toUpperCase());
}
```

To sum up, Dart enforces guarantees about variable types, does that at compile-time, and won't let us run our program. That's for our advantage as it helps us discover type-related bugs at compile time, makes our code more readable and more maintainable, and ensures a more efficient code performance after compilation.
