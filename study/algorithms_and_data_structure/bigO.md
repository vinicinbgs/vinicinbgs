# Big O Notation

#### What does better mean?
- Faster? (you can add timers for when function init and finish to measure timing)
- Less memory-intensive?
- More readable?

### Definition
1. f<sub>(n)</sub> could be linear (f<sub>(n)</sub> = n)
2. f<sub>(n)</sub> could be quadratic (f<sub>(n)</sub> = n²)
3. f<sub>(n)</sub> could be constant (f<sub>(n)</sub> = 1)
4. f<sub>(n)</sub> could be some entirely different

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

---
#### Big O Array's
1. Insertion - it's depend
2. Removal - it's depend
3. Searching - O<sub>(n)</sub>
4. Access - O<sub>(1)</sub>

e.g: push & pop is more fast than shift & unshift

- push = O<sub>(1)</sub>
- pop = O<sub>(1)</sub>
- shift = O<sub>(n)</sub>
- unshift = O<sub>(n)</sub>
- concat = O<sub>(n)</sub>
- slice = O<sub>(n)</sub>
- splice = O<sub>(n)</sub>
- sort = O<sub>(n * log n)</sub>
- forEach/map/filter/reduce/etc. = O<sub>(n)</sub>