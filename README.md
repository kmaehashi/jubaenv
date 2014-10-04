Simple Jubatus Version Management: jubaenv
=======================================================

jubaenv is a simple Jubatus version switcher like `pyenv` or `rbenv`.

Requirements
-------------------------

* git command
* bash or zsh
* g++ (or any compiler that can build Jubatus and its dependencies)

Installation
--------------------------

```
$ git clone https://github.com/kmaehashi/jubaenv.git ~/.jubaenv
```

Add the following line to your shell rc file.

```
eval "$(~/.jubaenv/bootstrap)"
```

Usage
-----------------

List all Jubatus versions available:

```
$ jubaenv install -l
```

Install Jubatus:

```
$ jubaenv install 0.6.3
```

List Jubatus versions installed:

```
$ jubaenv shell
0.5.4  0.6.3
```

Switch Jubatus version for the current shell:

```
$ jubaenv shell 0.6.3

$ jubaclassifier --version
jubatus-0.6.3 (jubaclassifier)
```
