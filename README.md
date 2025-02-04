# JavaScript Loose Equality and Null Handling

This repository demonstrates a common JavaScript bug related to loose equality (`==`) and null values.  Loose equality can lead to unexpected type coercion, causing errors that are difficult to track down. This example showcases a secure way to deal with null inputs to prevent such problems.

## Bug Description
The original code uses loose equality (`==`) to check for null values. This can cause unexpected behavior due to JavaScript's type coercion rules. For instance, `0 == false` evaluates to `true`, and `null == undefined` evaluates to `true`, potentially leading to incorrect logic.

## Solution
The provided solution uses strict equality (`===`) to accurately check for null values. Strict equality avoids type coercion and ensures that the comparison is only true if the values are exactly the same type and value.  Additionally, explicit null checks are added at the start of the function to provide clear and reliable null handling.