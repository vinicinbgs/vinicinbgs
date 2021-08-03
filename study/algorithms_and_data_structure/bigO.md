# Big O

#### What does better mean?
- Faster? (you can add timers for when function init and finish to measure timing)
- Less memory-intensive?
- More readable?

### Definition
1. f(n) could be linear (f(n) = n)
2. f(n) could be quadratic (f(n) = n²)
3. f(n) could be constant (f(n) = 1)
4. f(n) could be some entirely different

### Shorthands
1. Arithmetic operations are constant
2. Variable assignment is constant
3. Acessing elements in an array (by index) or object (by key) is constant
4. In a loop, the complexity is the length of the loop times the complexity of whatever happens inside of the loop

# Space Complexity in JS
- Most primitives (booleans, numbers, undefined, null) are constant space
- String require O(n) space (where n is the string length)
- References types are generally O(n), where n is the length (for arrays) or the number of keys (for objects)
- O(n) space!

# Logarithms
- log<sub>2</sub>(8) = 3 --> 2³ = 8
- log<sub>2</sub>(value) = exponent --> 2^exponent = value


### Time Complexity (faster to slower)
1. O(1)
2. O(log n)
3. O(n)
4. O(nlog n)
5. O(n²)
---
#### Who cares?
1. Searching algorithms have logarithmic time complexity
2. Efficient sorting algorithms involve logarithms
3. Recursion sometimes involves logarithmic space complexity