# Functions
Go programs are composed of functions. In Go, functions are typed entities that can either be named or be assigned to a variable as a value.


```
func moles(mass amu) float64 {
	return grams / float64(mass)
}
```

Go functions also have the ability to return multiple values.


```
func moles(mass amu) (float64, error) { 
    if mass < 0 { 
        return 0, error.New("Invalid mass!") 
    } 
    return (float64(mass) / grams), nil 
}
```

