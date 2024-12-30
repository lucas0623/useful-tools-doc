---
Created: 2024-10-05
---
## 1	Version
- This tutorial is written based on Version 1.2.0 of the add-in.
## 2	Introduction
### 2.1	Usage
- This function is used to quickly add bottom borders in the table. See example below:
- This is a sample data set. This function can help to add bottom border to separate the data of different groups (i.e. at row 4,6,11). ![[../../Z_System/Attachment/Pasted image 20241005103027.png|500]]
### 2.2 What Existing Problem is Solved?
- Time consuming process when formatting table for better presentation.
## 3	Instruction
1. Select the rows of data that you would need to add bottom data. (any columns are ok, only rows information is used for the macro.) ![[../../Z_System/Attachment/Pasted image 20241005103349.png|400]]
2. Click 'Add Bottom Borders in Same Group'. An userform will pop up. ![[../../Z_System/Attachment/Pasted image 20241005105601.png]]
3. Follow the instruction of the userform. 1 is used in this example. Click OK.
4. Another userform will pop up. Select the Column that is used to identify group data. Select any cell in Column A in this example, as the group data is presented in column A. Then Click OK.![[../../Z_System/Attachment/Pasted image 20241005105837.png]]
5. Bottom border is added at the desired locations. The bottom border will be applied to the whole row. ![[../../Z_System/Attachment/Pasted image 20241005105952.png]]

## 4	Remarks on Macro's Logic
- The logic is listed below:
	- First, the macro will get the 'group label' data from user's selected rows (before clicking the button) and the column specified in the userform.
	- then, the macro will loop each cell of the 'group label', and add bottom border to current row whenever the next row is different from the current row.