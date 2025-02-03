#  0x09. Island Perimeter
## The Domains/Concepts covered in this project: `Python` `OOP`

In this project I implemented the `island_perimeter(grid)` function in Python to calculate the perimeter of an island in a grid. I learned how to traverse a 2D list, identify land and water zones, and apply boundary conditions to determine the correct perimeter without using external python modules.

## Tasks :page_with_curl:

**0x09. Island Perimeter**

**Technical interview preparation:**

  * You are not allowed to google anything
  * Whiteboard first

Create a function `def island_perimeter(grid):` that returns the perimeter of the island described in `grid`:

  * `grid` is a list of list of integers:
    * 0 represents a water zone
    * 1 represents a land zone
    * One cell is a square with side length 1
    * Grid cells are connected horizontally/vertically (not diagonally).
    * Grid is rectangular, width and height don’t exceed 100
  * Grid is completely surrounded by water, and there is one island (or nothing).
  * The island doesn’t have “lakes” (water inside that isn’t connected to the water around the island).

Requirements:

  * First line contains `#!/usr/bin/python3`
  * You are not allowed to import any module
  * Module and function must be documented

```
guillaume@ubuntu:~/0x1C$ cat 5-main.py
#!/usr/bin/python3
"""
5-main
"""
island_perimeter = __import__('5-island_perimeter').island_perimeter

if __name__ == "__main__":
    grid = [
        [0, 0, 0, 0, 0, 0],
        [0, 1, 0, 0, 0, 0],
        [0, 1, 0, 0, 0, 0],
        [0, 1, 1, 1, 0, 0],
        [0, 0, 0, 0, 0, 0]
    ]
    print(island_perimeter(grid))

guillaume@ubuntu:~/0x1C$ 
guillaume@ubuntu:~/0x1C$ ./5-main.py
12
guillaume@ubuntu:~/0x1C$ 
```

  * [0-island_perimeter.py](./0-island_perimeter.py)
