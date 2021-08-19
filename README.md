# Vapor
Vapor (vLang) is a language that sits on top of python

See more here at the official website: https://mwd1993.github.io/Vapor/index.html

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
