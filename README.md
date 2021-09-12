--------------------------------------------------------------------------------------------------------------
This query is to create tasks using Zapier for vehicles that didn't get tasks from internal task generation feature.

I removed detailed information such as cityId, battery range, status, etc. 


Possible consequence if task doesn't get generated
Vehicles with low batery % can cause the following:
1. Riders can't ride therefore lead to decrease in revenue.
2. Increase the possibility of loss of a vehicle.
--> We can't guarantee when staff will swap the battery of a vehicle. It will lead to disconnection of IoT if the battery doesn't get swapped until it it discharges. 



Task should be created at least in last 24 hours ideally. 

--------------------------------------------------------------------------------------------------------------

** 24 **
- scooters made within 24 hours of NOW + currently open

** low_bat **
- main portion where batt percentage settings are set
- For new cities/geofences add necessary statements:
  - Check the following columns:
    - priority
    - points
  - Check the case statement in the where portion
*/
