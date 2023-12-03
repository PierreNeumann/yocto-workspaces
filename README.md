# yocto-workspaces
Yocto builds managed with KAS. 

## Install dependecies

### Distribution specific dependencies 

Ubuntu : 

```
sudo apt-get install gawk wget git-core diffstat unzip texinfo gcc-multilib \
     build-essential chrpath socat libsdl1.2-dev xterm lz4
```

You may also need to change your locale configuration : 

```
sudo apt-get install language-pack-en language-pack-en-base manpages
sudo update-locale LANG=en_US.UTF8
```

### Install KAS 

Use the provided poetry environment : 

```
sudo apt install python3-poetry
poetry install 
```

It's recommended to use the poetry environment but you can altenatively install it manually. 

```
pip3 install kas
```


## Availables Images

### rpi4_poky 

Minimalist rpi4 poky image. 

## Build an Image 

```
poetry run kas build IMAGE XXX.yml
```

## developper documentation for KAS manifests

https://kas.readthedocs.io/en/latest/ 
