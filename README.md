Instructions on how to run the system:

1. After downloading the project, Open the solution in Visual Studio and build the project.

2. Build the project as given below sequence. 
   . build the DAL project first
   . build the Services project
   . build the Assignment project.
   
3. Now run the solution and access the URL : http://localhost:37235/EquipmentType

4. All the equipment list gets loaded and now user can add to cart any of it.

5. When user will click on Add to Cart link then user will get redirected to the cart page and user need to add the rental days for the particular equipment which they need to rent.

6. Find the logging details at : C:\AppLog.txt file.

7. After adding necessary equipment, user can click on Print Invoice link and then invoice get downloaded in text format as per the given below example of calculation.

Example:

There are three different fees:

• One-time rental fee – 100€
• Premium daily fee – 60€/day
• Regular daily fee – 40€/day


The price calculation for different types of equipment is:
• Heavy – rental price is one-time rental fee plus premium fee for each day rented.
• Regular – rental price is one-time rental fee plus premium fee for the first 2 days plus regular fee for the number of days over 2.
• Specialized – rental price is premium fee for the first 3 days plus regular fee times the number of days over 3.

Loyalty points
Customers get loyalty points when renting equipment. A heavy machine gives 2 points and other types give one point per rental (regardless of the time rented).

Scenario 1 : User can ask 3 different type of equipment at the same time.

Heavy : rent for 3 days
Amount : 100€ one-time rental fee + (3 * 60€/day premium fee) = 280€

Regular : rent fot 4 days
Amount : 100€ one-time rental fee + (2 * 60€/day for 2 days premium fee) + (2 * 40€/day regular fee) = 300€

Specialized : rent for 5 days
Amount :  0€ + (3 * 60€/day for 2 days premium fee) + (2 * 40€/day regular fee) = 260€

Loyality Points : 
Heavy : 2 points 
Regular : 1 point
Specialized : 1 point

Total Amount = 280 + 300 + 260 = 840€
Total Loyality points = 4 points

