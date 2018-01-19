# BLSP - Biel LISP

A very simple LISP interpreter built in Python, implemented in < 50 lines of code.

Usage:
```
eval(parse("""(
    let factorial (lmb x
        (if (== x 1) 1
            (* x (factorial (- x 1)))
        )
    ) (factorial 10)
)""")) == 3628800
```