# Immutable variable

In Rust, immutable variables are variables that cannot be changed after they are initialized. By default, variables in Rust are immutable unless explicitly made mutable using the mut keyword.

Here's a simple example of an immutable variable:

## Step 1: Declare variable
``` Rust
// Main entry point
fn main() {
    // Declare variable 
    let name: &str = "John wick";
    
    // Print variable in console 
    println!("{}", name);
}
```

## Step 2: Run code
``` output
John wick
```

## Step 3: Conclusion
Immutable variables are useful for ensuring that variables don't change unexpectedly, which can help prevent bugs and make your code more predictable.

``` Rust
// Main entry point
fn main() {
    // Declare immtuable variable
    let name: &str = "John wick";
    
    // Change variable value
    name = "Jhack wick";
    
    // Print variable in console 
    println!("{}", name);
}
```

It will throw an error
``` Bash
error[E0384]: cannot assign twice to immutable variable `name`
```

## Step 4: Fix Error

Add `mut` keyword before variable name to make it mutable.

``` Rust
// Main entry point
fn main() {
    // Declare mutable variable
    let mut name: &str = "John wick";
    
    // Change variable value
    name = "Jhack wick";
    
    // Print variable in console 
    println!("{}", name);
}
```
## Step 5: Run code
``` output
Jhack wick
```




