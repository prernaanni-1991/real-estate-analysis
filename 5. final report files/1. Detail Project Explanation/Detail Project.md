![alt text](https://ineuron.ai/images/ineuron-logo.png)

# Analysis of Rental Properties on MagicBricks.com 

### Slicer1 :
Slicer showing Project names
**Field** : Project_name
**Style** : Dropdown

### Slicer2 :
Slicer showing Number of Balconies
**Field** : Balcony
**Style** : Between

### Slicer3 :
Slicer showing Number of Car Parking
**Field** : Car Parking
**Style** : Dropdown

### Slicer4 :
Slicer showing Number of Bathrooms
**Field** : Bathroom
**Style** : Between

### Slicer5 :
Slicer showing Tenant Preferred
**Field** : Tenant Preferred
**Style** : Vertical list

### Table :
Table showing the facing of the respective properties.
**Columns** : Facing

### Card1 :
Card having total number of properties.
**Fields** : Count of total index

### Multirow Card :
Multirow Card showing the floor no. along with the total no of floors in each property.
**Fields** : Total no. of floors (**Filter** : show items when the value 'is not blank')
             Floor no.
             project_name

### Donut Chart : 
Donut chart showing the overlooking features for all the properties.
**Legend** : Overlooking (**Filter** : basic filtering by ignoring null values)
**Values** : Count of project_name

### Stacked Area Chart :
Stacked Area Chart showing top 5 locations having highest no. of rental properties.
**X-Axis** : Location
**Y-Axis** : Count of index

### Area Chart :
Area chart showing the Carpet & Super Area along with dimensions of each flat.
**X-Axis** : Dimensions
**Y-Axis** : Carpet Area in Sqft
**Secondary y-axis** : Super area in Sqft

### Pie Chart1 :
Pie chart showing the number of properties having freehold ownership.
**Legend** : Ownership
**Values** : count of project_name 

### Pie Chart2 :
Pie chart displaying the proportion of homes where the owner also lives there.
**Legend** : Owner RESIDES
**Values** : count of project_name 

### Clustered column chart :
Clustered column chart showing the availability of Rental Properties in each location.
**X-Axis** : Availability
**Y-Axis** : Count of Location

### Stacked column chart :
 Stacked column chart showing the condition of property and the property type (1BHK, 2BHK, 3BHK )
**X-Axis** : Furnishing 
**Y-Axis** : Count of Location
**Legend** : Property type

### Stacked bar chart :
S.tacked bar chart showing the rent of each property.
**X-Axis** : Average of Final_Price
**Y-Axis** : Project_name










































