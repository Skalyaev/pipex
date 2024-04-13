# <p align="center">pipex</p>
> *Ce projet vise à approfondir votre compréhension des deux concepts que vous connaissez déjà : les redirections et les pipes. Il s'agit d'un projet d'introduction pour les projets UNIX plus importants qui apparaîtront plus tard dans le cursus.*
>
> *Votre programme devra reproduire le comportement de la syntaxe suivante: **`< file1 cmd1 | cmd2 > file2`***

## Preview
![](https://github.com/Skalyaeve/images-1/blob/main/screenshot/pipex.gif)

## Install
```bash
sudo apt update -y
sudo apt install -y gcc
sudo apt install -y make
```
```bash
mkdir -p $HOME/.local/bin
mkdir -p $HOME/.local/src
mkdir -p $HOME/.local/include
```
```bash
link=Skalyaeve/pipex
name=pipex

git clone https://github.com/$link.git $name
cd $name && make && make clean

ln -s $PWD/$name $HOME/.local/bin/$name
ln -s $PWD/src $HOME/.local/src/$name
ln -s $PWD/include $HOME/.local/include/$name
```

## Usage
```bash
export PATH=$HOME/.local/bin:$PATH
pipex <file> <cmd> <cmd> <file>
```

## Uninstall
```bash
name=pipex

rm -rf $name
rm $HOME/.local/bin/$name
rm $HOME/.local/src/$name
rm $HOME/.local/include/$name
```

