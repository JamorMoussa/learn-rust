# Custom types: 
Rust has two main keyworks for making a custom data types are `struct` and `enum`.

- `struct` : used for defining structure.
- `enum` : define a enumeration.


## Structures: 

In Rust there are three types of structures:

- **Tuple Structs**: which are named tuples.
- **Classic Struct**: which are the classic C strcut.
- **Unit Struct**: which are fields-less, are useful for generics.

### Tuple Structs: 

The first type that we'll discuss is `Tuple struct`, which are basicaly named tuples.

```rust
#[derive(Debug)]
struct Point(f32, f32);

fn main(){
    
    let p1 = Point(1.0, 2.0);

    println!("x = {:?}", p1.0);
    println!("y = {:?}", p1.1);

}
```
The code above, shows us how to define a tuple struct, using the `struct` keyword. we define a `Point` that has two fields of type `f32`. Then we define a `p1` which is an instance, we can access to any item by index, like any tuple in rust.


