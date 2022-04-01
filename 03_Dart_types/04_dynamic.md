There's one more keyword, `dynamic` and this keyword let's us escape the type safety.

```dart
void main () {
    var name = "laila";
    name = 56;
}
```

As we learned this code will lead to an error, let's change `var` with `dynamic` and see what happens:

```dart
void main() {
    dynamic name = "laila";
    name = 56;
}
```

Did we just broke dart? no, this is what `dynamic` do, it's like telling dart: hey, i know what i'm doing, i don't need your type safety. However, this is not a good idea as we benefit more of the type system in dart than being lazy not declaring types, but sometimes when parsing `json` data which we will learn later, we could benefit from the `dynamic` keyword.
