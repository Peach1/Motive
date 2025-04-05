# Motive
The companion scripting language for Stainless Steel.

Motive is a high level programming language designed for 3D video games and interactive multimedia.
It's a single language designed to be natively compiled to machine code
or used as an embedded scripting language.
Motive is a mix of popular programming languages in one minimalistic user friendly design

It's a C-like language primarily influenced by Swift, Rust, GLSL, Haskell, C++, Standard ML, Lua, and (The good parts of)Javascript.

Designed to be easy to use, even for complete beginners -
No manual memory allocation, no confusing naming

## Features

* Statically typed - Variable types don't change, large code bases are easier to manage
* Type inference - All the fun of a dynamic language, but without the runtime type errors 
* High Level Standard libraries: vector math, matrixes, text processing, image processing and more are built in
* Unicode support built in (grapheme clusters, oh my!)
* First class functions - pass around functions as easily as any other data type
* Polymorphic lambdas - write a function once, and it works for all compatible types 
* First class types - Pass around type information at compile time using the same language
* Automatic Reference counting with cycle detection and no garbage collector
* User friendly compiler error messages


```typescript

let today = "Friday";

const PI = 3.14 // use 'const' to declare unchanging values; semicolons are optional in Motive

fn add(x : int, y : int) -> int // fn stands for function; 'int' stands for integer(a whole number)
{
    return x+y;
}

fn add2(x,y) { x+y } // Generic functions are made by omitting types

int wow(int x, int y) { return x+y; } // C style function syntax also works too (the power of backward compatiblity!)

fn example()
{
    let x = PI*2.0; // 'let' is a variable that can't be modified
    mut y = x; // 'mut' is a variable than can *can* be modified
    y *= 2;
    y // Functions return the last expression in a block. 'return' also works too
}

```
 




## License

Licensed under either of

 * Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
 * MIT license ([LICENSE-MIT](LICENSE-MIT) or http://opensource.org/licenses/MIT)

at your option.

### Contribution

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall be dual licensed as above, without any
additional terms or conditions.
