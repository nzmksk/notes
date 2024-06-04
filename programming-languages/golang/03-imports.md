## Imports
- Used to import other packages to be used together with the local package.
- Import statements can be written multiple times.

Example:

```go
import "fmt"
import "math"
```

But it is good style to use the _factored_ import statement.

```go
import (
	"fmt"
	"math"
)
```
