# Makefiles

## Structure of a Makefile rule

```Makefile
target ... : prerequisite ...
	recipe
	...
```

* TAB character in front of recipe required
* if you want to use another character, set .RECIPEPREFIX
