---
layout: default
---

# Arrays

Example demonstrates printing arrays on console. Click [here](https://blog.golang.org/go-slices-usage-and-internals) to learn more

```go
func main() {
	// Defining Array Variation #1
	var avengers [5]string

	avengers[0] = "Iron Man"
	avengers[1] = "Captain America"
	avengers[2] = "Ant Man"
	avengers[3] = "Spider Man"
	avengers[4] = "Thor"

	for index := 0; index < len(avengers); index++ {
		fmt.Printf("Avenger at index [%d] is '%s'", 
			index, avengers[index])
		fmt.Println()
	}

	// Defining Array Variation #2
	cricketers := [5]string{
		"Sachin Tendulkar",
		"MS Dhoni",
		"Rahul Dravid",
		"Anil Kumble",
		"Virat Kohli",
	}

	for index, cricketer := range cricketers {
		fmt.Printf("Cricketer at index [%d] is '%s'", index, cricketer)
		fmt.Println()
	}
}
```

### Output

```bash
Avenger at index [0] is 'Iron Man'
Avenger at index [1] is 'Captain America'
Avenger at index [2] is 'Ant Man'
Avenger at index [3] is 'Spider Man'
Avenger at index [4] is 'Thor'
Cricketer at index [0] is 'Sachin Tendulkar'
Cricketer at index [1] is 'MS Dhoni'
Cricketer at index [2] is 'Rahul Dravid'
Cricketer at index [3] is 'Anil Kumble'
Cricketer at index [4] is 'Virat Kohli'
```

<a href='https://play.golang.org/p/f3UzBIDZQmy' target='_blank'>Try It Out</a> | <a href='https://github.com/sagar-jadhav/go-examples/blob/master/src/arrays.go' target='_blank'>Source Code</a>

### Contributors
- <a href='https://github.com/sagar-jadhav' target='_blank'>Sagar Jadhav</a>

[<< Home Page](./) | [Previous << Pointer](./pointer.html) | [Next >> Slice](./slice.html)
