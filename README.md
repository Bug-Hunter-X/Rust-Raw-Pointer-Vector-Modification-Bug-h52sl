# Rust Raw Pointer Vector Modification Bug

This repository demonstrates a common error in Rust involving unsafe code and vector manipulation.  Modifying a vector through a raw pointer after changing the vector's size or capacity leads to undefined behavior.  The provided solution shows the safe and correct way to achieve the same goal.

## Bug Description
The bug stems from modifying a vector using a raw pointer after altering the vector's contents or size. This breaks Rust's memory safety guarantees and can lead to crashes, data corruption, or unpredictable behavior.

## Solution
The solution avoids the use of raw pointers and instead utilizes safe methods provided by the Rust standard library to modify vector elements.