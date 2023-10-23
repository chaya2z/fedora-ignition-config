# fedora-ignition-config

## Generate Ignition file

```shell
butane config.bu >| public/transpiled_config.ign
```

## coreos-installer

I can install CoreOS using the raw file of GitHub without hosting a server by myself.

```shell
sudo coreos-installer install /dev/sda \
    --ignition-url https://raw.githubusercontent.com/chaya2z/fedora-ignition-config/main/public/transpiled_config.ign
```
