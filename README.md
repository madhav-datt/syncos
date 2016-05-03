# syncos

Working on two operating systems can be a pain, and even more so if you use both for similar kinds of work. `syncos` helps you sync directories across operating systems on your dual booted machine so you don't have to keep switching or copy-pasting files from one OS to the other.

## Installing syncos

```shell
$ wget -P ~/Downloads https://github.com/madhav-datt/syncos/archive/syncos-v1.0.zip
$ unzip ~/Downloads/syncos-v1.0.zip
$ mv ~/Downloads/syncos-syncos-v1.0 ~/Downloads/syncos
$ chmod +x syncos/install
$ sudo syncos/install
```

The program uses `rsync` which will be installed by the `install` script.

## Using syncos
