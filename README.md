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

SELECT * FROM Users;
SELECT name, email FROM Users;

**2. Apply WHERE, AND, OR, LIKE, BETWEEN**

WHERE is used to filter rows.
AND / OR are used for multiple conditions.
LIKE is used for pattern matching.
BETWEEN is used for range filtering.

SELECT * FROM ParkingSlots WHERE lot_id = 1 AND status = 'available';
SELECT * FROM Users WHERE email LIKE '%@gmail.com' OR email LIKE '%@yahoo.com';
SELECT * FROM Reservations WHERE start_time BETWEEN '2025-09-01' AND '2025-09-15';

**3. Sort with ORDER BY**

ORDER BY is used to sort results in ascending (ASC) or descending (DESC) order.

SELECT * FROM Users ORDER BY name ASC;
SELECT * FROM Reservations ORDER BY start_time DESC;
SELECT * FROM Payments ORDER BY amount DESC;

