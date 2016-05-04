# syncos :computer: :arrows_counterclockwise: :computer:

Working on two operating systems can be a pain, and even more so if you use both for similar kinds of work. `syncos` helps you sync directories across operating systems on your dual booted machine so you don't have to keep switching or copy-pasting files from one OS to the other.

## Installing syncos

### From source

```shell
$ cd ~/Downloads
$ git clone https://github.com/madhav-datt/syncos.git
$ chmod +x syncos/install
$ sudo syncos/install
```

The program uses `rsync` which will be installed by the `install` script.

## Using syncos

Suppose you are working on the final project for one of your courses and have folders for it on both the operating systems (Ubuntu and Windows) of your laptop. On the Ubuntu partition, your code is in a folder called `cs121-final-project` on the desktop and on your Windows desktop in a folder called `project_cs121`. 

```shell
$ syncos --help
$ syncos --add DIRECTORY_OS1 DIRECTORY_OS2
$ syncos --list
$ syncos --remove DIRECTORY_OS1 DIRECTORY_OS2
```

### help :question:

To figure out what to do if you get stuck:

    $ syncos

![syncos help](https://github.com/madhav-datt/syncos/blob/master/resources/help.png)

### add :heavy_plus_sign:

To add a new pair of directories across the OSs of your dual-booted computer:

    $ syncos --add ~/Desktop/cs121-final-project Users/madhav/project_cs121

![syncos add](https://github.com/madhav-datt/syncos/blob/master/resources/add.png)

### list :notebook:

If you don't remember all the directories you have synced:

    $ syncos --list

![syncos list](https://github.com/madhav-datt/syncos/blob/master/resources/list.png)

### remove :x:

If you don't want a pair of directories to sync anymore:

    $ syncos --remove ~/Desktop/cs121-final-project Users/madhav/project_cs121

![syncos remove](https://github.com/madhav-datt/syncos/blob/master/resources/remove.png)
