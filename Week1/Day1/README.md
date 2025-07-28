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
* Note: `mod` finds the remainder after division.
* Logical OR (`||`) returns `TRUE` (1) if either condition is `TRUE`.

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

```text
A. 1
```

---

## Summary:

The key to solving this question was to:

1. Understand how `mod` works.
2. Apply the logical OR condition correctly.
3. Plug in the values of `w = 40` and `x = 4`.
4. Evaluate each part of the condition separately and apply logical OR.
5. Follow the flow of the pseudocode accordingly.

