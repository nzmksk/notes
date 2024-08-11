## Go Arrays

### Declaration<sup>[1]</sup>

```go
package main
import ("fmt")

func main() {
    // Length is defined
    var arr1 = [3]int{1,2,3}
    arr2 := [5]int{4,5,6,7,8}

    // Length is inferred
    var arr3 = [...]int{1,2,3}
    arr4 := [...]int{4,5,6,7,8}
}
```

### Accessing Elements

```go
package main
import ("fmt")

func main() {
    prices := [3]int{10,20,30}

    fmt.Println(prices[0])  // 10
    fmt.Println(prices[2])  // 30
}

```

### Changing Elements

```go
package main
import ("fmt")

func main() {
    prices := [3]int{10,20,30}

    prices[2] = 50
    fmt.Println(prices) // [10, 20, 50]
}
```

### Array Initialization

If an array or one of its elements has not been initialized, it is assigned the [default value](06-data-types.md#default-values-of-data-type) of its type.

```go
package main
import ("fmt")

func main() {
    arr1 := [5]int{}            // not initialized
    arr2 := [5]int{1,2}         // partially initialized
    arr3 := [5]int{1,2,3,4,5}   // fully initialized

    fmt.Println(arr1)           // [0 0 0 0 0]
    fmt.Println(arr2)           // [1 2 0 0 0]
    fmt.Println(arr3)           // [1 2 3 4 5]
}
```

It is also possible to initialize only specific elements in the array.

```go
package main
import ("fmt")

func main() {
    arr1 := [5]int{1:10,2:40}

    fmt.Println(arr1)   // [0 10 40 0 0]
}
```

### Find the Length of an Array

Use `len()` to find the length of an array.

```go
package main
import ("fmt")

func main() {
    arr1 := [4]string{"Volvo", "BMW", "Ford", "Mazda"}
    arr2 := [...]int{1,2,3,4,5,6}

    fmt.Println(len(arr1))  // 4
    fmt.Println(len(arr2))  // 6
}
```

### Notes

- <sup>[1]</sup> _length_ specifies the number of elements to store in the array. In Go, arrays have a **fixed length**. The length of the array is either defined by a number or is inferred (based on the number of elements).

<br />
<hr />

|            Previous            |                 Home                  | Next |
| :----------------------------: | :-----------------------------------: | :--: |
| [Data Types](06-data-types.md) | [Go Introduction](01-introduction.md) |      |
