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

Example 9: Lower case - Upper case strings (UPPER, LOWER):
[See the interactive worksheet](https://public.tableau.com/app/profile/ayse.gocer/viz/AyseGocer_dynamic_worksheet_8/LowerUpper?publish=yes)

Example 10: Removing unwanted space from the text (LTRIM, RTRIM, TRIM, COUNTD):
[See the interactive worksheet](https://public.tableau.com/app/profile/ayse.gocer/viz/AyseGocer_dynamic_worksheet_9/LTRIMRTRIMTRIM?publish=yes)

Example 11: Extract particular field from a string (LEFT, RIGHT, MID):
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
![date_functions](https://github.com/user-attachments/assets/b03da04e-b5fb-4936-b36a-f923c5e12ce0)
[See the interactive worksheet](https://public.tableau.com/app/profile/ayse.gocer/viz/Ayse_Dynamic_WorkSheet_17/DATEFUNCTIONS?publish=yes)
