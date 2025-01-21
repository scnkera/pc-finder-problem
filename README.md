# Finder Problem

Problem belonging to the post-classroom Mock Interview Question Repository.

## Problem Statement

We are interested in writing a function to compare a given search value to a binary search tree. Specifically, we want to know whether the search value is smaller, bigger, or spanned by the tree.

Our function should accept two arguments, the root of a tree, and a search value to compare against it. The output of our functions should be as follows:

- If the value is smaller than the smallest element in the tree, our function should return `"smaller"`
- If the value is larger than the largest element in the tree, our function should return `"bigger"`
- If the value is between the smallest and largest element (inclusive) in the tree, our function should return `"spanned"`

For example, given this tree:

```
           6
         /   \
        /     \
       3       8
      / \       \
     1   5       9
```

If the search value was 10, our function should return `"bigger"`, because 10 is greater than 9.

If the search value was 0, our function should return `"smaller"`, because 0 is less than 1.

If the search value was 4, our function should return `"spanned"`, because 4 is between 1 and 9 (inclusive).

If the search value was 1, our function should return `"spanned"`, because 1 is between 1 and 9 (inclusive).

## Examples

### Example 1

For the following tree

```
           6
         /   \
        /     \
       3       8
      / \       \
     1   5       9
```

Any value below 1 should return `"smaller"`, any value above 9 should return `"bigger"`, and any value between 1 and 9 (inclusive) should return `"spanned"`.

### Example 2

For the following tree

```
           5
         /   \
        /     \
       3       7
      /         \
     1           8
    /
   0
```

Any value below 0 should return `"smaller"`, any value above 8 should return `"bigger"`, and any value between 0 and 8 (inclusive) should return `"spanned"`.
