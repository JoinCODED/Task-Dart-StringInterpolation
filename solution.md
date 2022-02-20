1. In your main function we have the following variables:

```dart
void main() {
double temperature = 20;
String juice = 'juice';
String flavor = 'orange';
}
```

2. Let's print the first variable `temperature`:

```dart
void main() {
double temperature = 20;
String juice = 'juice';
String flavor = 'orange';

print("The temperature is C");
}
```

3. As you learned you have 2 ways of interpolating strings, let's try them both:

```dart
print("The temperature is $temperatureC");
```

Using only the dollar sign to inject the variable will cause the compiler to get confused and think that `temperatureC` is a whole word and will look for a variable with this name.

The solution is to use curly braces `{}`:

```dart
print("The temperature is ${temperature}C");
```

4. Let's print our second statement:

```dart
void main() {
double temperature = 20;
String juice = 'juice';
String flavor = 'orange';

print("The temperature is ${temperature}C");
print("I like $flavor $juice.");
}
```

### 🍋 Arithmetic spice

1. Create a variable named `number` of type `int`:

```dart
void main() {
double temperature = 20;
String juice = 'juice';
String flavor = 'orange';
int number = 5;

print("The temperature is ${temperature}C");
print("I like $flavor $juice.");
}
```

2. Print this variable:

```dart
void main() {
double temperature = 20;
String juice = 'juice';
String flavor = 'orange';
int number = 5;

print("The temperature is ${temperature}C");
print("I like $flavor $juice.");
print("$number plus $number makes $number + $number");
}
```

But the output would be:

```
5 plus 5 makes 5 + 5
```

To have an `expression` in a string we also have to use the curly braces `{}` as everything in those curly braces will be evaluated as dart `expression`.

```dart
void main() {
double temperature = 20;
String juice = 'juice';
String flavor = 'orange';
int number = 5;

print("The temperature is ${temperature}C");
print("I like $flavor $juice.");
print("$number plus $number makes ${number + number}");
}
```
