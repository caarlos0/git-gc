# git-gc [![SayThanks.io](https://img.shields.io/badge/SayThanks.io-%E2%98%BC-1EAEDB.svg?style=flat-square)](https://saythanks.io/to/caarlos0)

> A simple bash script to reduce your local repos' size.

## Usage

```console
$ ./git-gc ~/Code
$ DEBUG=1 ./git-gc ~/Projects
```

## What does it do?

Basically, it expires all reflogs with `git reflog expire --all --expire=now`
and then it does an aggressive GC with `git gc --aggressive --prune=now`.

And, sure, print the results!
