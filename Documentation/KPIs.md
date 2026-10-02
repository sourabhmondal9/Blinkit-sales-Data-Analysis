# KPI Definitions

## 1. Total Sales

**Definition:** Sum of the Sales measure across the selected data.

**Business meaning:** Measures overall revenue/sales value generated.

**Typical DAX:**
```DAX
Total Sales = SUM('BlinkIT Grocery Data'[Sales])
```

## 2. Average Sales

**Definition:** Average sales value per record.

**Business meaning:** Provides a simple measure of the average sales value represented by each item-level record.

**Typical DAX:**
```DAX
Avg Sales = AVERAGE('BlinkIT Grocery Data'[Sales])
```

## 3. Number of Items

**Definition:** Count of item records.

**Business meaning:** Measures the volume of item-level records represented in the dataset.

**Typical DAX:**
```DAX
No of Items = COUNTROWS('BlinkIT Grocery Data')
```

## 4. Average Rating

**Definition:** Average of the customer rating field.

**Business meaning:** Provides an overall customer-rating indicator.

**Typical DAX:**
```DAX
Avg Rating = AVERAGE('BlinkIT Grocery Data'[Rating])
```

## Supporting Metrics

### Sales by Outlet Type

```DAX
Total Sales = SUM('BlinkIT Grocery Data'[Sales])
```

Use `Outlet Type` as the category.

### Sales by Outlet Location

Use `Outlet Location Type` as the category with Total Sales.

### Sales by Outlet Size

Use `Outlet Size` as the category with Total Sales.

### Sales by Establishment Year

Use `Outlet Establishment Year` as the axis with Total Sales.

### Average Item Visibility

```DAX
Avg Item Visibility = AVERAGE('BlinkIT Grocery Data'[Item Visibility])
```

## KPI Design Principle

The dashboard combines four dimensions of performance:

- Value → Total Sales
- Average value → Average Sales
- Volume → Number of Items
- Customer experience → Average Rating
