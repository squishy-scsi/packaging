# Squishy flatpak

**NOTE:** This is very experimental and likely to have major bugs

## Building and running locally

**NOTE:** Due to a bug in older versions of flatpak-builder version `>=1.2.3` is required (https://github.com/flatpak/flatpak-builder/pull/497)

In order to build and run this locally, you need `flatpak` and `flatpak-builder`.
Se instructions in: https://docs.flatpak.org/en/latest/first-build.html

Building and installing the package for user:
```sh
flatpak-builder --force-clean --user --install-deps-from=flathub --repo=repo --install builddir moe.scsi.squishy.yml
```

Running the installed package:
```sh
flatpak run moe.scsi.squishy --help
```

Removing the package:
```sh
flatpak remove moe.scsi.squishy
```
