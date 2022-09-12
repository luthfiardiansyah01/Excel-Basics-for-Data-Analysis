## Introduction to Creating Pivot Tables in Excel
A. Format data as a table
  1. Download the file `indian_startup_funding_Lab7.xlsx`. Upload and open it using Excel for the web.
  2. Select cell A2.
  3. On the Home tab, in the Tables group, click Format as Table.
  4. Select Light Gray, Table Style Medium 15.

B. Create a pivot table and use fields to arrange data in a pivot table
  1. Select cell D4
  2. On the Insert tab, click PivotTable.
  3. Click OK.

      ![image](https://user-images.githubusercontent.com/71245686/189595347-0b6fc4f0-ff5a-4134-8d7d-587cde51c90f.png)

  4. Double-click Sheet1, type Pivot1 and click OK.
  5. In the fields list, drag Industry Vertical to Rows. 
  6. In the fields list, drag City Location to Rows below Industry Vertical.
  7. In the fields list, drag Startup Name to Rows below City Location.
  8. In the fields list, drag Amount in USD to Values.
  9. In the ribbon, select the PivotTable tab, click Settings, then in the PivotTable Settings pane, under Layout, select Single column.

C. Perform a simple calculation in a pivot table
  1. In the PivotTable Fields pane, in the Values section, click the drop-down arrow next to Count of Amount in USD, and click Value Field Settings.
  2. Select Summarize value field by > Sum.

      ![image](https://user-images.githubusercontent.com/71245686/189595642-37e103a6-5033-47dc-ade1-dca5a19e4999.png)

  3. Click OK.
  4. Select the column called Sum of Amount in USD and then on the Home tab, select Accounting Number Format > $ English (United States).

## Pivot Table Features
```
Note: The 'Recommended Charts' feature only works with 'full' Office for the web plans (those plans that come with an Office 365 subscription). 
Recommended Charts do not work with the 'basic' plan that comes with a Microsoft Account.
```
A. Use of the Recommended Charts feature (Optional: If you have a full Office for the web plan)
  1. Switch to worksheet indian-startup-funding.
  2. Select column F (City Location).
  3. On the Insert tab, select Recommended Charts.
  4. Click + Insert PivotChart.

      ![image](https://user-images.githubusercontent.com/71245686/189596618-49132406-a5d3-4911-b6a2-2bc066545a0a.png)


  5. Switch to worksheet indian-startup-funding again.
  6. Select column C, D, E.
  7. On the Insert tab, select Recommended Charts.
  8. Choose the recommended chart, and click + Insert PivotChart.

      ![image](https://user-images.githubusercontent.com/71245686/189596686-8d5025ca-0839-41cc-84f9-c895bf8c48f0.png)


B. Use of the Filters feature
  1. Switch to worksheet Pivot1.
  2. In the Pivot Table, click the Row Labels arrow.
  3. Select City Location, then Filter....
  4. Just select Burnsville, Delhi, New York, then click OK to display the amounts for startups in these three cities only.
  5. In the Pivot Table, click the Row Labels arrow.
  6. Select City Location, then click Clear Filter From 'City Location' to display the startups in all cities again.
 
C. Use of the Slicers feature
  1. Download the file indian_startup_funding_Lab7_with_slicers_timelines.xlsx. Upload and open it using Excel for the web.
  2. Switch to worksheet Pivot1 if you are not there.
  3. In the City Location slicer, select Burnsville, then Delhi, then New York.
  4. To filter by multiple selection in the City Location slicer, with New York still selected, press CTRL and select Burnsville, and then Delhi.
  5. To filter using more than one slicer, in the Investors Name slicer, select Amour Infrastructure, then press CTRL and select Westbridge Capital, and then Breakthrough Energy Ventures.
  6. In the City Location slicer, click the Clear Filter button, then in the Investors Name slicer, click the Clear Filter button.

D. Use of the Timelines feature
  1. In the Date timeline, click top right drop-down and select DAYS, then scroll left and right.

      ![image](https://user-images.githubusercontent.com/71245686/189596895-1ced0948-ee8f-4cbe-afb8-d7112279a31c.png)

  2. In the Date timeline, click top right drop-down and select QUARTERS.
  3. In the Date Timeline, select 2019 Q1, then drag 2019 Q1 to 2019 Q3.
  4. In the Date timeline, click the Clear Filter icon.
  5. In the Date timeline, click top right drop-down and select YEARS, then select 2020 only.
