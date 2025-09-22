<img src="https://www.yegor256.com/images/books/angry-tests/onion.svg" height="128px"/>

[![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/yegor256/at/blob/master/LICENSE.txt)

The following principles may help you write better automated tests.
They are excerpts from the [Angry Tests] book.
To get a more detailed explanation you may want to read the book.

## Chapter 2. Basics

<a name="2-1">[<a href="#2-1">2.1</a>]</a> Keep every test shorter than a dozen lines.

<a name="2-2">[<a href="#2-2">2.2</a>]</a> Assert only once per test.

<a name="2-3">[<a href="#2-3">2.3</a>]</a> Assert in every test.

<a name="2-4">[<a href="#2-4">2.4</a>]</a> Finish every test with an assertion.

<a name="2-5">[<a href="#2-5">2.5</a>]</a> Don't use [assertDoesNotThrow].

<a name="2-6">[<a href="#2-6">2.6</a>]</a> Don't fail explicitly using [fail].

<a name="2-7">[<a href="#2-7">2.7</a>]</a> Use irregular input values, instead of `"foo"`.

<a name="2-8">[<a href="#2-8">2.8</a>]</a> Use different inputs in every test, don't reuse them.

<a name="2-9">[<a href="#2-9">2.9</a>]</a> Always write failure messages.

<a name="2-10">[<a href="#2-10">2.10</a>]</a> Don't share any data between tests; never use `setUp` and `tearDown`.

<a name="2-11">[<a href="#2-11">2.11</a>]</a> Don't define constants (static literals) inside tests.

<a name="2-12">[<a href="#2-12">2.12</a>]</a> Don't inline constants; assign them to variables first.

<a name="2-13">[<a href="#2-13">2.13</a>]</a> Don't bypass object interfaces, especially not via Reflection.

<a name="2-14">[<a href="#2-14">2.14</a>]</a> Name tests as full English sentences starting with a verb, e.g., `buildsHtmlPage`.

<a name="2-15">[<a href="#2-15">2.15</a>]</a> Never write any comments inside or outside of test methods.

<a name="2-16">[<a href="#2-16">2.16</a>]</a> Don't assert on behavior not promised by the object's contract.

<a name="2-17">[<a href="#2-17">2.17</a>]</a> Assert on the most vulnerable pain points.

<a name="2-18">[<a href="#2-18">2.18</a>]</a> Don't test getters, setters, and similar primitive functionality.

<a name="2-19">[<a href="#2-19">2.19</a>]</a> Don't delete tests, disable them instead.

<a name="2-20">[<a href="#2-20">2.20</a>]</a> Never test private or protected object methods.

<a name="2-21">[<a href="#2-21">2.21</a>]</a> Close resources after use, such as files and sockets.

<a name="2-22">[<a href="#2-22">2.22</a>]</a> Don't write feature code that is only used in tests.

<a name="2-23">[<a href="#2-23">2.23</a>]</a> Assert at every step while getting to the end of a use case.

<a name="2-24">[<a href="#2-24">2.24</a>]</a> Don't assert on side effects, like logs.

<a name="2-25">[<a href="#2-25">2.25</a>]</a> Assert on all possible intermediate results.

<a name="2-26">[<a href="#2-26">2.26</a>]</a> Don't test constructors — they are [code-free] anyway.

<a name="2-27">[<a href="#2-27">2.27</a>]</a> Clean up before a test, not after it.

<a name="2-28">[<a href="#2-28">2.28</a>]</a> Don't use mock frameworks, build [fake objects] instead.

<a name="2-29">[<a href="#2-29">2.29</a>]</a> Don't forgive incorrect behavior, disable the test instead.

<a name="2-30">[<a href="#2-30">2.30</a>]</a> Aim for [one-statement] tests.

<a name="2-31">[<a href="#2-31">2.31</a>]</a> Use [Hamcrest].

<a name="2-32">[<a href="#2-32">2.32</a>]</a> Don't be discouraged from writing bad tests; they're better than nothing.

<a name="2-33">[<a href="#2-33">2.33</a>]</a> Every time you change the code, add more tests.

## Chapter 3. Advanced

<a name="3-1">[<a href="#3-1">3.1</a>]</a> Classify tests as "fast" (50ms each) and "deep" (integrating everything).

<a name="3-2">[<a href="#3-2">3.2</a>]</a> Make tests flaky and unstable, then expect bugs to be reported and fixed.

<a name="3-3">[<a href="#3-3">3.3</a>]</a> Create custom matchers and reuse them in assert statements.

<a name="3-4">[<a href="#3-4">3.4</a>]</a> Reproduce bugs with the minimum possible scaffolding.

<a name="3-5">[<a href="#3-5">3.5</a>]</a> Tests must reproduce particular bugs, not successful usage scenarios.

<a name="3-6">[<a href="#3-6">3.6</a>]</a> Don't assert on unimportant details, don't be pedantic without reason.

<a name="3-7">[<a href="#3-7">3.7</a>]</a> Invent a DSL and write test stories using it.

<a name="3-8">[<a href="#3-8">3.8</a>]</a> Use randomizers to generate test data.

<a name="3-9">[<a href="#3-9">3.9</a>]</a> Don't help your tests; create the most inconvenient environment for them.

<a name="3-10">[<a href="#3-10">3.10</a>]</a> Don't keep temporary files next to the source code; use a temporary directory.

<a name="3-11">[<a href="#3-11">3.11</a>]</a> Don't test abstract classes.

<a name="3-12">[<a href="#3-12">3.12</a>]</a> Don't let tests log anything; keep the log empty.

<a name="3-13">[<a href="#3-13">3.13</a>]</a> Parameterize tests.

<a name="3-14">[<a href="#3-14">3.14</a>]</a> Stop tests on timeout; don't let them run forever.

<a name="3-15">[<a href="#3-15">3.15</a>]</a> Don't sleep for an arbitrary number of seconds; instead, wait for an event.

<a name="3-16">[<a href="#3-16">3.16</a>]</a> When it's necessary to simulate a hang, sleep for a billion seconds.

<a name="3-17">[<a href="#3-17">3.17</a>]</a> Let different tests test the same part of the feature code.

<a name="3-18">[<a href="#3-18">3.18</a>]</a> Test whether your objects are [thread-safe]:
  [in Java](https://www.yegor256.com/2018/03/27/how-to-test-thread-safety.html),
  [in Ruby](https://www.yegor256.com/2018/11/06/ruby-threads.html).

<a name="3-19">[<a href="#3-19">3.19</a>]</a> Let tests retry when the behavior they are testing is flaky.

<a name="3-20">[<a href="#3-20">3.20</a>]</a> Use tags to classify tests.

<a name="3-21">[<a href="#3-21">3.21</a>]</a> Let your testing framework repeat some tests to increase the chance of hitting the bug.

<a name="3-22">[<a href="#3-22">3.22</a>]</a> In tests for thread-safety, utilize all available CPUs.

<a name="3-23">[<a href="#3-23">3.23</a>]</a> Run all tests with no Internet connection; they must pass.

<a name="3-24">[<a href="#3-24">3.24</a>]</a> Don't assert on the details of errors.

<a name="3-25">[<a href="#3-25">3.25</a>]</a> Keep the scope of try/catch as small as possible.

<a name="3-26">[<a href="#3-26">3.26</a>]</a> Strictly one test per feature file:
  [jtcop](https://github.com/volodya-lombrozo/jtcop).

<a name="3-27">[<a href="#3-27">3.27</a>]</a> Don't use `verify()` from a mock framework.

<a name="3-28">[<a href="#3-28">3.28</a>]</a> Don't use [PowerMock] or similar frameworks.

<a name="3-29">[<a href="#3-29">3.29</a>]</a> In tests, don't instantiate objects or call their methods with default arguments.

<a name="3-30">[<a href="#3-30">3.30</a>]</a> Don't abbreviate; use `curl --silent` instead of `curl -s`.

<a name="3-31">[<a href="#3-31">3.31</a>]</a> Don't let feature objects do the job of tests — verify inputs and state.

<a name="3-32">[<a href="#3-32">3.32</a>]</a> Use decorating invariants to catch improper use of objects during testing.

<a name="3-33">[<a href="#3-33">3.33</a>]</a> Run tests in parallel threads:
  [threads](https://github.com/yegor256/threads).

<a name="3-34">[<a href="#3-34">3.34</a>]</a> Every fast test must take less than 100 milliseconds.

<a name="3-35">[<a href="#3-35">3.35</a>]</a> Don't mock the file system.

<a name="3-36">[<a href="#3-36">3.36</a>]</a> Make the place with temporary files accessible after the end of the test suite:
  [mktmp](https://github.com/yegor256/mktmp).

<a name="3-37">[<a href="#3-37">3.37</a>]</a> Don't assert on the content of logs generated by feature code during tests.

<a name="3-38">[<a href="#3-38">3.38</a>]</a> Use [ephemeral] TCP ports.

<a name="3-39">[<a href="#3-39">3.39</a>]</a> Don't use inheritance to reuse test tools.

<a name="3-40">[<a href="#3-40">3.40</a>]</a> Don't be scared of long test classes — they are OK.

<a name="3-41">[<a href="#3-41">3.41</a>]</a> Don't fix feature code in response to a flaky test failure.

<a name="3-42">[<a href="#3-42">3.42</a>]</a> Use [maybeslow] or a similar library to diagnose long-running tests.

<a name="3-43">[<a href="#3-43">3.43</a>]</a> Kill long-running tests on timeout.

<a name="3-44">[<a href="#3-44">3.44</a>]</a> Inline fixtures instead of keeping them in fixture files.

<a name="3-45">[<a href="#3-45">3.45</a>]</a> Don't keep large fixtures in static files; let tests generate them.

<a name="3-46">[<a href="#3-46">3.46</a>]</a> Create fixture objects that generate large fixtures at runtime.

<a name="3-47">[<a href="#3-47">3.47</a>]</a> Keep reference fixtures as static files in the repository.

<a name="3-48">[<a href="#3-48">3.48</a>]</a> Code duplication in tests is the last problem to fix.

<a name="3-49">[<a href="#3-49">3.49</a>]</a> Extract test libraries.

## Chapter 6. Fancy Tests

<a name="6-1">[<a href="#6-1">6.1</a>]</a> Test for grammar mistakes and typos:
  [languagetool](https://github.com/languagetool-org/languagetool).
  [typos-action](https://github.com/marketplace/actions/typos-action).

<a name="6-2">[<a href="#6-2">6.2</a>]</a> Employ [Property Based Testing] tools:
  [jqwik](https://github.com/jqwik-team/jqwik),
  [quickcheck](https://github.com/nick8325/quickcheck).

<a name="6-3">[<a href="#6-3">6.3</a>]</a> Use [Fuzzing] tools:
  [jqf](https://github.com/rohanpadhye/jqf),
  [oss-fuzz](https://github.com/google/oss-fuzz),
  [syzkaller](https://github.com/google/syzkaller).

<a name="6-4">[<a href="#6-4">6.4</a>]</a> Use [Mutation Testing]:
  [pitest](https://github.com/hcoles/pitest).

<a name="6-5">[<a href="#6-5">6.5</a>]</a> Check files layout during the build.

<a name="6-6">[<a href="#6-6">6.6</a>]</a> Use Load Tests:
  [jmeter](https://github.com/apache/jmeter),
  [locust](https://github.com/locustio/locust).

<a name="6-7">[<a href="#6-7">6.7</a>]</a> Use Performance Tests:
  [jmh](https://github.com/openjdk/jmh).

<a name="6-8">[<a href="#6-8">6.8</a>]</a> Benchmark new vs. previous builds:
  [jmh-benchmark-action](https://github.com/volodya-lombrozo/jmh-benchmark-action).

<a name="6-9">[<a href="#6-9">6.9</a>]</a> Use Linters:
  [eslint](https://github.com/eslint/eslint),
  [rust-clippy](https://github.com/rust-lang/rust-clippy),
  [checkstyle](https://github.com/checkstyle/checkstyle),
  [pylint](https://github.com/pylint-dev/pylint),
  [ruff](https://github.com/astral-sh/ruff).

<a name="6-10">[<a href="#6-10">6.10</a>]</a> Use [Static Analysis] at build time:
  [clang-tidy](https://clang.llvm.org/extra/clang-tidy),
  [spotbugs](https://github.com/spotbugs/spotbugs),
  [infer](https://github.com/facebook/infer).

<a name="6-11">[<a href="#6-11">6.11</a>]</a> Collect source code metrics and fail when thresholds are exceeded.

<a name="6-12">[<a href="#6-12">6.12</a>]</a> Test SQL queries:
  [pgtap](https://github.com/theory/pgtap).

<a name="6-13">[<a href="#6-13">6.13</a>]</a> Detect slowest SQL queries:
  [dexter](https://github.com/ankane/dexter).

<a name="6-14">[<a href="#6-14">6.14</a>]</a> Use Sanitizers.

<a name="6-15">[<a href="#6-15">6.15</a>]</a> Use [Dynamic Analysis] tools.

<a name="6-16">[<a href="#6-16">6.16</a>]</a> Employ Clone Detection tools:
  [simian](https://simian.quandarypeak.com/).

<a name="6-17">[<a href="#6-17">6.17</a>]</a> Use In-Browser Testing:
  [selenium](https://github.com/SeleniumHQ/selenium),
  [playwright](https://github.com/microsoft/playwright).

<a name="6-18">[<a href="#6-18">6.18</a>]</a> Use Multi-Browser Testing:
  [saucelabs](https://docs.saucelabs.com/secure-connections).

<a name="6-19">[<a href="#6-19">6.19</a>]</a> Use [Cross-Browser Testing].

<a name="6-20">[<a href="#6-20">6.20</a>]</a> Use [GUI Testing].

<a name="6-21">[<a href="#6-21">6.21</a>]</a> Use Cloud Code Analyzers:
  [SonarQube](https://www.sonarsource.com/products/sonarqube/),
  [Snyk](https://snyk.io/),
  [Codacy](https://www.codacy.com/).

<a name="6-22">[<a href="#6-22">6.22</a>]</a> Create Live Tests that verify production-ready configurations.

<a name="6-23">[<a href="#6-23">6.23</a>]</a> Use Health Checks after deployment.

<a name="6-24">[<a href="#6-24">6.24</a>]</a> Generate tests at build time:
  [randoop](https://github.com/randoop/randoop).

<a name="6-25">[<a href="#6-25">6.25</a>]</a> Employ Security Tests:
  [zaproxy](https://github.com/zaproxy/zaproxy).

<a name="6-26">[<a href="#6-26">6.26</a>]</a> Do License Compliance Testing:
  [ort](https://github.com/oss-review-toolkit/ort),
  [reuse-action](https://github.com/fsfe/reuse-action).

<a name="6-27">[<a href="#6-27">6.27</a>]</a> Detect redundant tests.

<a name="6-28">[<a href="#6-28">6.28</a>]</a> Validate architecture at build time:
  [archunit](https://github.com/TNG/ArchUnit).

[Angry Tests]: https://www.yegor256.com/angry-tests.html
[code-free]: https://www.yegor256.com/2015/05/07/ctors-must-be-code-free.html
[fake objects]: https://www.yegor256.com/2014/09/23/built-in-fake-objects.html
[PowerMock]: https://github.com/powermock/powermock
[assertDoesNotThrow]: https://docs.junit.org/5.9.0/api/org.junit.jupiter.api/org/junit/jupiter/api/Assertions.html#assertDoesNotThrow(org.junit.jupiter.api.function.Executable)
[fail]: https://docs.junit.org/5.9.0/api/org.junit.jupiter.api/org/junit/jupiter/api/Assertions.html#fail()
[one-statement]: https://www.yegor256.com/2017/05/17/single-statement-unit-tests.html
[Hamcrest]: https://hamcrest.org/
[ephemeral]: https://en.wikipedia.org/wiki/Ephemeral_port
[maybeslow]: https://github.com/yegor256/maybeslow
[Mutation Testing]: https://en.wikipedia.org/wiki/Mutation_testing
[Fuzzing]: https://en.wikipedia.org/wiki/Fuzzing
[Property Based Testing]: https://en.wikipedia.org/wiki/Property_testing
[Static Analysis]: https://en.wikipedia.org/wiki/Static_program_analysis
[Dynamic Analysis]: https://en.wikipedia.org/wiki/Dynamic_program_analysis
[Cross-Browser Testing]: https://en.wikipedia.org/wiki/Cross-browser_testing
[GUI Testing]: https://en.wikipedia.org/wiki/Graphical_user_interface_testing
[thread-safe]: https://en.wikipedia.org/wiki/Thread_safety
