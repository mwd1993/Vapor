# Vapor
Vapor (vLang) is a language that sits on top of python

See more here at the official website: https://mwd1993.github.io/Vapor/index.html

### printing made simple, included fstring functionality

```
message = "Hello World From Vapor"

'the message is [[message]]'
```
### simple for loops
```
message each word {
  'current word is [[word]]'
}

message each word with index {
  'current word is [[word]] at loop index [[index]]'
}
```
### simple if statement functionality, suffix statement with 'true' or 'false'
```
len(message) > 0 true {
  'message has [[len(message)]] words'
}
```
