![alt text](https://ineuron.ai/images/ineuron-logo.png)

# Analysis of Rental Properties on MagicBricks.com 


### Data Gathering
1. Go to the following link:
https://www.magicbricks.com/property-for-sale-rent-in-Bangalore/residential-real-estate-Bangalore?mbtracker=google_paid_brand_1_desk_bangalore&ccode=brand_1_sem&gclid=Cj0KCQiAw8OeBhCeARIsAGxWtUz1ORYSYFj2QXCg0gi5SgEzC8rPkiN8-MiQ0KBGnSZk3G0BMIaQ6ssaAm_mEALw_wcB

2. Try to inspect each element and scrape using python. The code is available in the folder 'datasets'.



### Data Cleaning &Preparation
3. Add indexing.
4. Reorder and move index column to left most column.
5. Duplicate the Table and name as Property_Type.
6. keep index and Proprty_Type column and remove all other columns.
7. Duplicate the main Table and name as Overlooking.
8. keep index and  Overlooking coloumn and remove all other columns.
9. In 'Furnishing' column, replace blank cell by 'Not Declared'.
10. In 'Car Parking' column, replace 'Open' by 'uncovered'.
11. In 'Car Parking' column, replace blank by 'Not Declared'.
12. In 'Availability' column, use conditional column :
     If 'Availability' equals From Jan '23 Then One month,
     Else If 'Availability' equals From Feb '23 Then Two months,
     Else If 'Availability' equals From Mar '23 Then Three months,
    Else If 'Availability' equals From Apr '23 Then Four months,
    Else If 'Availability' equals From May '23 Then Five months
    Else Immediately.
13. Rename 'custom' by 'Availability.' and delete old one.
14. Rename 'Carpet Area' by 'Carpet Area in sqft'
15. Replace 'sqft' by blank in 'carpet area' column.
16. Change datatype of the columns accordingly.
17. In 'Floor' column, replace Ground by 0, Upper Basement by -1 and Lower Basement by -2.
18. Split ' Floor' column.
19. In second ' floor' column replace 'out of' by blank.
20. Rename Floor.2 by 'total no of floors'.
21. Rename 'Super Area' by 'Super Area in Sqft'.
22. In 'Super Area in Sqft' column, replace sqft by blank.
23. In 'Super Area in Sqft' column, replace 45 sqyrd by 405 (45*9 = 405)
24. In 'Super Area in Sqft' column, change the datatype to numbers.
25. In 'Ownership' column, replace blanks by 'Not Declared'.
26. In 'Owner Resides' column, replace blanks by 'Others'.
27. In 'Dimensions' column, replace 'ft Sqft' by blanks.
28. Split 'Dimensions' column and multiply them using custom column and remove the previous one. Keep datatype as Decimal Numbers.
29. In 'Price' column, remove currency symbol and split by space.
30. Replace Lac by 100000 and null by 1 in 'Price.2' column, and then multiply Price.1 and Price.2 column and name as Final_Price. 
    After that, remove the columns Price.1 and Price.2.

31. In Property_Type table, split 'Property_Type' column by 'BHK'.
32. In Property_Type table, split 'Property_Type.2.1' column by 'SPACE'.
33. In Property_Type table, split 'Property_Type.2.2' column by 'comma'.
34. In Property_Type table, remove 'floor' in 'Property_Type.2.2.1' column.
35. In Property_Type table, remove 'for Rent in' in 'Property_Type.2.2.1' column.

36. In Overlooking table, replace 'Garden/Park' by 'Garden' and split the column by comma.
37. In Overlooking table, unpivot columns by selecting them and rename 'value' column by 'overlooking'.
38. Delete unwanted columns as per the requirement.
39. Click on 'manage relationships' and check the relationships between 3 tables.
40. Go to Report view and start Visualization.



