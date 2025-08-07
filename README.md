# cross-tools-riscv64

riscv64 cross-compile toolchain, supports both x86_64(amd64) and aarch64(arm64) architectures.

## Supported targets

| Version | Target                    | Kernel | Binutils | GCC    | Libc(glibc) | Libc(musl) |
| ------- | ------------------------- | ------ | -------- | ------ | ----------- | ---------- |
| stable  | riscv64-unknown-linux-gnu | 6.6.74 | 2.41     | 12.4.0 | 2.38        | ---        |


## How to use

Download the tarball from the [release page](https://github.com/czhehua/crosstool-riscv64) and extract it to `/opt/x-tools`:

```sh
sudo mkdir -p /opt/x-tools
sudo tar -xf x86_64-cross-tools-riscv64-unknown-linux-gnu-stable.tar.xz -C /opt/x-tools
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
- [cross-tools](https://github.com/loong64/cross-tools)