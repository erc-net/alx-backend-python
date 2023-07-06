![](https://i.ytimg.com/vi/H_LfhdFzNcE/maxresdefault.jpg)

Variable annotations in Python allow you to provide type hints for variables. They were introduced in Python 3.6 as part of the type hinting feature, which is a way to add type information to your code for better static analysis and documentation purposes.
def factorial(n: int) -> int:
  """
  Calculates the factorial of a number.

  Args:
    n: The number to calculate the factorial of.

  Returns:
    The factorial of n.
  """

  if n < 0:
    raise ValueError("n must be non-negative")

  if n == 0:
    return 1

  return n * factorial(n - 1)


if __name__ == "__main__":
  print(factorial(5))

