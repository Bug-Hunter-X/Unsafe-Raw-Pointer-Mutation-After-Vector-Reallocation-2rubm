# Rust Bug: Unsafe Raw Pointer Mutation

This repository demonstrates a common error in Rust involving the use of raw pointers with vectors.  Modifying a vector through a raw pointer after the vector's internal capacity has been exceeded can result in undefined behavior, memory corruption, or program crashes. The example code shows this error and its solution.

## Bug Description

The `bug.rs` file showcases the incorrect usage of a raw pointer to modify a vector after its capacity is exceeded. This can lead to unpredictable results and is a significant risk.

## Solution

The `bugSolution.rs` file provides a safer alternative, avoiding raw pointers and using Rust's built-in methods for vector manipulation, ensuring memory safety.