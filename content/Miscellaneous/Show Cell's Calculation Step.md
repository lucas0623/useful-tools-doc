---
Created: 2024-10-05
---
## 1	Version
- This tutorial is written based on <u>Version 1.2.1</u> of the 'Useful Tools Add-in'
## 2	Introduction
### 2.1	Usage
- To convert the formula created with the defined excel formula 'FormulaConcat' to excel default 'Concat' function. 
### 2.2	What Problem is Solved?
- Time consuming process of showing calculation steps for simple calculation.
## 3	Instruction
### 3.1	User Defined Formula 'FormulaConcat'
1. See this example. We would like to show the calculation steps of cell D5 in Cell D4. ![[Pasted image 20241012162013.png]]
2. In Cell D4, input '=FormulaConcat(D5)' and press Enter. ![[Pasted image 20241012162144.png]]
3. The output of 'FormulaConcat' will be a String of a 'Concat' formula. ![[Pasted image 20241012162217.png]]
### 3.2	Converting the 'FormulaConcat' to Default 'Concat'
1. Continue from the example above, after using the 'FormulaConcat' function, press the button ![[Pasted image 20241012162542.png|180]]. 
2. All cells with 'FormulaConcat' will be converted to excel default 'Concat' function. In this example, the formula in cell D4 is converted and the calculation step is shown. ![[Pasted image 20241012162955.png]]

## 4	Remarks on Macro's Logic
- Calculation using 'LET' or 'Lambda' is not support.