# Javy npm package

This is the npm package for javy. The package contains a small Node script
that downloads the appropriate javy binary on demand and invokes it with the
parameters given. 

## Usage

```
# Install javy globally
$ npm install -g javy

# Directly invoke it via npm
$ npx javy
```

## Updating javy

The npm package won't download javy again once its downloaded. If a new
version of the javy npm package has been published, you can use the following
invocation to update to the latest release:

```
UPDATE_JAVY=1 npx jaxy
```

## Building from source

If there are no binaries available for your platform or the available binaries
don't work for you for some reason, the npm package can also build javy from 
source.

```
BUILD_JAVY=1 npx javy
```

Please note that for this to work you must have all prerequisites of javy
(listed in the [README]) installed. (That is CMake, Rust, Rust for wasm32-wasi
target, cargo wasi, wasmtime-cli and Rosetta on Mac M1).

[README]: https://github.com/Shopify/javy/blob/main/README.md


