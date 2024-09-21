

### **Error-Based Questions**

1. **Question:**
    ```cpp
    int a = 5;
    int b;
    cout << a + b;
    ```
    **Error Type:**  
    **Explanation:**  
    - **Problem:** The variable `b` is declared but not initialized.
    - **Error:** This will result in **undefined behavior** since `b` is used without being assigned a value.
    - **Correction:** Initialize `b` before using it.

---

2. **Question:**
    ```cpp
    int x = 10;
    if (x = 5) {
        cout << "Equal";
    }
    ```
    **Error Type:**  
    **Explanation:**  
    - **Problem:** The condition in the `if` statement uses a single equals `=` instead of a double equals `==`.
    - **Error:** This will cause **logical error** because `x` will be assigned the value `5`, and the condition will always evaluate to true.
    - **Correction:** Use `==` for comparison, like `if (x == 5)`.

---

3. **Question:**
    ```cpp
    cout << "Hello";
    int a = 5;
    ```
    **Error Type:**  
    **Explanation:**  
    - **Problem:** Missing `#include <iostream>` at the top of the program.
    - **Error:** This will cause a **compile-time error** as the `cout` function is undefined without including the proper header file.
    - **Correction:** Add `#include <iostream>` at the beginning of the program.

---

4. **Question:**
    ```cpp
    int arr[5] = {1, 2, 3, 4, 5};
    cout << arr[5];
    ```
    **Error Type:**  
    **Explanation:**  
    - **Problem:** Accessing the array index `arr[5]`, but valid indices are `0` to `4`.
    - **Error:** This causes **out-of-bounds access**, which could lead to a **runtime error** or undefined behavior.
    - **Correction:** Ensure array index stays within valid bounds, e.g., `arr[4]`.

---

5. **Question:**
    ```cpp
    int a = 10 / 0;
    cout << a;
    ```
    **Error Type:**  
    **Explanation:**  
    - **Problem:** Division by zero.
    - **Error:** This will result in a **runtime error** because division by zero is undefined in arithmetic.
    - **Correction:** Ensure the divisor is never zero before performing division.

---

6. **Question:**
    ```cpp
    int a = 5;
    float b = 2.5;
    cout << a + b;
    ```
    **Error Type:**  
    **Explanation:**  
    - **Problem:** Mixing integer and float types.
    - **Error:** Although this won't cause a compile-time error, it may cause **precision loss** during the addition due to implicit type conversion.
    - **Correction:** Explicitly cast the variables if necessary, or perform operations with consistent types.

---

7. **Question:**
    ```cpp
    int arr[3] = {1, 2, 3};
    for (int i = 0; i <= 3; i++) {
        cout << arr[i] << " ";
    }
    ```
    **Error Type:**  
    **Explanation:**  
    - **Problem:** The loop iterates up to `i = 3`, which is out of bounds for the array of size 3.
    - **Error:** This results in an **out-of-bounds access** leading to undefined behavior or a runtime error.
    - **Correction:** Change the loop condition to `i < 3`.

---

8. **Question:**
    ```cpp
    void foo() {
        int a = 10;
    }
    cout << a;
    ```
    **Error Type:**  
    **Explanation:**  
    - **Problem:** The variable `a` is declared inside the function `foo()`, so it is not accessible outside the function.
    - **Error:** This will cause a **scope error** as `a` is out of scope when accessed outside the function.
    - **Correction:** Declare `a` outside the function if it needs to be accessed globally.

---

9. **Question:**
    ```cpp
    int a;
    cout << a;
    ```
    **Error Type:**  
    **Explanation:**  
    - **Problem:** The variable `a` is declared but not initialized.
    - **Error:** This will cause **undefined behavior** because the value of `a` is not set before being used.
    - **Correction:** Initialize `a` before using it, e.g., `int a = 0;`.

---

10. **Question:**
    ```cpp
    int a = 5;
    if (a > 0);
        cout << "Positive";
    ```
    **Error Type:**  
    **Explanation:**  
    - **Problem:** The semicolon after the `if` condition ends the `if` statement.
    - **Error:** This causes the **logical error** where the `cout` statement always executes, regardless of the condition.
    - **Correction:** Remove the semicolon after the `if` condition.

---

11. **Question:**
    ```cpp
    int *p;
    *p = 10;
    cout << *p;
    ```
    **Error Type:**  
    **Explanation:**  
    - **Problem:** The pointer `p` is declared but not initialized.
    - **Error:** Dereferencing an uninitialized pointer leads to a **segmentation fault** or undefined behavior.
    - **Correction:** Initialize `p` to point to a valid memory address before dereferencing it.

---

12. **Question:**
    ```cpp
    int i = 0;
    while (i < 5) {
    cout << i;
    ```
    **Error Type:**  
    **Explanation:**  
    - **Problem:** The `while` loop is missing a closing curly brace.
    - **Error:** This will cause a **syntax error** during compilation because the loop is incomplete.
    - **Correction:** Add the closing curly brace to properly terminate the loop.

---

13. **Question:**
    ```cpp
    int main() {
        cout << "Hello";
    }
    ```
    **Error Type:**  
    **Explanation:**  
    - **Problem:** The `main()` function is declared to return an `int` but does not include a return statement.
    - **Error:** This will cause a **compile-time warning** or error depending on the compiler, expecting a return value.
    - **Correction:** Add a `return 0;` statement at the end of `main()`.

---

14. **Question:**
    ```cpp
    int a[3] = {1, 2};
    cout << a[2];
    ```
    **Error Type:**  
    **Explanation:**  
    - **Problem:** The array `a` has a size of 3 but only two elements are initialized.
    - **Error:** The uninitialized element `a[2]` may contain **garbage value**, leading to unexpected results.
    - **Correction:** Initialize all elements in the array, e.g., `int a[3] = {1, 2, 0};`.

---

15. **Question:**
    ```cpp
    int a = "5";
    cout << a;
    ```
    **Error Type:**  
    **Explanation:**  
    - **Problem:** Attempting to assign a string literal `"5"` to an integer variable `a`.
    - **Error:** This will cause a **type mismatch error** because a string cannot be assigned to an integer.
    - **Correction:** Assign an integer value, e.g., `int a = 5;`.
