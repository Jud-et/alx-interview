# Making Change

Welcome to the **Making Change** project! This classic problem tests your skills in algorithms by finding the minimum number of coins needed to meet a given total. It's a fun and practical challenge for algorithm enthusiasts. 💡

---

## **Problem Statement**

Given a pile of coins with different values, determine the fewest number of coins needed to make a specific total.

### **Prototype**
```python
def makeChange(coins, total):
```

### **Parameters**
- **`coins`**: A list of integers representing the values of available coins.
- **`total`**: An integer representing the target amount to achieve.

### **Returns**
- **Integer**: The minimum number of coins needed to meet the total.
- **`-1`**: If the total cannot be met with the available coins.

---

## **Requirements**
- Return `0` if the total is `0` or less.
- Assume you have an infinite number of each coin denomination.
- The algorithm should prioritize efficiency.

---

## **Example Usage**

```bash
$ cat 0-main.py
#!/usr/bin/python3
makeChange = __import__('0-making_change').makeChange

print(makeChange([1, 2, 25], 37))  # Expected output: 7
print(makeChange([1256, 54, 48, 16, 102], 1453))  # Expected output: -1
```

Run the script:
```bash
$ ./0-main.py
7
-1
```

---

## **Algorithmic Approach**

1. **Sort Coins**: Coins are sorted in descending order to use the largest denominations first (greedy algorithm).
2. **Calculate Count**: For each coin, calculate how many can fit into the remaining total.
3. **Check Remainder**: If the total reaches `0`, return the coin count. If not, return `-1`.

---

## **Code Overview**

### **`0-making_change.py`**
This file contains the core function:

```python
#!/usr/bin/python3
def makeChange(coins, total):
    if total <= 0:
        return 0

    coins.sort(reverse=True)
    num_coins = 0

    for coin in coins:
        if total == 0:
            break
        num_coins += total // coin
        total %= coin

    return num_coins if total == 0 else -1
```

---

## **What I Learned**

- **Greedy Algorithm**: Leveraging sorted inputs for optimization.
- **Edge Case Handling**: Managing scenarios where the total is unreachable.
- **Algorithm Efficiency**: Writing code that balances clarity and performance.

---

## **How to Run the Code**
1. Clone this repository.
2. Navigate to the project directory.
3. Run the test script:
   ```bash
   ./0-main.py
   ```

---

## **Author**
Developed with 💻 and 💡 by a dedicated backend engineer.
Judith

Enjoy coding and solving challenges! 🚀

