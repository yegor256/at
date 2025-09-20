<img src="https://www.yegor256.com/images/books/angry-tests/onion.svg" height="92px"/>

The following principles may help you write better automated tests.
They are excerpts from the [Angry Tests](https://www.yegor256.com/angry-tests.html) book.

[2.1] Keep every test shorter than a dozen lines.

[2.2] `assert` only once per test.

[2.3] `assert` in every test.

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

Feel free to contribute.
