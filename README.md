# Python Classes - Square

## Task 0: Define a Square

In this task, we created a class `Square` that defines a square by its size.

### Requirements:

- Private instance attribute: `size`
- Constructor accepts `size` parameter.
- No type or value validation is done in this task.
- You are not allowed to import any module.

### Why is `size` a private attribute?

The size of a square is crucial for computations like area or perimeter. Making it private allows the class to control access and modification, ensuring proper validation can be added in future tasks.

### Example:

```python
from 0-square import Square

my_square = Square(3)
print(type(my_square))
print(my_square.__dict__)

# Accessing private attribute directly will fail
try:
    print(my_square.size)
except Exception as e:
    print(e)

try:
    print(my_square.__size)
except Exception as e:
    print(e)
