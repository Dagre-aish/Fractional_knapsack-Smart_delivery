

# Fractional Knapsack – Smart Delivery Planning

A menu-driven **C program** that implements the **Fractional Knapsack Greedy Algorithm** using a real-world smart delivery planning scenario.

The program selects packages for a delivery vehicle with limited capacity while maximizing the total value of the delivered packages. Since packages can be divided, the **Fractional Knapsack** approach is used.

## Features

- Enter package details
- Set maximum vehicle capacity
- Display package information
- Calculate Value/Weight ratio
- Sort packages based on their ratio
- Select complete or fractional packages
- Calculate maximum possible value
- Display selected packages and fractions taken
- Display total weight used
- Interactive menu-driven interface

## Algorithm Used

### Fractional Knapsack

The program uses a **Greedy Algorithm**.

For every package, the following ratio is calculated:

```text
Value/Weight Ratio = Value ÷ Weight
```

Packages are then sorted in **decreasing order of their Value/Weight ratio**.

The vehicle is filled according to the following strategy:

1. Select the package with the highest ratio.
2. If the complete package fits, take the entire package.
3. If it does not fit, take only the required fraction.
4. Continue until the vehicle capacity is full.

This approach gives the **optimal solution for the Fractional Knapsack problem**.

## Program Flow

```text
Enter Package Details
        ↓
Calculate Value/Weight Ratio
        ↓
Sort Packages by Ratio
        ↓
Apply Greedy Algorithm
        ↓
Select Full/Fractional Packages
        ↓
Calculate Maximum Value
        ↓
Display Result
```

## Technologies Used

- **Programming Language:** C
- **Algorithm:** Greedy Algorithm
- **Problem:** Fractional Knapsack
- **Libraries:** `stdio.h`, `stdlib.h`
- **Sorting:** `qsort()`

## How to Run

### Clone the Repository

```bash
git clone https://github.com/Dagre-aish/AOA_PBLE.git
cd AOA_PBLE
```

### Compile the Program

Using GCC:

```bash
gcc PBLE.c -o PBLE
```

### Run

**Windows:**

```bash
PBLE.exe
```

**Linux/macOS:**

```bash
./PBLE
```

## Menu Options

The program provides the following options:

```text
1. Enter Package Details
2. Display Package Details
3. Calculate Value/Weight Ratio
4. Sort Packages by Ratio
5. Find Maximum Value
6. Display Selected Packages
7. Exit
```

## Complexity Analysis

Let **n** be the number of packages.

| Operation | Time Complexity |
|---|---:|
| Enter package details | O(n) |
| Calculate ratios | O(n) |
| Sort packages | O(n log n) |
| Select packages | O(n) |
| Overall | O(n log n) |

### Space Complexity

```text
O(n)
```

The program stores information for all packages in an array.

## Project Structure

```text
fractional-knapsack-smart-delivery/
│
├── PBLE.c
└── README.md
```

## Learning Objectives

This project demonstrates:

- Greedy algorithm implementation
- Fractional Knapsack problem solving
- Structures in C
- Arrays and functions
- Sorting using `qsort()`
- Value-to-weight ratio calculation
- Fractional selection of items
- Menu-driven programming
- Time and space complexity analysis

## Real-World Application

The algorithm can be applied to **delivery and logistics planning**.

When a delivery vehicle has limited carrying capacity, packages can be prioritized according to their **value per unit of weight**. The vehicle can carry the most valuable combination of packages while making efficient use of its available capacity.

## Author

**Aishwarya Dagre**

GitHub: [Dagre-aish](https://github.com/Dagre-aish)
