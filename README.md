# TypeScript Type Error: String in Arithmetic Operation

This example demonstrates a common TypeScript type error that occurs when performing arithmetic operations with strings instead of numbers.  The compiler's type checking helps prevent runtime errors by identifying this issue at compile time.

**Bug:**
The code attempts to add a number to a string and subtract a string from a number.  TypeScript's type system correctly identifies this as a type error because these operations are not defined for strings and numbers without explicit type coercion.

**Solution:**
Ensure that all operands in arithmetic operations are of the numeric type (number).  Explicit type conversion can be used if necessary, but this should be done with caution to avoid unexpected behavior.

**How to Reproduce:**
1.  Save the code in `bug.ts`.
2.  Compile the TypeScript code using the TypeScript compiler (tsc).
3.  Observe the type errors reported by the compiler.