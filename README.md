# monkey-interpreter
The implementation of the Monkey interpreter, as seen in Thorsten Ball book, Writing An Interpreter In Go.

## How to Use
This interpreter has its own REPL. To start it, go to the following location and execute that command.

`cd src/monkey/`

`go run main.go`

Now that you are in the REPL, it is time to write some Monkey code. Here are some examples.

```
Hello gctse! This is the Monkey programing language!
Feel free to type in commands
>> let astring = "astring"
>> astring + " plus"
astring plus
>> let afunc = fn() { return astring + " plus" }
>> afunc()
astring plus
```

```
Hello gctse! This is the Monkey programing language!
Feel free to type in commands
>> let a = 5
>> let b = 10
>> let f = fn(x, y) { if (x > 4) { return x * y } else { return x + y } }
>> f(a,b)
50
>> let a = 2
>> f(a,b)
12
```

```
Hello gctse! This is the Monkey programing language!
Feel free to type in commands
>> let myarray = [1,2,3,4]
>> let myhash = {"name": "bob", "age": 25, "isAdult": true }
>> myarray[2]
3
>> len(myarray)
4
>> myhash["name"]
bob
>> myhash["age"]
25
```

## How to Test

Each package has its set of tests. To run them, run the command `go test ./package-name`. For example: `go test ./evaluator`.