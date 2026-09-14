# International Airport Database — ERD

## Database Course — Laboratory Work 1

This project contains an Entity-Relationship Diagram (ERD) and documentation for an International Airport Database.

## Entities

The database contains the following main entities:

1. **Airport**
2. **Airline**
3. **Flight**
4. **Passenger**
5. **Booking**
6. **BoardingPass**
7. **Baggage**
8. **BaggageCheck**
9. **SecurityCheck**
10. **BookingFlightChange**

## Main Relationships

* One **Airline** can operate many **Flights**.
* One **Airport** can be the departure airport for many **Flights**.
* One **Airport** can be the arrival airport for many **Flights**.
* One **Passenger** can have many **Bookings**.
* One **Flight** can have many **Bookings**.
* One **Booking** can have zero or one **BoardingPass**.
* One **Booking** can have zero or many **Baggage** records.
* One **Booking** can have zero or many **BaggageCheck** records.
* One **Passenger** can have zero or many **BaggageCheck** records.
* One **Passenger** can have zero or many **SecurityCheck** records.
* One **Booking** can have zero or many **BookingFlightChange** records.

## Keys and Constraints

* Each entity has a **Primary Key (PK)**.
* Foreign Keys (**FK**) are used to connect related entities.
* Required attributes are marked as **NOT NULL**.
* Unique attributes, such as `airline_code` and `passport_number`, are marked as **UNIQUE**.
* `BookingFlightChange` stores the history of flight changes for a booking.

## Files

* `ERD/airport_erd.png` — Entity-Relationship Diagram.
* `Documentation/International_Airport_Database_ERD_Lab1_Revised.pdf` — Complete laboratory work documentation.

## Modeling Notes

The system description mentions accounts, booking legs, aircraft information, and frequent flyer programs, but does not provide enough specific attributes or relationships to model them reliably. Therefore, they are not included as separate entities in this ERD.

`BookingFlightChange` is included as a separate entity because the assignment explicitly requires storing flight booking changes.

## Course

**Database Course — Laboratory Work 1**

**Topic:** Entity-Relationship Diagram (ERD)

**Database:** International Airport Database
