## Go Output Functions
| Function | Description |
| --- | --- |
| `Print()` | Print its arguments with their default format. |
| `Println()` | Similar to `Print()` but whitespace is added between the arguments, and a newline is added at the end. |
| `Printf()` | Format its argument based on the given formatting verb and print it. See [formatting verbs](#formatting-verbs). |

Examples:
```go
package main
import ("fmt")

func main() {
  var i,j string = "Hello","World"

  fmt.Print(i, j)
}

// Output: HelloWorld

func main() {
  var i,j = 10, 20

  fmt.Print(i, j)
}

/* Output: 10 20
Print() inserts a space between the arguments if neither are strings.
*/
```

```go
package main
import ("fmt")

func main() {
  var i,j string = "Hello","World"

  fmt.Println(i, j)
}

// Output: Hello World
```

```go
package main
import ("fmt")

func main() {
  var i string = "Hello"
  var j int = 15

  fmt.Printf("i has value: %v and type: %T\n", i, i)
  fmt.Printf("j has value: %v and type: %T", j, j)
}

/* Output:
i has value: Hello and type: string
j has value: 15 and type: int
*/
```

<hr />

### Formatting Verbs
#### General Formatting Verbs
| Verb | Description |
| --- | --- |
| `%v` | Print the value in the default format. |
| `%#v` | Print the value in Go-syntax format. |
| `%T` | Print the type of the variable. |
| `%%` | Print the % sign. |

```go
func main() {
  var i = 15.5
  var txt = "Hello World!"

  fmt.Printf("%v\n", i)
  fmt.Printf("%#v\n", i)
  fmt.Printf("%v%%\n", i)
  fmt.Printf("%T\n", i)

  fmt.Printf("%v\n", txt)
  fmt.Printf("%#v\n", txt)
  fmt.Printf("%T\n", txt)
}

/* Output:
15.5
15.5
15.5%
float64
Hello World!
"Hello World!"
string
*/
```

#### Integer Formatting Verbs
| Verb | Description |
| --- | --- |
| `%b` | Base 2. |
| `%d` | Base 10. |
| `%+d` | Base 10 and always show sign. |
| `%o` | Base 8. |
| `%O` | Base 8 with leading 0o. |
| `%x` | Base 16 lowercase. |
| `%X` | Base 16 uppercase. |
| `%#x` | Base 16 with leading 0x. |
| `%4d` | Pad with spaces - width 4, right justified. |
| `%-4d` | Pad with spaces - width 4, left justified. |
| `%04d` | Pad with zeroes - width 4. |

```go
package main
import ("fmt")

func main() {
  var i = 15
 
  fmt.Printf("%b\n", i)
  fmt.Printf("%d\n", i)
  fmt.Printf("%+d\n", i)
  fmt.Printf("%o\n", i)
  fmt.Printf("%O\n", i)
  fmt.Printf("%x\n", i)
  fmt.Printf("%X\n", i)
  fmt.Printf("%#x\n", i)
  fmt.Printf("%4d\n", i)
  fmt.Printf("%-4d\n", i)
  fmt.Printf("%04d\n", i)
}

/* Output:
1111
15
+15
17
0o17
f
F
0xf
  15
15
0015
*/
```

#### String Formatting Verbs
| Verb | Description |
| --- | --- |
| `%s` | Print the value as plain string. |
| `%q` | Print the value as double-quoted string. |
| `%8s` | Print the value as plain string - width 8, right justified. |
| `%-8s` | Print the value as plain string - width 8, left justified. |
| `%x` | Print the value as hex dump of byte values. |
| `% x` | Print the value as hex dump with spaces. |

```go
package main
import ("fmt")

func main() {
  var txt = "Hello"
 
  fmt.Printf("%s\n", txt)
  fmt.Printf("%q\n", txt)
  fmt.Printf("%8s\n", txt)
  fmt.Printf("%-8s\n", txt)
  fmt.Printf("%x\n", txt)
  fmt.Printf("% x\n", txt)
}

/* Output:
Hello
"Hello"
   Hello
Hello
48656c6c6f
48 65 6c 6c 6f
*/
```

#### Boolean Formatting Verbs
| Verb | Description |
| --- | --- |
| `%t` | Value of the boolean operator in true or false format (same as using `%v`). |

#### Float Formatting Verbs
| Verb | Description |
| --- | --- |
| `%e` | Scientific notation with `e` as exponent. |
| `%f` | Decimal point without exponent. |
| `%.2f` | Default width, precision 2. |
| `%6.2f` | Width 6, precision 2. |
| `%g` | Exponent as needed, only necessary digits. |

```go
package main
import ("fmt")

func main() {
  var i = 3.141

  fmt.Printf("%e\n", i)
  fmt.Printf("%f\n", i)
  fmt.Printf("%.2f\n", i)
  fmt.Printf("%6.2f\n", i)
  fmt.Printf("%g\n", i)
}

/* Output:
3.141000e+00
3.141000
3.14
  3.14
3.141
*/
```

<br />
<hr />

| Previous | Home | Next |
| :---: | :---: | :---: |
| [Constants](04-constants.md) | [Go Introduction](01-introduction.md) |  |