# Cargo deb

This is [cargo-deb] configured for use with [whalebrew] to build debian packages on non-linux
systems. Install it with:

```sh
whalebrew install ghcr.io/dnaka91/cargo-deb
```

Then you can use it the same as the normal **cargo-deb** but it's running in a Docker container in
the background.

[cargo-deb]: https://github.com/mmstick/cargo-deb
[whalebrew]: https://github.com/whalebrew/whalebrew
