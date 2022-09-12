## Basics of Formulas
1. Download the file `Personal_Monthly_Expenditure_Lab4.xlsx`. Upload and open it using Excel for the web. Go to the Expense - 2018 worksheet.
![image](https://user-images.githubusercontent.com/71245686/189628315-3a005cf5-6f94-4487-a931-2ee26b1497cc.png)
2. In A14, type Totals and in B14, type =SUM( then select cells B2 to B13 with the mouse, and press Enter.
3. Select the fill handle on cell B14 and drag to G14 to copy the formula.
4. In cell H1, type Monthly Total and double-click the divider between H and I.
5. In H2, type =SUM( then select cells B2 to G2 with the mouse, and press Enter. If necessary, select the fill handle on cell H2 and drag to H14 to copy the formula.
6. Select columns B to H. On the Home tab, in the Number group, click the Accounting Number Format ($) drop-down list, and select $ English (United States).
![image](https://user-images.githubusercontent.com/71245686/189628508-1c9ff9f0-6ada-409a-bfea-13322a7feef6.png)


## Basics of Functions
1. In cells A16-A20, type the following:
    + Avg
    + Min
    + Max
    + Count
    + Median
2. In B16, type =AVERAGE( then select cells B2 to B13 with the mouse, and press Enter. Select the fill handle on cell B16 and drag to G16 to copy the formula.
3. In B17, type =MIN( then select cells B2 to B13 with the mouse, and press Enter. Select the fill handle on cell B17 and drag to G17 to copy the formula.
4. In B18, type =MAX( then select cells B2 to B13 with the mouse, and press Enter. Select the fill handle on cell B18 and drag to G18 to copy the formula.
5. In B19, type =COUNT( then select cells B2 to B13 with the mouse, and press Enter. Select the fill handle on cell B19 and drag to G19 to copy the formula. Select row 19. On the Home tab, click the Number Format drop-down list, and select Number.
6. In B20, type =MEDIAN( then select cells B2 to B13 with the mouse, and press Enter. Select the fill handle on cell B20 and drag to G20 to copy the formula.
![image](https://user-images.githubusercontent.com/71245686/189628602-7685832f-c37b-41d6-b008-6e8cbdbf7843.png)
7. Explore some more commonly used functions of a data analyst by clicking the arrow under AutoSum, then select More Functions and look at some of the functions in various categories to see what actions they perform:
    + Financial : ACCRINT, INTRATE
    + Logical : AND, IF, OR, NOT
    + Text : CONCAT, FIND, SEARCH
    + Date & Time : NETWORKDAYS, WEEKDAY
    + Lookup & Reference : AREAS, SORTBY, VLOOKUP, HLOOKUP
    + Math & Trig : POWER, SUMIF, SUMPRODUCT
    + Statistical : AVERAGE, COUNTIF, MAX, MEDIAN, MIN

## Referencing Data in Formulas (relative vs absolute) & Formula Errors
1. In cells A31-A40, type 1-10. Select row 31 to 40. On the Home tab, click the Number Format drop-down list, and select General.
2. Relative References : In cell B33, type =A31+A32 and press Enter. Select the fill handle on cell B33 and drag to B40 to copy the formula. Here, both first and second cell reference will move 1 cell down. For example, on cell B34 formula will be changed to =A32+A33, on cell B35 formula will be changed to =A33+A34 and so on.
3. Absolute References : In cell C33, type =$A$31+$A$32 and press Enter. Select the fill handle on cell C33 and drag to C40 to copy the formula. Here, both first and second cell references will not change. For example, on cell C34 formula will remain =$A$31+$A$32, on cell C35 formula will remain =$A$31+$A$32 and so on.
4. Mixed References : In cell D33, type =$A$31+$A32 and press Enter. Select the fill handle on cell D33 and drag to D40 to copy the formula. Here, first cell reference will stay the same, but the second reference will change. For example, on cell D34 formula will be changed to =$A$31+$A33, on cell D35 formula will be changed to =$A$31+$A34 and so on.
![image](https://user-images.githubusercontent.com/71245686/189628857-e9d1399e-a6bb-4821-b871-7a3fb3d0a257.png)
5. In cell B31, type =A16+A17. Now this will lead to a formula error #VALUE! since cells A16 and A17 do not contain any number.
![image](https://user-images.githubusercontent.com/71245686/189628905-5105c29e-ee5b-4a1c-9740-5866a43a2207.png)
6. Click the question mark icon in the error message box. This will open the Help for this topic. Read through this help file for more information about #VALUE! errors in formulas.
![image](https://user-images.githubusercontent.com/71245686/189628933-20069601-8f44-45f0-9fe7-914e4d40b63e.png)
