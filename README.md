# todo-cli

This repository is a little todo app made with this [tutorial](https://www.freecodecamp.org/news/how-to-build-a-to-do-app-with-rust/)

## Add an item

```
cargo run -- add "nameofitem"
```

## Set an item as complete

```
cargo run -- complete "nameofitem"
```
## Example

```
// this commands:
$ cargo run -- add "play video games"
$ cargo run -- add "write some code"
$ cargo run -- complete "write some code"

// will print that:
"add", "play video games"
todo saved
"add", "write some code"
todo saved
"complete", write some code"
todo saved
```

if we check the content of db.json, we will see something like that:

```
$ cat db.json
play video games    true
write some code     false
```
