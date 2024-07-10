## Go Syntax
Consists of the following parts:
- package declaration
- import packages
- functions
- statements and expressions

Example:
```go
package main
import ("fmt")

func main() {
    fmt.Println("Hello World!")
}
```
- Every program is part of a package. This is defined using the `package` keyword. In this example, the program belongs to the `main` package.
- `import ("fmt")` import files included in the `fmt` package.
- `func main() {}` is a Go function. Any code inside the curly brackets `{}` will be executed.
- `fmt.Println()` is a function made available from the `fmt` package. It is used to output/print text. In this example, the output will be "Hello World!".

### Go Comments
| Syntax | Description |
| --- | --- |
| // | Single-line comment. |
| /* */ | Multi-line comment. |

### Notes
- In Go, any executable code belongs to the `main` package.

<br />
<hr />

| Previous | Home | Next |
| :---: | :---: | :---: |
|  | [Go Introduction](01-introduction.md) | [Variables](03-variables.md) |
