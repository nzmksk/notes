## Go Constants
- Used to declare variables with a fixed value that cannot be changed (read-only variables).
```go
// Typed constant
const user string = "John Doe"

// Untyped constant
const PI = 3.142

// Declaring multiple constants
const (
    A int = 1
    B = 3.14
    C = "Hi!"
)
```

### Notes
- A constant must be declared with a value.
- Type of constant is inferred from the value if it's untyped constant.
- Constants can be declared inside and outside functions.

<br />
<hr />

| Previous | Home | Next |
| :---: | :---: | :---: |
| [Variables](03-variables.md) | [Go Introduction](01-introduction.md) | [Output](05-output.md) |