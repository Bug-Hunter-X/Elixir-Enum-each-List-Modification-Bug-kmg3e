# Elixir Enum.each List Modification

This example demonstrates a common misconception when working with lists and `Enum.each` in Elixir.  Attempting to modify the list directly inside the `Enum.each` loop does not alter the original list. This is because Elixir uses immutable data structures.  The provided solution showcases a more functional approach to achieve the desired outcome.

**Problem:**  The code intends to remove the element 3 from the list, but the `List.delete` function creates a new list without affecting the original one.

**Solution:**  The solution uses `Enum.filter` to create a new list containing only the elements that are not equal to 3, effectively removing it.