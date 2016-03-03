Learning APL
----------------------
Don't need to install anything in your PC.. it could be done with online interpreter http://ngn.github.io/apl/web/

It is a language where the code lines need to read from right to left i.e.

```2+2 2+2``` it is not ```4 4``` but ```6 6```

Cheat sheet https://en.wikipedia.org/wiki/APL_syntax_and_symbols

Lets solve Euler's problems (https://projecteuler.net/archives):

1.If we list all the natural numbers below 10 that are multiples of 3 or 5, we get 3, 5, 6 and 9. The sum of these multiples is 23.

Find the sum of all the multiples of 3 or 5 below 1000.

```
n ← 1 + ⍳999
t ← ((3 |n) = 0)
f ← ((5 |n) = 0)
+/ ((f + t) > 0) / n

```
_Answer:_ 233168
