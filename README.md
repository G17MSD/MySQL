# MySQL
use aircargo;
SELECT * FROM customer;
SELECT * FROM passengers;
SELECT * FROM route;
SELECT * FROM ticket_details;
INSERT into customer(customer_id,first_name,last_name,date_of_birth,gender)
VALUES (3,'Morris','Lois','1993-12-09','M'),
(4,'Cathenna','Emily','1977-09-14','F');
INSERT into passengers(aircraftID,routeID,customerID,departure_location,arrival_location,seat_number,class_ID,travel_date,flight_num)
VALUES(2,'A321',34,'CRW','COD','01B','Business',2019-01-26,1117), (8,'A321',38,'CST','DAL','02EP','Economy Plus',2020-09-28,1148);
alter table passengers modify column routeID varchar (50);
describe passengers;
alter table passengers modify column seat_number varchar(5);
alter table passengers modify column class_ID varchar(15);
alter table passengers modify column travel_date varchar(15);
INSERT into route(route_ID,flight_num,origin_airport,destination_airport,aircraft_ID,distance)
VALUES(1,1111,'EWR','HNL','767-301ER',4962);
alter table route modify column route_ID int;
delete from passengers where aircraftId=2;
