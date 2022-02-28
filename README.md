# Vapor
Vapor (vLang) is a dynamic (but supports a type system) programming language that transpiles down to valid python code.

See more here at the official website: https://mwd1993.github.io/Vapor/index.html  

# Vapor IDE In Development ( Coming Soon! )

<img src="https://raw.githubusercontent.com/mwd1993/Vapor/main/Images/VaporIDE_Alpha_Example1png.png" width="700" height="450">  

# Getting Started

### [download](https://github.com/mwd1993/Vapor/releases) the Compiler and then run your .vap files like so  
```
vapor_parsor.exe path/to/my_vapor_file.vap args1 arg2 etc
```

### printing made simple, included fstring functionality

```
message = "Hello World From Vapor"

'the message is [[message]]'
```
### simple for loops
```c++
message = "Hello World From Vapor"

message each word {
  'current word is [[word]]'
}

# enumeration
message each word with index {
  'current word is [[word]] at loop index [[index]]'
}
```
### simple if statement functionality, suffix statement with 'true' or 'false'
```c++
message = "Hello World From Vapor"

len(message) > 0 true {
  'message has [[len(message)]] words'
}
```

# Fizz Buzz
```c++
m do_fizz_buzz() {
    range(101) each number {
        number % 3 == 0 true {
            'Fizz'
            continue
        }
        number % 5 == 0 true {
            'FizzBuzz'
            continue
        }
        '[[number]]'
    }
    -> 'this is a return value'
}

return_value = do_fizz_buzz()
```
