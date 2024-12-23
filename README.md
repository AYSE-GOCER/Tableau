**Tableau Notes: Inserting Dynamic Filters in Tableau**

Example 1:

[See the interactive worksheet:](https://public.tableau.com/views/Ayse_Dynamic_WorkSheet_1/InsertingDynamicTreshold?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
![trashold](https://github.com/user-attachments/assets/27537487-b53a-49a2-8798-8bafacbc8cb7)

Example 2:

[See the interactive worksheet:](https://public.tableau.com/app/profile/ayse.gocer/viz/Ayse_Dynamic_WorkSheet/DynamicMeasures)
![dynamic_measure](https://github.com/user-attachments/assets/f3c65be8-8007-4c2a-8fb1-cee2d8aea254)

Example 3:

[See the interactive worksheet:](https://public.tableau.com/app/profile/ayse.gocer/viz/Ayse_Dynamic_WorkSheet_2/DynamicFilters)
![top_n_proucts](https://github.com/user-attachments/assets/3cac2852-ce8c-4586-902f-1197837a2986)

Example 4:

[See the interactive worksheet:](https://public.tableau.com/app/profile/ayse.gocer/viz/Ayse_Dynamic_WorkSheet_3/DynamicDimensions)
![choose_dim](https://github.com/user-attachments/assets/6e394154-fd1b-457c-9e19-ef254dab27fa)

Example 5:
[See the interactive dashboard:](https://public.tableau.com/app/profile/ayse.gocer/viz/Ayse_Dynamic_WorkSheet_4/Dashboard1?publish=yes)
![dashbord_1](https://github.com/user-attachments/assets/31a7e4aa-0d41-48ea-9c73-e21c5bd5d7ea)

Example 6:
[See the interactive dashboard:](https://public.tableau.com/app/profile/ayse.gocer/viz/Ayse_Dynamic_WorkSheet_5/Dashboard2?publish=yes)
![filter](https://github.com/user-attachments/assets/cb582d30-acb4-4a4c-a67b-669b6e53d365)

Example 7:
[See the interactive worksheet:](https://public.tableau.com/app/profile/ayse.gocer/viz/Ayse_Dynamic_WorkSheet_6/Sheet7?publish=yes)
![action_set](https://github.com/user-attachments/assets/08bfa68f-fb74-4a44-82ae-97630350bb6b)

Example 8:
[See the interactive dashboard:](https://public.tableau.com/app/profile/ayse.gocer/viz/Ayse_Dynamic_WorkSheet_7/Dashboard3?publish=yes)
![by_month](https://github.com/user-attachments/assets/c8a4e5df-2b39-4106-be9e-fe013fa35ed5)

Example 9: Lower case - Upper case strings:

 - UPPER([Product_Name]) 
 - LOWER([Product_Name])
   
[See the interactive worksheet](https://public.tableau.com/app/profile/ayse.gocer/viz/AyseGocer_dynamic_worksheet_8/LowerUpper?publish=yes)

Example 10: Removing unwanted space from the text):

- LTRIM([Product_Name])
- RTRIM([Product_Name])
- TRIM([Product_Name])
- COUNTD([Product_Name])

[See the interactive worksheet](https://public.tableau.com/app/profile/ayse.gocer/viz/AyseGocer_dynamic_worksheet_9/LTRIMRTRIMTRIM?publish=yes)

Example 11: Extract particular field from a string (LEFT, RIGHT, MID):

- LEFT([Product_Image],5)
- RIGHT([Product_Image], 3)
- MID([Product_Image],9,21)

[See the interactive worksheet](https://public.tableau.com/app/profile/ayse.gocer/viz/AyseGocer_dynamic_worksheet_10/LEFTRIGHTMID?publish=yes)

Example 12: Search particular character in a string (STARTSWITH, ENDSWITH, CONTAINS):

- CONTAINS(LOWER([Product_Name]), "samsung")

- STARTSWITH([Product_Name],"Apple")

- ENDSWITH([Product_Name], "Clock")

[See the interactive worksheet](https://public.tableau.com/app/profile/ayse.gocer/viz/AyseGocer_dynamic_worksheet_11/SEARCH?publish=yes)

Example 13: Filtering the data:

IF CONTAINS(LOWER([Product_Name]), "apple") THEN "Apple"
ELSEIF CONTAINS(LOWER([Product_Name]), "samsung") THEN "Samsung"
ELSEIF CONTAINS(LOWER([Product_Name]), "microsoft") THEN "Microsoft"
ELSE "Unknown"
END

[See the interactive worksheet](https://public.tableau.com/app/profile/ayse.gocer/viz/AyseGocer_dynamic_worksheet_12/FILTERINGDATA?publish=yes)

Example 14: Filtering the data:

LEFT([Phone], FIND([Phone], "-")-1)

[See the interactive worksheet](https://public.tableau.com/app/profile/ayse.gocer/viz/AyseGocer_dynamic_worksheet_13/FINDFINDNTH?publish=yes)

Example 15: Combine and/or split data:

- [First_Name] + " " + [Last_Name]
- [Category] + ":" + [Product_Name]
- SPLIT([Phone], "-", 2)
- SPLIT([Phone],"-", 3) + "-" + SPLIT([Phone],"-", 4)
  
[See the interactive worksheet](https://public.tableau.com/app/profile/ayse.gocer/viz/AyseGocer_dynamic_worksheet_14/SPLITCOMBINE?publish=yes)

Example 16: Replace:

- REPLACE([Phone], "+", "00")
- REPLACE(REPLACE([Phone], "+", "00"), "-", "")

[See the interactive worksheet](https://public.tableau.com/app/profile/ayse.gocer/viz/AyseGocer_dynamic_worksheet_15/REPLACE?publish=yes)

Example 17: Date Functions:

- DATEPART('year', [Order Date]) (numeric output)
- DATENAME('year', [Order Date]) (string output)
- YEAR([Order Date]) (numeric output)
- MONTH([Order Date])
- DATENAME("month",[Order Date])
- DAY([Order Date])
- QUARTER([Order Date])
- LEFT(DATENAME("month",[Order Date]),3)

[See the interactive worksheet](https://public.tableau.com/app/profile/ayse.gocer/viz/Ayse_Dynamic_WorkSheet_16/DATEFUNCTIONS?publish=yes)
- DATETRUNC("month", [Order Date])
![date_trunck](https://github.com/user-attachments/assets/671bb784-e3fc-41a2-b65a-8dd77535886d)
[See the interactive worksheet](https://public.tableau.com/app/profile/ayse.gocer/viz/Ayse_Dynamic_WorkSheet_18/DATETRUNC?publish=yes)
![date_functions](https://github.com/user-attachments/assets/b03da04e-b5fb-4936-b36a-f923c5e12ce0)[See the interactive worksheet](https://public.tableau.com/app/profile/ayse.gocer/viz/Ayse_Dynamic_WorkSheet_17/DATEFUNCTIONS?publish=yes)

- DATEADD("year", 3, [Order Date])
- DATEADD("month", 6, [Order Date])
- DATEDIFF("day", [Order Date], [Shipping Date])
![daystoship](https://github.com/user-attachments/assets/24f7cf7d-a5d8-4457-8d5f-582e67e48ef5)
[See the interactive worksheet](https://public.tableau.com/app/profile/ayse.gocer/viz/Ayse_Dynamic_WorkSheet_19/DATEADD?publish=yes)

Example 18: Null Functions:

**ZN** replaces Null values with Zero. (Works just for numbers)
- ZN([Sales])

**IFNULL** replaces Null values with any given value (Works both numbers and strings)
- IFNULL([Sales], 0)
- IFNULL([Sales], 1)
- IFNULL([Country], "N/A")

**ISNULL** returns True or False. ISNULL returns True for Null values.
- ISNULL([Sales])

Example 19: Logical Functions: "IF, ELSEIF, IIF" support **any data type**, but "CASE WHEN" supports only **string**. "And" returns True if **both** conditions are True, but "OR" returns True if **at least** one condition is True. Attribute function ATTR() aggregates the values of **Dimensions**. ATTR() might also be used to check the quality of data.

- IF [Sales] > 1000 THEN "HIGH" ELSE "LOW" END
- IF [Sales] > 1000 THEN "HIGH" ELSEIF [Sales] > 500 THEN "MEDIUM" ELSE "LOW" END
- CASE [Country] WHEN "Turkiye" THEN "TR" WHEN "Canada" THEN "CA" WHEN "Germany" THEN "DE" ELSE "n/a" END
- IIF([Sales] > 1000, "HIGH", "LOW")
- IF SUM([Sales]) > 200000 THEN "green" ELSEIF SUM([Sales]) > 100000 THEN "orange" ELSE SUM([Sales]) <= 100000 THEN "red" END
- IF [Sales] > 1000 **AND** [Country] = "Germany" THEN "HIGH" END
- IF [Sales] > 1000 **OR** [Country] = "Germany" THEN "HIGH" END
- IF [Sales] > 1000 **AND** [Country] = "Germany" THEN [Sales] END
- IF **NOT** [Country] = "Germany" THEN [Sales] END
- ATTR([Postal Code])

Example 20: LOD Functions:

- Fixed:
{ FIXED [Customer_ID] : COUNT([Order_ID]) }
![customer_royalty](https://github.com/user-attachments/assets/e8086383-1b4f-4536-841b-68f923a7691d)
[See the interactive worksheet](https://public.tableau.com/app/profile/ayse.gocer/viz/AyseGocer_dynamic_worksheet_20/HistogramCustomerLoyalty?publish=yes)

- Exclude:
{ EXCLUDE [Sub_Category]: SUM([Sales of Tables])}
![exclude](https://github.com/user-attachments/assets/07bb6105-74d3-449d-9bbc-9ca83cfeb67b)
[See the interactive worksheet](https://public.tableau.com/app/profile/ayse.gocer/viz/AyseGocer_dynamic_worksheet_21/ComparativeSalesAnalysisbyCategory?publish=yes)

Example 21: Table Calculations (First, Last, Index, Rank)

- First()
- Last()
- Index()
- Rank(SUM([Sales]))
![table_calc](https://github.com/user-attachments/assets/5e4697f6-94d7-46e9-9e6d-e51ae137c374)

[See the interactive worksheet](https://public.tableau.com/app/profile/ayse.gocer/viz/Ayse_Dynamic_WorkSheet_22/TableCalculations?publish=yes)

[See the interactive worksheet](https://public.tableau.com/app/profile/ayse.gocer/viz/Ayse_Dynamic_WorkSheet_23/TABLECALC_?publish=yes)
