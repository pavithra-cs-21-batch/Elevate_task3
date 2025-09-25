# Elevate_task3

**Entities and Attributes**

Users → user_id, name, phone, email, password
Vehicles → vehicle_id, user_id, vehicle_number, vehicle_type, color
ParkingLots → lot_id, name, location, total_slots
ParkingSlots → slot_id, lot_id, slot_number, status, slot_type
Reservations → reservation_id, user_id, slot_id, start_time, end_time, status
Payments → payment_id, reservation_id, amount, method, payment_time

**1. Use SELECT * and Specific Columns**

SELECT * is used to fetch all columns from a table.
We can also select only specific columns if needed.

SELECT * FROM Vehicle;

<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/a85d5ac4-fbd1-4258-a938-23179d9a8c4e" />

SELECT OwnerName, VehicleNumber FROM Vehicle;

<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/8d14b55c-6cb3-4976-b451-be511878e63a" />

**2. Apply WHERE, AND, OR, LIKE, BETWEEN**

WHERE is used to filter rows.
AND / OR are used for multiple conditions.
LIKE is used for pattern matching.
BETWEEN is used for range filtering.

SELECT * FROM ParkingSlot WHERE Status='Available';
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/d469a56e-2def-46a3-b21f-7aec9520b113" />

SELECT * FROM Booking WHERE Status='Active' AND PaymentStatus='Pending';
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/dc7d7e6b-6010-4f39-8572-c40257ce2f50" />

SELECT * FROM Vehicle WHERE VehicleType='Car' OR VehicleType='Bike';
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/e13dfdce-1cff-4f91-9313-abe2d06cbcc9" />

SELECT * FROM Vehicle WHERE OwnerName LIKE 'Pav%';
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/ed9c5dc8-ad74-49c7-b470-73c0871521ec" />

SELECT * FROM Payment WHERE Amount BETWEEN 50 AND 100;
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/3ea3703b-ddf7-40f5-9fd2-61ce967d61cb" />


**3. Sort with ORDER BY**

ORDER BY is used to sort results in ascending (ASC) or descending (DESC) order.

SELECT * FROM Payment ORDER BY Amount ASC;
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/bff2822f-0a1a-4235-baf4-eed8c41e1f97" />

SELECT * FROM Booking ORDER BY StartTime DESC;
<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/0fa789dc-162d-410e-9d8e-d05513917ac8" />


