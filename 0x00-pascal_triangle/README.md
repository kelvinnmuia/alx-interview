#  0x00. Pascal's Triangle
## The Domains/Concepts covered in this project: `Python` `OOP`

This project introduced me to generating Pascal’s Triangle in Python, a classic mathematical problem often used in technical interviews. I learned how to implement algorithms to construct the triangle efficiently using iterative and recursive approaches while understanding its combinatorial properties.

## Tasks :page_with_curl:

**Technical interview preparation:**

  * You are not allowed to google anything
  * Whiteboard first

Create a function `def pascal_triangle(n):` that returns a list of lists of integers representing the Pascal’s triangle of `n`:

  * Returns an empty list if `n <= 0`
  * You can assume `n` will be always an integer
  * You are not allowed to import any module

```
guillaume@ubuntu:~/0x0B$ cat 12-main.py
#!/usr/bin/python3
"""
12-main
"""
pascal_triangle = __import__('12-pascal_triangle').pascal_triangle

def print_triangle(triangle):
    """
    Print the triangle
    """
    for row in triangle:
        print("[{}]".format(",".join([str(x) for x in row])))


if __name__ == "__main__":
    print_triangle(pascal_triangle(5))

guillaume@ubuntu:~/0x0B$ 
guillaume@ubuntu:~/0x0B$ ./12-main.py
[1]
[1,1]
[1,2,1]
[1,3,3,1]
[1,4,6,4,1]
guillaume@ubuntu:~/0x0B$ 
```

  * [0-pascal_triangle.py](./0-pascal_triangle.py)
