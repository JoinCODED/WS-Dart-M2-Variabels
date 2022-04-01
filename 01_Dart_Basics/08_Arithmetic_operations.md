In this lesson you will learn about operators in dart.

We can perform all types of arithmetic operations with dart, for example:

```dart
print(5 + 2);
print(5 - 2);
print(5 * 2);
print(5 / 2);
```

Output:

```
7
3
10
2.5
```

We also have augmented operators that works in this way:

```dart
void main() {
int x = 5;
x = x + 2;
print(x);
}
```

To make it shorter we use augmented operators:

```dart
void main() {
int x = 5;
x += 2;
print(x);
}
```

And this will work with `+`,`-`,`*`,`/`.

It's worth to notice that dart unlike us, is good at math, and it will follow the rules of math, for example:

```dart
print(6-3*2);
```

Output:

```
0
```

Dart will do the multiplication first, then evaluate the remaining. If we want dart to do the subtraction first we use parenthesis:

```dart
print((6-3)*2);
```

Output:

```
6
```

### Logical operators:

We can also do all logical operators such as:

1. `==` equal,
2. `!=` does not equal,
3. `>=` bigger than or equal,
4. `>` bigger than,
5. `<` less than,
6. `<=` less than or equal

For example:

```dart
void main(){
    int x = 7;
    int y = 5;

print(x==y); // false
print(x!=y); // true
print(x>=y); // true
print(x>y); // true
print(x<y); // false
print(x<=y); // false
}
```

But some times, you need to compare multiple expressions in one go, and for that you use `&&` and `||` logical operators:

```dart
void main(){
    int x = 7;
    int y = 5;
print(x > y && x < 10 ); // true
print(x > y && x < 4 ); // false
print(x > y || x < 4 ); // true
}
```

For the `&&` aka `And` operator, both conditions should evaluate to true so it can consider it as true:

```dart
print(x > y && x < 10 ); // true
```

Will be evaluated to:

```dart
print(true && true ); // true
```

But for:

```dart
print(x > y && x < 4 ); // true
```

Will be evaluated to:

```dart
print(true && false ); // false
```

For the `||` aka `OR` operator only one of the conditions should evaluate to true to be considered as true by dart:

```dart
print(x > y || x < 4 ); // true
```

Will be evaluated to:

```dart
print(true || false ); // true
```
