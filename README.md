# VHDL Counter Overflow Bug

This repository demonstrates a common error in VHDL code: an integer counter that doesn't handle overflow correctly. The `buggy_counter.vhdl` file contains the buggy code, while `fixed_counter.vhdl` provides a corrected version.

## Problem

The original counter increments indefinitely, exceeding the defined range (0 to 15). This can cause unpredictable results in simulations and hardware implementations. 

## Solution

The solution adds a check within the counter process to prevent it from exceeding the maximum value. When the counter reaches 15, it wraps back to 0, ensuring the counter behaves as expected. This type of handling is crucial for avoiding unexpected behaviors in digital systems.  This ensures that the counter behaves correctly.