# make

## structure of a Makefile rule

The file name is typically ``Makefile``.

```Makefile
target ... : prerequisite ...
	recipe
	...
```

To create the _target_, the _recipe_ commands will be executed. If the
_prereqisites_ are newer, the rules for building them are executed first.
Prerequisites and recipies are optional.

* **tab** character in front of recipe required
* if you want to use another character, set ``.RECIPEPREFIX``
* the **backslash** character connects two lines
* the **gate** character is for comments - everything after is treated as a
  comment

## rules

* ``.DEFAULT_GOAL: target`` sets the default target otherwise it's the first
  target found
* a target can be provided multiple times - the result is cumulated
* one can use implicit (build-in) rules


## variables

```Makefile
# define variable
objects = a.o b.o c.o
# use variable
echo $(objects)
```

