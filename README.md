## Installation

This uses Node.js with the following packages:

- `babel`
- `mocha`

You may start the project by issuing:

```
npm install
npm run test
```


## Problem

Fill in the function `detectSums` in `algo.js` that detects sums in an array, and make sure all tests pass.

##### Function definition

`detectSums` should take an array as input and detect any items in it that are the sum of another two items in the array, e.g., `[1, 2, 3] => [{ sum: 3, parts: [1, 2] } ]`.

Interesting cases:

- `[1, 2, 3] => [{ sum: 3, parts: [2, 1] }]` is valid cause parts may be returned in any order
- `[1, 2, 3] => [{ sum: 3, parts: [1, 2] }, { sum: 3, parts: [2, 1] }]` is invalid because every sum and parts must appear once in the results
- `[1, 2, 4] => []` because we can't use `2` twice as in `2 + 2 = 4`
- `[3, 0, 3] => [{ sum: 3, parts: [0,3] }]`
- `[3, 0, 2] => []` because we can't use `3` twice as in `3 + 0 = 3`



##### Details

- You may write your own tests to cover any edge cases you may think of.
- You may install and use any third party libraries. `lodash` and `faker` are already provided
- You should use ES6 syntax
- You may provide multiple versions of the function, detailing advantages/disadvantages of each


## Bonus

#### Complexity

Provide the time and memory complexity of your function.

#### Make it memory efficient

Suppose we have memory limitations, e.g. mobile, but no time limitations. Provide a memory-efficient version of the function.

#### Make it time efficient

Suppose we have unlimited memory, but we want it to be *fast*. Provide a time-efficient version of the function.
