# Intial Discovery

## 1. Facts
* The community organisation manages different facilities, including sports pitches, sports halls, courts and other activity spaces.
* Currently booking are managed manually through phone calls, emails, spreadsheets and calendars.
* Currently they have difficulty when conflicting bookings.
* It consumes the time of the staff to answer booking quieries
* They have difficulty in keeping information up to date.
* Cancelation of booking is an issue.
* Different facilities have different rules on booking it.
* The organization need to protect user information.
* The organization is concern about accessibility and usability.

## 2. Assumptions
* The organization needs a mobile app for users to make and manage bookings.
* Staff will receive a notice or reminder when a booking is about to end.
* A user wants to easily know if a facility is available to be book.
* Users will be able to easily check the availability of facilities.
* Users will be able to create accounts to manage their bookings.

## 3. Unknowns
* Who can book the facilities?
* How early can users book a facility, and how long can they book it for?
* What personal information will the system collect, and who can see it?
* If a user keeps cancelling bookings or does not show up, what will happen?
* Do users need to pay online?

## 4. Stakeholders
* Users / Customers - Availability, easy booking and cancellation.
* Booking staff - Better bookings, fewer questions, and less work for staff.
* Community management - Fewer booking problems, happy customers, and accurate reports.
* IT - A reliable, secure system that is easy to maintain and fix.
* Facility maintenance - Maintenance schedules, facility availability, and repair notices.
* Event organizers - Easy booking, checking availability, and managing schedules.
* Vendors / Merchants - Available spaces, event permissions, and booking details.

## 5. Goals
* Streamline bookings
* Let users check availability and manage bookings to reduce staff work.
* Provide an accessible, secure and easy-to-use platform for users.

## 6. Scope
* Users can make, view, and cancel bookings.
* One system for booking facilities to avoid double bookings.
* Staff can manage facilities, schedules, and booking rules.
* Facilities can be booked for a specific date and time.
* Users can check available facilities and time slots.


## 7. Candidate Requirements
#### Functional Requirements
* The system shall let users check facility availability.
* The system shall let users book an available facility.
* The system shall let users cancel their bookings.
* The system shall let authorised staff manage facility availability and booking rules.
* The system shall send booking notifications.
#### Non-Functional Requirements
* The system shall require users to log in and only allow authorised staff to access admin functions.
* The system shall be easy to use and accessible to all users.
* The system shall protect users personal and booking information.

## 8. Requirements Surgery
**Requirement 1**
The system shall show users whether a facility is available or already booked for a selected date and time.

- How can it be verified?
Select a facility and date/time and check that the system correctly shows whether it is available or booked.

**Requirement 2**
The system shall allow new users to book a facility by choosing a facility, date, and available time within 3 minutes.

- How can it be verified?
Conduct usability testing to new users and measure how long it takes them to complete a booking without help.

**Requirement 3**
The system shall allow users to cancel their facility booking before the booking start time.

- How can it be verified?
Create a booking and attempt to cancel it before the start time. Check that the booking is cancelled and the facility becomes available again.


