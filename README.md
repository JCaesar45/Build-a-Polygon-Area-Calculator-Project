```markdown
# Polygon Area Calculator

A Python project that demonstrates object-oriented programming by creating `Rectangle` and `Square` classes to calculate areas, perimeters, diagonals, and visualize shapes.

---

## Features

- **Rectangle Class**
  - Initialize with width and height.
  - Set and get dimensions.
  - Calculate area, perimeter, and diagonal length.
  - Generate a visual ASCII representation.
  - Determine how many of another shape fit inside.
  - String representation for easy debugging.

- **Square Class (Subclass of Rectangle)**
  - Initialize with a single side length.
  - Set and get side length.
  - Automatically update both width and height when side is changed.
  - String representation for clarity.

---

## Usage

```python
from your_module_name import Rectangle, Square

# Create a rectangle
rect = Rectangle(10, 5)
print(rect.get_area())            # Output: 50
rect.set_height(3)
print(rect.get_perimeter())       # Output: 16
print(rect)                       # Output: Rectangle(width=10, height=3)
print(rect.get_picture())

# Create a square
sq = Square(9)
print(sq.get_area())              # Output: 81
sq.set_side(4)
print(sq.get_diagonal())          # Output: 5.656854249492381
print(sq)                       # Output: Square(side=4)
print(sq.get_picture())

# Fit shapes inside each other
rect.set_height(8)
rect.set_width(16)
print(rect.get_amount_inside(sq))  # Output: 8
``

---

## Example Output

``
50
26
Rectangle(width=10, height=3)
**********
**********
**********

81
5.656854249492381
Square(side=4)
****
****
****
****

8
``

---

## Installation

- Save the classes in a Python file, e.g., `shapes.py`.
- Import and use in your scripts.

---

## License

This project is for educational purposes and is provided as-is.
``

---

### Notes:
- Replace `your_module_name` with the actual filename if you save the classes in a file (e.g., `shapes.py`).
- You can expand the README with sections like "Contributing", "Authors", or "Acknowledgments" depending on your needs.
