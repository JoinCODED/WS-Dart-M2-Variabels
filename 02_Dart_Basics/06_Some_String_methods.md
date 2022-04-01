We will keep learning about `string`s and in this lesson I'll show you some cool methods that you can apply on your strings.

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

As you can see, the `.toUpperCase()` method turns our string to all uppercase letters!

Oh, We forgot to explain what a method is.. 🙄

You can think of methods as operations that perform some logic on a givin variable or an object.

So we have `myCountry` variable and we can call a method on it by adding a `.`.


Yeah you guessed it, we also have a `.toLowerCase()` ⏬ method that does the opposite:

```dart
    print(myCountry.toLowerCase());
```

Output:

```
kuwait
```

The next method we will learn is the `.contains()` method, and as the name suggests, it checks for us if a string contain a certain character or a series of characters and return to us the result as a boolean, `true` or `false`.

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

For our next method lets modify out string a bit:

```dart
   String myCountry = 'I live in Kuwait';
```

The method is `.replaceAll()`, but this time, this method needs two arguments, the string you wanna replace and the replacement, and we separate arguments like i did in this sentence, i used a lot of commas `,`.

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

Are we done with string methods? no, there's a lot more that you can do with strings, and you can find them here:

💡 [Docs](https://api.dart.dev/stable/2.16.1/dart-core/String-class.html)
