# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program
~~~
def pascals_triangle(n):
    for i in range(n):
       
        print(' ' * (n - i), end='')
        val = 1
        for j in range(i + 1):
            print(f'{val} ', end='')
            val = val * (i - j) // (j + 1)
        print()

rows = int(input("Enter the number of rows for Pascal's Triangle: "))
pascals_triangle(rows)

~~~
## Sample Output
<img width="1034" height="252" alt="image" src="https://github.com/user-attachments/assets/7b277c76-1682-4b44-916b-12a173a2e008" />

## Result
The Python program that generates Pascal's Triangle using numbers. The number of rows is accepted from the user is executed successfully.
