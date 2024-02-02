# Pipex
> This project will let you discover in detail a UNIX mechanism that you already know by using it in your program.

## Objectives
Reproduire le fonctionnement de `< file1 cmd1 | cmd2 > file2`.

## Usage
```sh
git clone git@github.com:Skalyaeve/pipex.git
cd pipex
make
echo "Hello, world!" > input
./pipex input cmd1 cmd2 output
```
