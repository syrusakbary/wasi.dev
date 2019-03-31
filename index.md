---
layout: page
title: WASI
permalink: /
subtitle: The WebAssembly System Interface
header_text_feature_image: polyfill/WASI-small.png
---

For a quick intro to WASI, including getting started using it, see [the intro document](https://github.com/CraneStation/wasmtime/blob/master/docs/WASI-intro.md).

For more documentation, see [the documents guide](https://github.com/CraneStation/wasmtime/blob/master/docs/WASI-documents.md).

Here's a quick guide to the repositories where things live:

[wasi-sdk](https://github.com/CraneStation/wasi-sdk) - “WASI SDK” packages for C/C++. If you want to try out compiling C/C++, this is a good place to start. "It's just clang."

WASI-enabled Rust - Rust Nightly builds now have built-in WASI support. To get started using Rust for targeting WASI:

```
rustup target add wasm32-unknown-wasi --toolchain nightly
cargo +nightly build --target wasm32-unknown-wasi
```

[wasmtime](https://github.com/CraneStation/wasmtime/) - Wasmtime WebAssembly runtime, with WASI support, as well as the WASI documentation.

[Lucet](https://github.com/fastly/lucet/) - Fastly's WebAssembly runtime with WASI support.

Everything here is a work in progress prototype, and not yet stable.
