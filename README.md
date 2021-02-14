# llvm-patch-stuff
Some LLVM patches.


## dereferenceable-select
Improves LLVM's ability to reason with dereferencability when it comes to select instructions, which improves passes like SROA. 
Causes functions like std::clamp to produce better (though still sub-optimal) IR.

## cpp-20-unevaluated-lambdas
Provides support for lambdas in an unevaluated context with C++20.
