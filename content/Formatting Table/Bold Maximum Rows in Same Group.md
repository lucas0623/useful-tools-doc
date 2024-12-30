---
Created: 2024-10-05
---
## 1	Version
- This tutorial is written based on Version 1.2.0 of the add-in.
## 2	Introduction
### 2.1	Usage
- This function is used to **bold** rows with maximum value in the same group. See example in this page. The way of using it is similar to [[Add Bottom Borders in Same Group]].
- This is a sample data set. This function can help to bold the maximum utilization for each group.
![[content/Z_System/Attachment/Pasted image 20241005110908.png]]
### 2.2	What Existing Problem is Solved?
- Time consuming process when formatting table for better presentation.

## 3	Instruction
1. **Select the rows of data** that you would need to process with. (any columns are ok, only rows information is used for the macro.) ![[content/Z_System/Attachment/Pasted image 20241005111131.png]]
2. **Click 'Bold Maximum Rows in Same Group'. Select the Column that is used to identify group data.** Select any cell in Column A in this example, as the group data is presented in column A. Then Click OK. ![[content/Z_System/Attachment/Pasted image 20241005111543.png]]
3. Another userform will pop up. Select the Column that contains the value of data. Select any cell in Column C in this example, as the utilization data is presented in column C. Then Click OK.![[content/Z_System/Attachment/Pasted image 20241005111623.png]]
4. The rows of maximum utilization of each group are bolded. ![[content/Z_System/Attachment/Pasted image 20241005115102.png]]

## 4	Remarks on Macro's Logic
- The logic is similar to [[Add Bottom Borders in Same Group]] and described below:
	- First, the macro will get the 'group label' data from user's selected rows (before clicking the button) and the column specified in the userform.
	- then, the macro will identify the 'value' data, and find out the range of data in the same group, and bold the row with the maximum value.
![[content/Z_System/Attachment/Pasted image 20241230224403.png]]

![[content/Z_System/Attachment/Pasted image 20241230230348.png]]
