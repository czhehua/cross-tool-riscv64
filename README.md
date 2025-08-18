# cross-tools-riscv64

riscv64 cross-compile toolchain, supports both x86_64(amd64) and aarch64(arm64) architectures.

## Supported targets

| Version | Target                     | Kernel | Binutils | GCC    | Libc(glibc) | Libc(musl) |
| ------- | -------------------------- | ------ | -------- | ------ | ----------- | ---------- |
| stable  | riscv64-unknown-linux-gnu  | 6.6.74 | 2.41     | 12.4.0 | 2.38        | ---        |
| stable  | riscv64-unknown-linux-musl | 6.6.74 | 2.41     | 14.2.0 | ---         | 1.2.5      |


## How to use

Download the tarball from the [release page](https://github.com/czhehua/cross-tool-riscv64/releases) and extract it to `/opt/x-tools`:

```sh
sudo mkdir -p /opt/x-tools
sudo tar -xf XXX-cross-tools-riscv64-XXX.tar.xz -C /opt/x-tools
```

## How to build

Fork this project and create a new release, or build manually:

```sh
./make
```

## License

MIT

## Acknowledgements

We would like to express our gratitude to the following individuals and projects:

- [crosstool-ng](https://github.com/crosstool-ng/crosstool-ng)
- [musl-cross](https://github.com/musl-cross/musl-cross)
- [loong64/cross-tools](https://github.com/loong64/cross-tools)