We will keep learning about `string`s. In this lesson I'll show you some cool methods that you can apply to your strings.

Let's start by defining a string:

```dart
void main() {
    String myCountry = 'Kuwait';
    print(myCountry);
}
```

The first method we will learn is the `.toUpperCase()` ⏫ method:

```dart
void main() {
    String myCountry = 'Kuwait';
    print(myCountry.toUpperCase());
}
```

Output:

```
KUWAIT
```

As you can see, the `.toUpperCase()` method turns our string into uppercase letters!

Oh, We forgot to explain what a method is.. 🙄

Methods are a collection of statements that perform some operations on a givin variable or an object.

So we have `myCountry` variable, and we can apply a certain method to it by adding a period `.`.

Yeah, you guessed it. We also have a `.toLowerCase()` ⏬ method that does the opposite:

```dart
    print(myCountry.toLowerCase());
```

Output:

```
kuwait
```

The next method we will learn is the `.contains()` method. As the name suggests, it checks if a string contains a certain character or a series of characters and returns to us the result as a boolean: `true` or `false`.

```dart
void main() {
    String myCountry = 'Kuwait';
    print(myCountry.contains('wa'));
    print(myCountry.contains('s'));
}
```

Output:

```
true
false
```

Let's modify our string a bit for the next method:

```dart
   String myCountry = 'I live in Kuwait';
```

The next method is `.replaceAll()`. This time, it needs two arguments, the string you want to replace with and the replacement, and we separate those arguments with a comma `,`, like the following sentence:

```dart
void main() {
    String myCountry = 'I live in Kuwait';
    print(myCountry.replaceAll('Kuwait','Oman'));
}
```

Output:

```
I live in Oman
```

Are we done with string methods? No, there is a lot more that you can do with strings. You can check the [docs](https://api.dart.dev/stable/2.16.1/dart-core/String-class.html).
