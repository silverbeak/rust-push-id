# Rust Push Id
A Rust library for creating Firebase-style push id:s

## Crate
This is available as a Crate, [here](https://crates.io/crates/pushid).

## Usage

Add rust-push-id crate like so:

```toml
[dependencies]
pushid = "0.0.1"
```

The pushid library can then be used like this:
```rust
// Reference the crate
extern crate pushid;

// use PushIdGen from the crate
use pushid::PushIdGen;

fn main() {
    // Create generator. Remember to make it mutable
    let mut push_id_generator = pushid::PushId::new();
    
    // PushId can be generated using 'get_id'
    let id = push_id_generator.get_id();

    // ... use id here
    println!("{}", id);
}


```

## NB
This is my first attempt at rust. Hence, the code is not likely to be idiomatic Rust. I'll gladly accept improvements and PR:s.

## Credits
I was inspired by [this Gist from mikelehen](https://gist.github.com/mikelehen/3596a30bd69384624c11)
Mine is faster, his is prettier. :)

**-Kristofer**

[trollmoj.com](https://trollmoj.com/#blog)
