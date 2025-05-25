# Summary:
This Rust program declares a variable name with the value "John wick" and prints it to the console.

# Explanation

``` Rust
// Main entry point
fn main() {
    // Declare variable 
    let name: &str = "John wick";
    
    // Print variable in console 
    println!("{}", name);
}
```

## `let name: &str = "John wick";` 
- `let` keyword is used to declare a variable.
- `name` is the name of the variable.
- `:` is used to specify the type of the variable.
- `&str` is the type of the variable.
- `"John wick"` is the value of the variable.

## `println!("{}", name);`
- `println!` is a macro provided by the Rust standard library.
- `{}` is a placeholder for the value of the variable.
- `name` is the value of the variable.
