<img src="https://www.yegor256.com/images/books/angry-tests/onion.svg" height="92px"/>

The following principles may help you write better automated tests.
They are excerpts from the [Angry Tests](https://www.yegor256.com/angry-tests.html) book.

## Basics

[2.1] Keep every test shorter than a dozen lines.

[2.2] Assert only once per test.

[2.3] Assert in every test.

[2.4] Finish every test with an `assert`.

[2.5] Don't use `assertDoesNotThrow`.

[2.6] Don't fail explicitly using `fail()`.

[2.7] Use irregular input values, instead of `foo` or `hello, world`.

[2.8] Use different inputs in every test, don't reuse.

[2.9] Always write failure messages.

[2.10] Don't share any data between tests.

[2.11] Don't use any static literals inside tests.

[2.12] Don't inline constants, assign them to variables first.

[2.13] Don't go around object interfaces, never via Reflection.

[2.14] Name tests as full English sentences, e.g. `buildsHtmlPage`.

[2.15] Never write any comments inside or outside of test methods.

[2.16] Don't assert on behavior not promised by object's contract.

[2.17] ...

[2.18] Don't test getters, setters, and similar primitive functionality.

[2.19] Don't delete test, disable them instead.

[2.20] Never test private or protected object methods.

[2.21] Close resources after use, like files and sockets.

[2.22] Don't write feature code that is only used in tests.

[2.23] ...

[2.24] Don't assert on side-effects, like logs.

[2.25] Assert on all possible intermediate results.

[2.26] Don't test constructors --- they are [code-free] anyway.

[2.27] Clean up in front of a test, not after it.

[2.28] Don't use mock frameworks, build [fake objects] instead.

[2.29] Don't forgive incorrect behavior, disable the test instead.

[2.30] Aim for one-statement tests.

[2.31] Use Hamcrest.

[2.32] Don't be discouraged to write bad tests, they're better than nothing.

[2.33] Every time you change the code, add more tests.

## Advanced

[3.1] Classify tests as "fast" (50ms per each) and "deep" (integrate all together).

[3.2] Make tests flaky and unstable, and expect bugs reported and fixed.

[3.3] Create custom matchers and reuse them in assert statements.

[3.4] Reproduce bugs with the minimum possible scaffolding.

[3.5] Tests must reproduce particular bugs, not successful usage scenarios.

[3.6] Invent a DSL and write test stories using it.

<hr>

Feel free to contribute.

[code-free]: https://www.yegor256.com/2015/05/07/ctors-must-be-code-free.html
[fake objects]: https://www.yegor256.com/2014/09/23/built-in-fake-objects.html
