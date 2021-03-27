# reproduce-mockk-slow-down

```
% ./gradlew clean compileTestKotlin

> Task :compileTestKotlin FAILED
e: /Users/orange/reproduce-mockk-slow-down/src/test/kotlin/LibraryTest.kt: (3, 42): Too many arguments for public constructor Foo(p1: Int, p2: Int, p3: Int, p4: Int, p5: Int, p6: Int, p7: Int, p8: Int, p9: Int) defined in Foo
e: /Users/orange/reproduce-mockk-slow-down/src/test/kotlin/LibraryTest.kt: (3, 46): Too many arguments for public constructor Foo(p1: Int, p2: Int, p3: Int, p4: Int, p5: Int, p6: Int, p7: Int, p8: Int, p9: Int) defined in Foo

FAILURE: Build failed with an exception.

* What went wrong:
Execution failed for task ':compileTestKotlin'.
> Compilation error. See log for more details

* Try:
Run with --stacktrace option to get the stack trace. Run with --info or --debug option to get more log output. Run with --scan to get full insights.

* Get more help at https://help.gradle.org

BUILD FAILED in 1m 20s
3 actionable tasks: 3 executed
```

Note that the build failure is expected, but taking `1m 20s` is not expected.

