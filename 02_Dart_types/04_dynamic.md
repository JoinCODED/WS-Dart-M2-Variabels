There's one more keyword, which is `dynamic`. This keyword allows us to escape the type safety.

```dart
void main () {
    var name = "laila";
    name = 56;
}
```

As we learned, this code will lead to an error, let's change `var` with `dynamic` and see what happens:

```dart
void main() {
    dynamic name = "laila";
    name = 56;
}
```

Did we just break Dart? No, this is what `dynamic` does, it's like telling Dart: hey, I know what I'm doing, I don't need your type safety. However, this is not a good idea as we benefit more of the type system in Dart than being lazy not declaring types, but sometimes when parsing `json` data, which we will learn later, we could benefit from the `dynamic` keyword.
