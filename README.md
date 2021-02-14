# llvm-patch-stuff
Some LLVM patches.


## dereferenceable-select
Improves LLVM's ability to reason with dereferencability when it comes to select instructions, which allows passes like SROA to reason about them better. Causes functions like std::clamp to produce better IR.

## cpp-20-unevaluated-lambdas
Provides support for lambdas in an unevaluated context with C++20.