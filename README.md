# SudokuBot
CS 171 Winter Quarter 2026 
Details in student manual PDF.

## AI Algorithms
### Consistency Checking
- Forward Checking (FC)
- Norvig Checking (NOR)
### Variable Selection
- Minimum Remaining Values (MRV)
- MRV with Tiebreaker (MAD)
### Value Ordering
- Least Constraining Value (LCV)

## Generating Sudoku Boards 
1. Change directory to board generator folder.
```
cd ~/SudokuBot/Sudoku_Generator
```
2. Run Makefile.
```
make
```
3. Enter parameters (example entries below). 
```
Enter p: 3
Enter q: 3
Enter given values: 7
How many boards created?: 10
```

## Solving Sudoku Boards
1. Change directory to main folder.
```
cd ~/SudokuBot/Sudoku_Python_Shell
```
2. Run Makefile to generate .pyc files if not already done so.
```
make
```
3. Execute AI solver (example arguments down below).
```
python3 bin/Main.pyc FC MRV LCV ~/SudokuBot/Sudoku_Generator/easy
python3 bin/Main.pyc NOR MAD LCV ~/SudokuBot/Sudoku_Generator/intermediate/board_0.txt

```