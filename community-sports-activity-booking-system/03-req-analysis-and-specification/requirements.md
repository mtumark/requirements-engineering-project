# Requirements Analysis and Specification

## 1. Information So Far
The organisation has different places that people can book, such as sports pitches, halls and courts.

Right now, bookings are done by phone, email, spreadsheets and calendars. This can cause problems like:

* conflicting or double bookings;
* difficulty checking facility availability;
* cancellations and no-shows;
* staff spending time answering booking questions;
* difficulty keeping booking information up to date;
* different facilities having different booking rules;
* concerns about protecting user information;
* accessibility and usability concerns.

The main people involved are:

* Users / Customers
* Booking Staff
* Community Management
* IT Staff
* Facility Maintenance Staff
* Event Organisers

Some things are still unclear, like who can book, when they can book, how long they can book, cancellation rules, no-shows, and payment.

## 2. Candidate Requirements
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

## 3. Requirements Surgery
### Requirement 1
Original requirement: The system shall let users check facility availability.

**What is the problem?**

Does not explain what information the user needs to select when checking availability.

**Clarification question**

What information should the user select when checking if a facility is available?

**Important missing information**

* Which facilities can users search for?
* Does the user select a date and time?
* Can users search for multiple facilities?
* Should unavailable times also be displayed?

**Improved requirement**

The system shall allow users to check the availability of a facility for a selected date and time.

**How could it be verified?**

Select a facility, date and time and check that the system correctly displays whether the facility is available or already booked.

### Requirement 2
Original requirement: The system shall let users book an available facility.

**What is the problem?**

We still don't know what details users need to book or what rules they must follow.

**Clarification question**

What information must users provide when booking a facility, and what booking rules apply?

**Important missing information**
* What information is needed to make a booking?
* How early can users book?
* How long can they book for?
* Do different facilities have different rules?
* Does staff need to approve the booking?

**Improved requirement**

The system shall allow users to book an available facility by selecting a facility, date and time, subject to the applicable booking rules.

**How could it be verified?**

Choose a facility, date and time, then make a booking. Check that the booking is saved and the facility is no longer available at that time.

### Requirement 3
Original requirement: The system shall let users cancel their bookings.

**What is the problem?**

Does not say when a booking can be cancelled or whether there are any cancellation rules.

**Clarification question**

How late can a user cancel a booking?

**Important missing information**
* Is there a deadline for cancelling?
* Do different facilities have different cancellation rules?
* What happens if someone does not show up?
* Can someone else book the facility after cancellation?

**Improved requirement**

The system shall allow users to cancel their booking according to the cancellation rules for the facility.

**How could it be verified?**

Make a booking and try to cancel it. Check if it is cancelled and if the facility is free again.

### Requirement 4
Original requirement: The system shall let authorised staff manage facility availability and booking rules.

**What is the problem?**

The requirement does not explain which staff members are authorised or what specific actions they can perform when managing facility availability and booking rules.

**Clarification question**

What actions should authorised staff be able to perform when managing facility availability and booking rules?

**Important missing information**
* Which staff can manage facilities?
* Can staff add, change or remove facilities?
* Can staff block a facility for maintenance?
* Who can change booking rules?
* Can staff change existing bookings?

**Improved requirement**

The system shall allow authorised staff to update facility availability and manage the booking rules for each facility.

**How could it be verified?**

Log in as staff and check if they can change facility availability and booking rules. Then log in as a normal user and check that they cannot change them.

### Requirement 5
Original requirement: The system shall send booking notifications.

**What is the problem?**

The requirement does not say who receives the notification, when it is sent or what information it contains.

**Clarification question**

When should users receive notifications about their bookings?

**Important missing information**
* Who gets the notification?
* Is a notification sent after booking?
* Is a notification sent after cancellation?
* Do users get reminders?
* Do staff also get notifications?
* Are notifications sent by email, SMS or other ways?

**Improved requirement**

The system shall notify users when their booking is confirmed or cancelled.

**How could it be verified?**

Create and cancel a booking and check that the appropriate notification is sent to the user.

## 4. Functional Requirements

## 5. Quality Requirements

## 6. Project Application

## 7. Reflection
