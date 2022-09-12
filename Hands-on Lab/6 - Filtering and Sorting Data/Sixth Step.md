## Filtering and Sorting Data
A. Filtering data
  1. Download the file `Customer_demographics_and_sales_Lab6.xlsx`. Upload and open it using Excel for the web.
  2. Select any cell in the data, and click the Data tab, then click Filter.
  3. Click the filter drop-down in column AG (Purchase_Status), and select Filter....
  4. In the list, only select Frequent and click OK.
  
      ![image](https://user-images.githubusercontent.com/71245686/189583220-b994db6e-0c1c-4a43-9d65-75d5fd80d7f7.png)
  
  5. Click the filter drop-down in the column AG, and click Clear Filter From “Purchase_Status”.

      ![image](https://user-images.githubusercontent.com/71245686/189584373-e971f00f-7692-40ed-8255-8cc6f2c01bd2.png)

  6. Click the filter drop-down in column AE (T_Type), and select Filter....
  7. In the list, only select Cancelled and click OK.
  8. Click the filter drop-down in column AF (Purchase_Touchpoint), and select Filter....
  9. In the list, only select Desktop and click OK.
  10. On the Data tab, click Clear.
  
      ![image](https://user-images.githubusercontent.com/71245686/189584750-ea9f29e9-0011-4ca0-892c-4d6e964c41eb.png)

      ```
      To use Custom Filters to filter data:
      o Click the filter drop-down in column AD (Order_Value), then Number Filters>Top 10....
      o Change the value from 10 to 50 and Click OK.
      o Click the filter drop-down in the column AD, and click Clear Filter From “Order_Value”.
      ```
  
B. Sorting data
  1. On the Data tab, click Custom Sort to open a dialog box like below
      
      ![image](https://user-images.githubusercontent.com/71245686/189588046-89f78c51-e60c-4426-9c44-6c602e693f6e.png)
  
  2. Click the Column drop-down of row Sort By, select Order_Ship_Date.
  3. Click the Order drop-down of row Sort By, select Sort Ascending
  4. Click Add.
  5. Click the Column drop-down of row Then By, select Order_Value.
  6. Click the Order drop-down of row Then By, select Sort Descending.
  7. Click OK.

## Useful Functions for Data Analysis
A. Use of IF to apply one condition
  1. Select column AF, right-click, Insert.
  2. In cell AF1, type Complete?.
  3. In cell AF2, type =IF(AE2="Complete","Yes","No") and press Enter.
  4. Double-click the Fill Handle of AF2 to copy down the column.
 
B. Use of Nested IF to apply multiple conditions
  1. Select column AE, right-click, Insert.
  2. In cell AE1, type Order Size (IF).
  3. In cell AE2, type =IF(AD2>300,"Large",IF(AD2>100,"Medium",IF(AD2>0,"Small"))) and press Enter.
  4. Double-click the Fill Handle of AE2 to copy down the column.

C. Use of IFS to apply multiple conditions (alternative of Nested IF)
  1. Select column AE, right-click, Insert.
  2. In cell AE1, type Order Size (IFS).
  3. In cell AE2, type =IFS(AD2>300,"Large",AD2>100,"Medium",AD2>0,"Small") and press Enter.
  4. Double-click the Fill Handle of AE2 to copy down the column.

D. Use of COUNTIF to count the number of cells that meet a specified criterion
  1. Select cell BX2 and type count VISA card.
  2. Select cell BY2 and type =COUNTIF(N2:N195,"VISA") and press Enter.

E. Use of SUMIF function to sum the values within a specified range that meet a specified criterion
  1. Select cell BX3 and type sum Large order.
  2. Select cell BY3 and type =SUMIF(AE2:AE195,"Large", AD2:AD195) and press Enter. 
      ```
      Formula: =SUMIF(range, criteria, [sum range]).
      ```

F. Use of SUMIFS function to sum the values within a specified range that meet multiple specified criteria
  1. Select cell BX4 and type sum Large order with Baby Gen.
  2. Select cell BY4 and type =SUMIFS(AD2:AD195, AE2:AE195,"Large", AL2:AL195,"*BABY_BOOMERS*") and press Enter. 
      ```
      Formula: =SUMIFS ([sum range], range1, criteria1, range2, criteria2, ...).
      ```
  
## Using the VLOOKUP and HLOOKUP Functions
A. Use of VLOOKUP to look up data in a table organized vertically
  1. Download the file `indian_startup_funding_Lab6.xlsx`. Upload and open it using Excel for the web.
  2. In cell K2,L2,M2, type VLOOKUP, Startup Name, Amount in USD respectively.
  3. Select and copy cells from C9 to C15 and paste in cell L3.
  4. In cell M3, type =VLOOKUP(L3, C2:I113, 7, FALSE) and press Enter.
      ```
      Formula: =VLOOKUP (value, table, col_index, [range_lookup]).
      ```
  5. Hover over the bottom-right corner of cell M3, and drag the Fill Handle down to the cell M9.
  6. Select cells from M3 to M9 and select Number Format>Currency.

      ![image](https://user-images.githubusercontent.com/71245686/189590838-99cb6b2c-d8d6-40f0-ad25-0f35152f67fd.png)


B. Use of HLOOKUP to look up data in a table organized horizontally
  1. Download the file `Personal_Monthly_Expenditure_Lab6.xlsx`. Upload and open it using Excel for the web.
  2. In cell J2,K2,L2,M2, type HLOOKUP, Month, Food & Dining, Health & Fitness respectively.
  3. Select and copy cells from A10 to A12 and paste in cell K3.
  4. In cell L3, type =HLOOKUP(D1, A1:H14, 10, FALSE) and press Enter.
      ```
      Formula: =HLOOKUP (value, table, row_index, [range_lookup]).
      ```
  5. Hover over the bottom-right corner of cell L3, and drag the Fill Handle down to the cell L5.
  6. Select cells from L3 to L5 and select Number Format>Currency.
  7. In cell M3, type =HLOOKUP(G1, A1:H14, 10, FALSE) and press Enter.
  8. Hover over the bottom-right corner of cell M3, and drag the Fill Handle down to the cell M5.
  9. Select cells from M3 to M5 and select Number Format>Currency.
      ![image](https://user-images.githubusercontent.com/71245686/189591513-ce51911e-9913-4d24-9c5c-549beebaef34.png)
