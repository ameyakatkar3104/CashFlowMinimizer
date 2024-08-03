# CashFlowMinimizer

## Objective: 
The Cash Flow Minimizer is designed to optimize the settlement of debts among a group of individuals. Given a set of transactions, the goal is to minimize the total number of transactions required to settle all debts using the backtracking algorithm.

## Key Features:

1. **Data Structures:**
    - Transactions Representation:
      - A 2D array transactions[N][N] where transactions[i][j] represents the amount that person i owes to person j.
    - Net Amount Array:
      - An array netAmount[N] where netAmount[i] represents the net amount to be settled by person i. A positive value indicates a net creditor, and a negative value indicates a net debtor.

3. **Backtracking Algorithm:**

    - The backtracking algorithm is used to explore all possible ways to settle debts and choose the one that results in the minimum number of transactions.
    - It recursively tries to minimize the cash flow by settling debts between creditors and debtors in different orders.
3. **Functions:**

    - Calculate Net Amount:
      - Compute the net amount to be paid/received by each individual.
    - Minimize Cash Flow:
      - Recursively minimize the number of transactions by settling debts using the backtracking approach.
    - Utility Functions:
      - Find the person with the maximum credit (getMax()) and the person with the maximum debt (getMin()).
      - 
## Implementation Details:
1. **Calculate Net Amount:**

    - Iterate through the transactions array to compute the net amount for each individual.
2. **Minimize Cash Flow:**

    - Find the person with maximum credit and maximum debt.
    - Settle the maximum possible amount between these two individuals.
    - Recursively call the function to settle the remaining amounts.
3. **Utility Functions:**

    - getMax(): Returns the index of the person with the maximum credit.
    - getMin(): Returns the index of the person with the maximum debt.
