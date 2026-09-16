**Lab Experiment 4: Bivariate Analysis for Sales Data using Power BI**

### Name: SUDARSHANA
### Register Number: 212223050054

**Aim**

To perform data preparation and bivariate analysis on sales data using Power BI, create DAX measures, visualize relationships between variables, and develop an interactive Bivariate Sales Analysis Report.

**Procedure**

**1.Import Data**

Import the Customers, Orders, Order Items, and Products datasets into Power BI.

**2.Data Preparation using Power Query**

  Open Power Query Editor.
  Remove unnecessary columns.
  Rename relevant columns.
  Change appropriate data types.
  Filter data where required.
  Split columns where applicable.
  Replace values where required.
  Click Close & Apply.

**3.Create Data Relationships**

    Open Model View.
    Create/check relationships between the tables using common fields such as:
      Customer ID
      Order ID
      Product ID

**4.Create DAX Measures**

Create the following measures:
    (i)Total Sales = SUMX(
        'Order Items',
        'Order Items'[quantity] *
        RELATED(Products[unit_price]) *
        (1 - 'Order Items'[discount_rate]))

    (ii)Total Orders =DISTINCTCOUNT(Orders[order_id])
    (iii) Total Quantity = SUM('Order Items'[quantity])
    (iv) Average Order Value = DIVIDE([Total Sales],[Total Orders])
  
**5.Perform Bivariate Analysis**

    Category vs Sales: Use Category and [Total Sales] in a Column/Bar Chart.
    Sales Channel vs Sales: Use Sales Channel and [Total Sales] in a Column/Bar Chart.
    Payment Method vs Sales: Use Payment Method and [Total Sales] in a Bar/Column Chart.
    Category vs Quantity: Use Category and [Total Quantity] in a Column/Bar Chart.
    Price vs Quantity: Use Unit Price and Quantity in a Scatter Plot to observe their relationship.

**6.Create Summary Cards**
    
      Create four cards using:
      [Total Sales]
      [Total Orders]
      [Total Quantity]
      [Average Order Value]

**7.Add Slicers**

    Add two slicers:
      Sales Channel
      Product Category

**8.Create the Report**
    Arrange the cards, charts, and slicers clearly on a single report page.
    Add meaningful titles to the visualizations.
    Analyze the results and identify useful business insights.      

**Output**

<img width="2006" height="1122" alt="image" src="https://github.com/user-attachments/assets/7d50df39-a9cf-4e2a-a073-68c291857134" />

**Result**
Thus, the sales data was successfully prepared and analyzed using Power BI. 
