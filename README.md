# Red-Black Tree

This is a Python implementation of a Red-Black tree, a type of self-balancing binary search tree. Red-Black trees maintain their balance during insertion and deletion operations by enforcing a set of properties that ensure the tree remains balanced.

## Table of Contents

- [Introduction](#red-black-tree)
- [Usage](#usage)
- [Methods](#methods)
- [Example](#example)
- [Contributing](#contributing)
- [License](#license)

## Usage

To use this Red-Black tree implementation, create an instance of the `RBTree` class and use the `insert` method to insert elements. The tree will automatically maintain its balance after each insertion.

```python
# Create a Red-Black tree
rb_tree = RBTree()

# Insert elements into the tree
rb_tree.insert(RBNode(5, 1))
rb_tree.insert(RBNode(10, 1))
rb_tree.insert(RBNode(3, 1))
```

## Methods

### `insert(node)`

Inserts a new node into the Red-Black tree while maintaining its balance.

### `delete(node)`

Deletes a node from the Red-Black tree while maintaining its balance.

### `inorder()`

Performs an in-order traversal of the tree and returns a list of nodes with their values and colors.

## Example

```python
# Create a Red-Black tree
rb_tree = RBTree()

# Insert elements into the tree
children = [11, 2, 14, 1, 7, 15, 5, 8, 4]
for child in children:
    node = RBNode(child, 1)
    rb_tree.insert(node)

# Perform in-order traversal
result = rb_tree.inorder()
print("In-order traversal:", result)
```

## Contributing

If you'd like to contribute to this Red-Black tree implementation, feel free to submit a pull request. Issues and feature requests are also welcome.

## License

This Red-Black tree implementation is released under the [MIT License](LICENSE).
