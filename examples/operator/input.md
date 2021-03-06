In Rust, many of the operators can be overloaded via traits. This is possible
because operators are just sugar for method calls. For example, `a + b`
desugars to `a.add(&b)`. This `add()` method is part of the `Add` trait, hence
any implementor of the `Add` trait will be able to use the `+` operator.

{operator.play}

Here is a [list](http://static.rust-lang.org/doc/master/core/ops/index.html) of
the traits that overload operators.
