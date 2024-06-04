## Exported Names
- In Go, a name is exported if it **begins with a capital letter**.
- For example, `Pi` is an exported name, which is exported from the `math` package.
- `pi` does not start with a capital letter, so this is not exported.
- When importing a package, a function or a constant can only be referred by its exported names. Any *unexported* names are not accessible from outside the package.

Example:
```go
func main() {
	fmt.Println(math.Pi)     // Runs without an error
}

func main() {
	fmt.Println(math.pi)     // Runs with error - undefined
}
```
