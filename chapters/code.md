# Code 

Syntax highlighting is built-in!


```fsharp
// sum : int list -> int
let rec sum xs = 
    match xs with
    | [] -> 0
    | first :: rest -> first + sum rest
```