F100
====

We've found a `core` file in a repository on GitHub. The developer should have
added core dumps to his `.gitignore`. See if you can do anything with it.

Flag
----

`t#hean;SW.er`


Answer
------

By running `strings` one can see a "password:" string there. Nearby you can see
the string "not~the~answer" several times. Actually, you just need to pay
attention to the first strings. The answer is "t#hean;SW.er".


Testing
=======

Core dumps must be enabled first with `ulimit -c unlimited`.

Run `make` to create a `core` file to make available to contestants. The answer
must be in the first 40 lines of strings output for this to be doable quickly.


-- Carlos Rodrigues
