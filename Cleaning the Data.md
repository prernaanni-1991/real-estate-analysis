![alt text](https://ineuron.ai/images/ineuron-logo.png)

# Real Estate Analysis


### Data Gathering



### Data Cleaning
1. added index.
2. reorded.
3. duplicate and name as property type.
4. keep index and proprty_type coloumn and remove all.
5. duplicate and name as overlooking.
6. keep index and  overlooking coloumn and remove all.
7. In 'Furnishing' column replace blank cell by 'Not Declared'.
8. In 'Car Parking' column replace 'Open' by 'uncovered'.
9. In 'Car Parking' column replace blank by 'Not Declared'.
10. In 'Availability' column, use conditional column :
     If 'Availability' equals From Jan '23 Then One month,
     Else If 'Availability' equals From Feb '23 Then Two months,
     Else If 'Availability' equals From Mar '23 Then Three months,
    Else If 'Availability' equals From Apr '23 Then Four months,
    Else If 'Availability' equals From May '23 Then Five months
    Else Immediately.
11. Rename 'custom' by 'Availability.' and delete old one.
12. Rename 'Carpet Area' by 'Carpet Area in sqft'
13. Replace 'sqft' by blank in 'carpet area' column.
14. change datatype of thre same.
15. In 'Floor' column, replace Ground by 0, Upper Basement by -1 and Lower Basement by -2.
16. Split ' Floor' column.
17. In second ' floor' column replace 'out of' by blank.
18. Rename Floor.2 by 'total no of floors'.
19. Rename 'Super Area' by 'Super Area in Sqft'.
20. In 'Super Area in Sqft' column, replace sqft by blank.
21. In 'Super Area in Sqft' column, replace 45 sqyrd by 405 (45*9 = 405)
22. In 'Super Area in Sqft' column, change the datatype to numbers.
23. In 'Ownership' column, replace blanks by 'Not Declared'.
24. In 'Owner Resides' column, replace blanks by 'Others'.
25. In 'Dimensions' replace 'ft Sqft' by blanks.
26. Split 'Dimensions' column and multiply them using custom column and remove the previous one. Keep datatype as Decimal Numbers.
27. In 'Price' column, remove currency symbol and split by space.
28. Replace Lac by 100000 and null by 1 in 'Price.2' column, and then multiply Price.1 and Price.2 column and name as Final_Price. 
    After that, remove the columns Price.1 and Price.2.

29. In Property_Type table, split 'Property_Type' column by 'BHK'.
30. In Property_Type table, split 'Property_Type.2.1' column by 'SPACE'.
31. In Property_Type table, split 'Property_Type.2.2' column by 'comma'.
32. In Property_Type table, remove 'floor' in 'Property_Type.2.2.1' column.
33. In Property_Type table, remove 'for Rent in' in 'Property_Type.2.2.1' column.

34. In Overlooking table, replace 'Garden/Park' by 'Garden' and split the column by comma.
35. In Overlooking table, unpivot columns by selecting them and rename 'value' column by 'overlooking'.
36. 




































### Data Preparation


