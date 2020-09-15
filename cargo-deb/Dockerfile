FROM rust as builder

RUN cargo install cargo-deb

FROM rust

COPY --from=builder /usr/local/cargo/bin/ /usr/local/cargo/bin/

LABEL io.whalebrew.config.volumes='[\
  "~/.cargo/git:/usr/local/cargo/git",\
  "~/.cargo/registry:/usr/local/cargo/registry",\
  "$PWD/target:/workdir/target"\
]'

ENTRYPOINT ["cargo", "deb"]
