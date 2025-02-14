 Simplex Algorithm Solver

A C++ implementation of the Simplex method for solving Linear Programming problems. This program efficiently finds the optimal solution to a given set of linear constraints and an objective function using the tableau method.

# Features

✅ Implements the Simplex Algorithm for Linear Programming ✅ Iterative approach to ensure optimality ✅ Detects unbounded solutions ✅ User-friendly output with formatted tableau representation ✅ Structured and modular code for easy understanding and modification

# Installation & Usage

1️⃣ Compile the Program

Ensure you have a C++ compiler installed (e.g., g++ for GCC).

g++ simplex_solver.cpp -o simplex_solver
2️⃣ Run the Program

./simplex_solver
📂 Project Structure

📁 Simplex Solver Project
│── simplex_solver.cpp   # Main program implementing the Simplex method
│── README.md            # Project documentation
📌 How It Works

1️⃣ Initial Tableau Creation: Represents the LP problem as a tableau. 2️⃣ Pivot Column Selection: Identifies the most negative coefficient in the objective function row. 3️⃣ Pivot Row Selection: Uses the minimum ratio test to determine the leaving variable. 4️⃣ Pivoting Operation: Converts the pivot element to 1 and other elements in the column to 0. 5️⃣ Iteration Until Optimality: The algorithm repeats until all coefficients in the last row are non-negative.

📊 Example Output

Initial Tableau:
     2.00     3.00     1.00     0.00     0.00   100.00 
     4.00     1.00     0.00     1.00     0.00    80.00 
     3.00     2.00     0.00     0.00     1.00    60.00 
    -3.00    -5.00     0.00     0.00     0.00     0.00 

Pivot Column: 1
Pivot Row: 1
Updated Tableau:
...

Optimal Solution:
Z = 166.67
