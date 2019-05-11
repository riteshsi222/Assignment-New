
Instructions on how to run the system:

1. After downloading the files open it with Visual Studio and run in as administrator mode.

2. Kindly build the entire project and if you face any issue then first build the DAL project then Services project and after that Assignent project.

3. Once build is successfully done then run the project and browse the below local URL.
   http://localhost:37235/EquipmentType

4. On above link user can see equipment types and user can add to card by clicking on link Add To Cart and then user will navigate to the new page where they need to add the Rental days in it.

5. User can add all type of equipment with rental days and then they can generate their invoice after clicking on Print Invoice link and text file get downloaded which will show all the calculations as given below example.

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

----------------------------------------------------------------------------------------------------------------------------------
