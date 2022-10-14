## Introduction to Go

- Programming language created by Google in 2007
- Open sourced in 2009
- Multi-concurrency support
- Designed to run multithreaded concurrent applications that take advantage of
  new performant infrastructure
- Concurrency in Go is cheap & easy
- Main usecase of Go is, to use for performant applications that typically runs on scaled, distributed systems


## Characteristics of Go

- Simple syntax : Easy to learn, read and write code
- Fast build time, start up and run
- Resource Effiecient : Requires fewer resources
- Compiled language : Compiles into single binary (machine code) which can be used across different platforms

## Local setup to write/compile Go code

1. Download & Install Go : Follow instruction from [Go official documentation](https://go.dev/doc/install) to setup Go on your local machine.

2. IDE : Install IDE to write Go code


## Variables and constants in Go

# Variables
- Used for storing values which be changed/updated later if required.
- Give the variable name and reference everywhere in the app
- Update the value at one location and it will get updated where variable is referenced.
- Make our app more flexible
- If variable is declared but not used in the program, compiler shows warning for it.
- Synatx :
    `
        var a = "Hello World"
        a := "Hello World"
        var a string = "Hello World"
    `


# Constants
- Constants are like variables, except that their values cannot be changed once declared
  in the program.

## Pointers in Go

- Pointer is a variable which points to memory address of the another variable.
- Syntax : 
    `&variable_name`


## Print formatted data in Go
- It takes template string & annotation verb that will tell format function how to format 
  the variable passed in.
- Package fmt implements formatted I/O with functions analogous to C's printf and scanf. The format 'verbs' are derived from C's but are simpler.
- E.g. 
    `fmt.printf("Hello, welcome to golangNotes %s", username}`

- Refer Go official documentation to know more about available [formatting options](https://pkg.go.dev/fmt) for more details.


## How to take user input in Go
- Use fmt.scan() to take user input
- Example:
  `fmt.scan("Enter your name : ")`

## Datatypes in Go

- Go is statically typed language
- We need to tell compiler datatype when declaring the variable
- Syntax :
    `var varname datatype`


## Arrays in Go

- Fixed size single type array
- Syntax
  `var variablename = [size] datatype {comma separated elements}`
  `var variable_name = [size] datatype  <----- Declaring an empty array`

- Adding & accessing element by their index in array

## Slices in Go

- Slice is an abstraction of an array
- Variable sized array
- Can get subarray of its own
- Resized when needed
- Add new element in slice using append() at the end of an slice
- Syntax
  `
  var variablename [] datatype
  var variablename = [] datatype {}
  variablename := [] datatype {}
  `


## Loops in Go

- We only have the for loop in Go
- Syntax :
  `
    1. For loop :
     for {}
    2. For Each Loop :
    for index, index_var := range slice_var{}
    for _, index_var := range slice_var{}

  `