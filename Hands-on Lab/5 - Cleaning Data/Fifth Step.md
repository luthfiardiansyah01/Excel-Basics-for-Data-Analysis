## Removing Duplicated, Irrelevant or Inaccurate Data
A. Check spelling
  1. Download the file `Customer_demographics_and_sales_Lab5.xlsx`. Upload and open it using Excel for the web.
  2. Select column L (CREDITCARD_TYPE), then click Review tab, and select Spelling.
  3. Click the correct suggestion to change the spelling
      + Note: Don’t change ‘jcb’ spelling when doing the spell check. We will need 'jcb' for the Exercise 1 Task D.
  4. Close the Spelling pane.
  ![image](https://user-images.githubusercontent.com/71245686/189687172-70ed6e9d-8f4b-47b2-a27c-2547c0d5d0d3.png)

B. Remove empty rows
  1. Press CTRL+HOME, then press CTRL+SHIFT+END to select the whole datasheet.
  2. On the Data tab, click Filter.
  3. Press CTRL+HOME, click the filter arrow in the CUST_NAME column, and then click Filter.
  4. Click the Select All checkbox to deselect all of them. Then select just Blanks, then OK.
  5. Select first row, then press CTRL+SHIFT+END to select all rows.
  6. Right-click the selected rows and then click Delete Rows.
  7. Finally, on the Data tab, click Clear, then click Filter.
  ![image](https://user-images.githubusercontent.com/71245686/189687246-1bee104e-790f-4e89-90f2-b5d0f881a108.png)

C. Remove duplicate rows
  1. Select Column T (ORDER_ID) since ORDER_ID values are unique.
  2. On the Home tab, click Conditional Formatting> Highlight Cells Rules> Duplicate Values, and then click OK.
  3. Select the whole datasheet (CTRL+SHIFT+END)
  4. On the Data tab, click Remove Duplicates.
  5. In the Remove Duplicates dialog box, ensure that Select all columns is checked and that My data has headers is also checked, then click OK.
  6. In the pop-up box informing you how many duplicate values were found and removed, click OK.
  ![image](https://user-images.githubusercontent.com/71245686/189687321-9bf16045-7402-43b0-b063-78fce78ce711.png) 

D. Use Find & Replace to correct misspelling
  1. On the Home tab, click Find & Select.
  2. Click Find. In Find what, type jcb, and click Find All.
  3. Click Replace.
  4. In Replace with, type JCB, click Replace All, and then click the Close icon.
  5. On the Home tab, click Conditional Formatting> Clear Rules> Clear Rules from Entire Sheet.
  ![image](https://user-images.githubusercontent.com/71245686/189687368-4cbeb209-45ac-4399-aa5d-f51b2581bd15.png)

## Dealing with Inconsistencies in Data
A. Use the PROPER function to change text from upper case to proper case
  1. Select row 2, then right-click it and choose Insert Rows.
  2. In cell A2, type =PROPER(A1) and press Enter.
  3. Hover over the bottom-right corner of cell A2, and drag the Fill Handle across to the last column.
    + If dragging across is too difficult with the mouse, then select the cells in the row 2 using SHIFT+RIGHT ARROW, then press F2 to put the cursor focus back in cell A2, then hold CTRL while you press Enter.
  4. Select row 2, then press CTRL+C.
  5. Select row 1, Right-click and choose Paste Options>Values.
  6. Select row 2, right-click it and choose Delete Rows.

B. Use the UPPER function to change text from proper case to upper case
  1. Select column AG (Generation). Then right-click and choose Insert Columns. In cell AG1, type Generation.
  2. In cell AG2, type =UPPER(AH2) and press Enter.
  3. Hover over the bottom-right corner of cell AG2 and double-click the Fill Handle.
  4. Select column AG, then press CTRL+C.
  5. Select column AH, right-click and choose Paste Options>Values.
  6. Select column AG, right-click it and choose Delete Columns.

C. Use the LOWER function to change text from proper case to lower case
  1. Select column AC (T_Type). Then right-click and choose Insert Columns. In cell AC1, type T_Type.
  2. In cell AC2, type =LOWER(AD2) and press Enter.
  3. Hover over the bottom-right corner of cell AC2 and double-click the Fill Handle.
  4. Select column AC, then press CTRL+C.
  5. Select column AD, right-click and choose Paste Options>Values.
  6. Select column AC, right-click it and choose Delete Columns.

D. Change date formatting
  1. Select column Z (Order_Ship_Date).
  2. On the Home tab, in the Number group click Number Format> More Number Formats.
  3. In the Category list, select Date.
  4. In the Format Cells box, under Locale, select English (United States).
  5. Under Type, select Wednesday, March 14, 2012 and click OK.
  ![image](https://user-images.githubusercontent.com/71245686/189687447-361eec08-8db1-412d-a4aa-9f9c3e9e5070.png)

E. Use Find & Replace to trim whitespace
  1. Click CTRL+HOME.
  2. Select all the data using CTRL+SHIFT+END.
  3. On the Home tab, click Find & Select, then Replace.
  4. In Find what, type 2 spaces. In Replace with, type 1 space.
  5. Click Find All, then click Replace All.
  6. Click the Close icon.

## More Excel Features for Cleaning Data
A. Use the Flash Fill feature to clean data
  1. Select column A (Cust_Name), right-click and choose Insert Columns.
  2. In cell A1 type Customer_Name and press Enter
  3. In cell A2, type Mr. Allen Perl and press Enter.
  4. Select column A (Customer_Name), on the Data tab, click Flash Fill.
  5. Click Undo to undo this step.

```
If you are using the desktop version of Excel, you could use the 'Text to Columns' feature to perform this next task (see the corresponding topic video for instructions).
If you are using ‘Excel for the web’ (the online version of Excel), the ‘Text to Columns’ feature is not available, but you can achieve the same results using functions, as shown in the steps below.
```

B. Use LEFT, RIGHT, LEN, and SEARCH functions to clean data
  1. Select column A (Cust_Name), right-click and choose Insert Columns.
  2. Select column A again, right-click and choose Insert Columns.
  3. In cell A1, type Customer_Firstname and in cell B1, type Customer_Lastname.
  4. Click C1, then on the Home tab, click Format Painter, then drag across to A1 and B1.
  5. Double-click the divider between columns A and B.
  6. In cell A2 type =LEFT(C2, SEARCH(" ",C2,1)) and press Enter.
  7. In cell B2 type =RIGHT(C2,LEN(C2)-SEARCH(" ",C2,1)) and press Enter.
  8. Double-click the Fill Handle on cell A2.
  9. Double-click the Fill Handle on cell B2.
