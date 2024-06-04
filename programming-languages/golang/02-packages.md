## Packages
- Every Go program is made up of packages.
- Programs start running in package `main`.
- By convention, the package name is the same as the last element of the import path. For example, the `math/rand` package comprises files that begin with the statement `package rand`.

Example:
`packages.go`
```go
package main

import (
	"fmt"
	"math/rand"
)

func main() {
	fmt.Println("My favorite number is", rand.Intn(100))
}
```

Sample output:
```
My favorite number is 9
```