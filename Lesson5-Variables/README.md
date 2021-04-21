Fun facts:

By default all variables are immutable. Once you assign, you cannot change

Lets say...
```
fn main() {
  let name = "neelima";
  println!("name is {}", name);
```
Now, lets try to reassign the name to something else
```
fn main() {
    let name = "neelima";    // created a variable `name` and assigned a value to it
    println!("name is {}", name);
    name = "neelkrish";    // trying to assign a new value to the variable `name`      println!("new name is {}", name);
}
```
yay! Now you have succesfully pissed off the compiler :D

Can you make it mutable? Yes!
-> Use "mut", for example: let mut name = "neelima";
```
fn main() {
    let mut name = "neelima";    // just change the varible to a `mutable` variable
    println!("name is {}", name);
    name = "neelkrish";
    println!("new name is {}", name);
}
```
Or, we can use Shadowing. Redeclare an already declared variable, again  :)

For example:
```
fn main() {
    let name = "neelima";
    println!("name is {}", name);
        let name = "neelkrish";  // here the variable is in inner scope (see the braces?), and this is shadowing the external declartion of `name`
        println!("new name is {}", name);
}
```

Its not complicated...Yet!

