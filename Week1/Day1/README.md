# Week1 - Day 1

## Problems
- Problem 1

What will be the output of the following pseudocode of fun for w = 40 and x = 4?

```pseudo
1. void fun( Integer w, Integer x )
2.   Integer y
3.   Set y = 0
4.   if (x mod w EQUALS 0 || w mod x EQUALS 0)
5.     y = y + 1
6.   Else
7.     y = y + 10
8.   End if
9.   Print y
10. End function fun()
```

## Given:

* `w = 40`, `x = 4`

## Step-by-Step Evaluation:

### Step 1: Initialize y

```pseudo
y = 0
```

### Step 2: Evaluate the condition

```pseudo
x mod w = 4 mod 40 = 4
w mod x = 40 mod 4 = 0
```

Now evaluate:

```pseudo
(4 mod 40 == 0) || (40 mod 4 == 0)
=> (4 == 0) || (0 == 0)
=> FALSE || TRUE
=> TRUE
```

### Step 3: Condition is TRUE

So the control goes to:

```pseudo
y = y + 1 = 0 + 1 = 1
```

### Step 4: Print y

```pseudo
Output = 1
```

## Final Answer:

A. 1

## Summary:

The key to solving this question was to:

1. Understand how `mod` works.
2. Apply the logical OR condition correctly.
3. Plug in the values of `w = 40` and `x = 4`.
4. Evaluate each part of the condition separately and apply logical OR.
5. Follow the flow of the pseudocode accordingly.

- Problem 2

## 📄 Question:
Consider the pseudocode mentioned below. For how many times will the `while` loop be executed?

```plaintext
1.  Integer a  
2.  Set a = 1  
3.  while (a < 5)  
4.      a = a + 2  
5.  end while  
6.  Print a  
```

## 🔍 Options:
- A. 1  
- B. 4  
- C. 2  
- D. 3  

---

## ✅ Correct Answer: **C. 2**

---

## 🧠 Approach:

We need to count how many times the condition `a < 5` is true, and how many times the loop body gets executed.

### Initial value:
- `a = 1`

### Loop condition:
- `while (a < 5)`

Each time the loop runs:
- We increment `a` by 2: `a = a + 2`

---

## 🧾 Conclusion:
The loop is executed **2 times** before the condition becomes false.

So, the correct option is:

### ✅ **C. 2**


- Problem 3

## 📄 Question:
What will be the output of the following pseudocode for `a = 8`, `b = 8`?

```plaintext
1.  Integer funn(Integer a, Integer b)
2.      if (a && b && a + b > 0)
3.          return a + funn(a - 2, b - 2) + b
4.      End if
5.      return a ^ b
6.  End function funn()
```

### Notes:
- `&&` is the logical AND operator — returns true (1) if all conditions are true.
- `^` is the bitwise XOR operator.

---

## 🔍 Options:
- A. 39  
- B. 46  
- C. 48  
- D. 40  

---

## 🧠 Approach:

We analyze the recursion with `a = 8`, `b = 8`.

### Base Condition:
```plaintext
if (a && b && a + b > 0)
```
This means recursion will continue **as long as both `a` and `b` are non-zero and their sum is > 0**.

Otherwise, it returns `a ^ b`.

---

## 🧾 Dry Run (Recursive Tree):

Let's evaluate `funn(8, 8)`:

```plaintext
funn(8,8) = 8 + funn(6,6) + 8
funn(6,6) = 6 + funn(4,4) + 6
funn(4,4) = 4 + funn(2,2) + 4
funn(2,2) = 2 + funn(0,0) + 2
funn(0,0) = 0 ^ 0 = 0
```

### Now unwind the recursion:

```plaintext
funn(2,2) = 2 + 0 + 2 = 4
funn(4,4) = 4 + 4 + 4 = 12
funn(6,6) = 6 + 12 + 6 = 24
funn(8,8) = 8 + 24 + 8 = 40
```

---

## 🖨️ Final Output:
- `funn(8, 8)` returns **40**

---

## ✅ Correct Answer:
### **D. 40**

-Problem 4


## 📄 Question:
What will be the output of the following pseudocode?

```plaintext
1.  Integer a, b
2.  Set a = 3, b = 3
3.  a = b
4.  if(1 ^ 1)
5.      a = 1
6.  Else
7.      b = 2
8.  End if
9.  Print a + b
```

---

## 🔍 Options:
- A. 16  
- B. 1  
- C. 5  
- D. 6  

---

## 🧠 Key Concepts:

- `^` is the **bitwise XOR** operator.
  - `1 ^ 1 = 0` (since both bits are the same, XOR returns 0)
- `if(x)` executes when `x` is non-zero.
  - Since `1 ^ 1 = 0`, the `if` condition fails → `else` block runs.

---

## 🧾 Dry Run:

1. `a = 3`, `b = 3`
2. `a = b` → `a = 3`
3. Evaluate `if(1 ^ 1)` → `0` → **false**
4. Execute `else`: `b = 2`
5. Final values:
   - `a = 3`
   - `b = 2`
6. Output: `a + b = 3 + 2 = 5`

---

## ✅ Correct Answer:
### **C. 5**
