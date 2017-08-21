# gocolor

A simple lib to help you color when developing some bash applications using ANSI-COLORS.

The goal is to make the lib leaner and leaner.

The gcolor was made just with this intuition to leave the texts in the colored bash.

You can collaborate by giving a "Fork" and sending us a "pull request", lib gcolor was just an academic play with only didactic input, which we use in our projects, something fun to do and learn.


## Install

```go

go get github.com/jeffotoni/gcolor

```

## Use gcolor

```go

package main

import (
	// "fmt"
	. "github.com/jeffotoni/gcolor"
)

//
// start
//
func main() {

	//
	// First instantiate form
	//
	var C Color
	C.Cor = "purple"
	C.Cprintln("Purple")

	//
	// Second way to instantiate
	//
	c := new(Color)
	c.Cor = "green"
	c.Cprintln("Color Green")

	//
	// Third way to instantiate
	//
	red := Color{"red"}
	red.Cprintln("Color red")

	//
	// Fourth way to instantiate
	//
	Red.Cprintln("Red color instance otherwise")

	//
	// Yellow
	//
	Yellow.Cprintln("Yellow color!!")

}

```