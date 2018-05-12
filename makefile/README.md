# Makefiles

## Structure of a Makefile rule

```Makefile
target ... : prerequisite ...
	recipe
	...
```

To create the _target_, the _recipe_ commands will be executed. If the
_prereqisites_ are newer, the rules for building them are executed first.
Prerequisites and recipies are optional.

* __tab__ character in front of recipe required
* if you want to use another character, set ``.RECIPEPREFIX``
* the **backslash** character connects two lines
* the **gate** character is for comments - everything after is treated as a comment
