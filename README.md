# install-deft

A GitHub Action to install [deft](https://github.com/dylan-lang/deft). This action also
invokes the [install-opendylan](https://github.com/dylan-lang/install-opendylan) Action.

To install the latest deft release:

```yaml
    - uses: dylan-lang/install-deft@v1
```

To install a specific released version:

```yaml
    - uses: dylan-lang/install-deft@v1
      with:
        tag: v0.12.0
```

`tag` must exactly match a tagged version in the [deft
repository](https://github.com/dylan-lang/deft).

When this Action has completed the `deft` executable is available on the `PATH` and the
`deft` directory contains the `deft` checkout and build products.

See the [hello](https://github.com/cgay/hello) repository for the canonical
example of using this Action.
