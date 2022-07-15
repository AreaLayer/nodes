# LNP/BP nodes integration

The repo provides integration packages for LNP/BP node suit, which includes

- [BP Node](https://github.com/BP-WG/bp-node),
- [LNP Node](https://github.com/LNP-WG/lnp-node),
- [RGB Node](https://github.com/RGB-WG/rgb-node),
- [Storm Node](https://github.com/Storm-WG/storm-node), and
- [Store Service](https://github.com/Storm-WG/storm-node), which usually shipped separately from
  the Storm node.

Installing all nodes locally:

```shell
rustup update nightly
cargo +nightly install lnpbp_nodes -Z bindeps
```

Installing just command-line tools:

```shell
rustup update nightly
cargo +nightly install lnpbp-cli -Z bindeps
```

Using RPC API in another project `Cargo.toml`:

```toml
[dependecies]
lnpbp_rpc = "0.8.0"
```

## Integration architecture

![image](https://user-images.githubusercontent.com/372034/174442561-117e9225-3912-49c8-9609-c71c70cd81d6.png)
