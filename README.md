# 4-queen-problem
The 4-Queen Problem is a combinatorial puzzle to place 4 queens on a 4x4 chessboard such that no two queens threaten each other. This repository provides a backtracking-based solution to find all valid configurations efficiently.

Step-by-Step Solution for the 4-Queen Problem
Step 1: Start with the first queen
1. Place the first queen in the first row (row 0).
2. Try the first column (column 0).
3. The board is empty, so no conflicts.
The first queen is placed!
Step 2: Place the second queen
1. Move to the second row (row 1).
2. Check column 0:
Not safe (vertical attack by the first queen).
3. Check column 1:
Not safe (diagonal attack by the first queen).
4. Check column 2:
Safe! Place the second queen here.
Step 3: Place the third queen
1. Move to the third row (row 2).
2. Check column 0:
Not safe (diagonal attack by the second queen).
3. Check column 1:
Not safe (diagonal attack by the first queen).
4. Check column 2:
5. Not safe (vertical attack by the second queen).
6. Check column 3:
Safe! Place the third queen here.
Step 4: Place the fourth queen
1. Move to the fourth row (row 3).
2. Check column 0:
Not safe (diagonal attack).
3. Check column 1:
Not safe (diagonal attack).
4. Check column 2:
Not safe (vertical attack).
5. Check column 3:
Not safe (vertical attack).
6. No safe spot for the fourth queen. Time to backtrack!
Step 5: Backtracking
1. Remove the third queen from column 3.
2. Try moving the third queen to another column:
No other safe spots in row 2.
3. Backtrack further:
Remove the second queen from column 2.
Move it to column 3 (safe now).
Step 6: Adjust and Retry
1. Place the third queen in row 2:
Check column 0: Safe! Place it here.
2. Place the fourth queen in row 3:
Check column 2: Safe! Place it here.
The Final Board
After all the steps and adjustments, the final positions of the queens are:
1. Row 0, Column 0
2. Row 1, Column 3
3. Row 2, Column 1
4. Row 3, Column 2
The puzzle is solved! All queens are safely placed without attacking each other.
