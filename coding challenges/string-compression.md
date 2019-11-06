# String compression

Let's write a function that will receive a string as parameter. It should return a compressed version of the string, but only if the compressed string is shorter than the original.

For example, for the string `'aabccccccaaa'` it should return `'a2b1c5a3'`.
For the string `'abc'` it should still return `'abc'` as it is shorter than the compressed version `'a1b1c1'`.
