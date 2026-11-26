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
* The system shall allow users to view their existing bookings.
* The system shall prevent conflicting bookings for the same facility and time.
* The system shall allow authorized staff to update booking information.
* The system shall allow staff to view booking information when responding to user queries.

#### Non-Functional Requirements
* The system shall require users to log in and only allow authorised staff to access admin functions.
* The system shall be easy to use and accessible to all users.
* The system shall protect users personal and booking information.
* The system shall keep booking information accurate and up to date.
* The system shall be available when users need to check facility availability and make bookings.
* The system shall be maintainable so that technical issues and system updates can be handled.

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

### Requirement 6
Original requirement: The system shall allow users to view their existing bookings.

**What is the problem?**

Does not explain what booking information users can view or whether they can only see their own bookings.

**Clarification question**

What booking information should users be able to see when viewing their existing bookings?

**Important missing information**
* Can users only view their own bookings?
* What booking details should be displayed?
* Should the booking status be shown?
* Can users view past and upcoming bookings?

**Improved requirement**

The system shall allow users to view their own bookings, including the facility name, booking date, time and booking status.

**How could it be verified?**

Log in as a user and check that they can view their existing bookings with the correct details. Also check that they cannot view another user's bookings.

### Requirement 7
Original requirement: The system shall prevent conflicting bookings for the same facility and time.

**What is the problem?**

Does not explain what counts as a conflicting booking or how the system should handle overlapping booking times.

**Clarification question**

How should the system handle bookings that overlap with an existing booking for the same facility?

**Important missing information**

* Should the system prevent partially overlapping bookings?
* Should it prevent bookings with exactly the same time?
* Can different facilities be booked at the same time?
* Do cancelled bookings still block the facility's availability?

**Improved requirement**

The system shall prevent users from booking a facility if the selected date and time overlap with an existing confirmed booking for the same facility.

**How could it be verified?**

Create a booking for a facility, then try to book the same facility for an overlapping time. Check that the system prevents the second booking.

### Requirement 8
Original requirement: The system shall allow authorized staff to update booking information.

**What is the problem?**

Does not explain which staff members are authorized or what booking information they are allowed to change.

**Clarification question**

What booking information should authorized staff be able to update?

**Important missing information**

* Which staff members can update bookings?
* Can staff change the facility, date and time?
* Can staff update the booking status?
* Should the system check facility availability before saving changes?
* Should changes made by staff be recorded?

**Improved requirement**

The system shall allow authorized staff to update booking details, including the facility, date, time and booking status, subject to facility availability.

**How could it be verified?**

Log in as authorized staff and try to update an existing booking. Check that the changes are saved and that conflicting booking times are not allowed. Also check that normal users cannot update other users' bookings.

### Requirement 9
Original requirement: The system shall allow staff to view booking information when responding to user queries.

**What is the problem?**

Does not explain how staff can find a booking or what information they need to see when responding to user queries.

**Clarification question**

How should staff search for a booking and what information should they be able to view?

**Important missing information**

* Can staff search using the user's name?
* Can staff search using a booking reference?
* What booking details should be displayed?
* Can all staff members access booking information?
* Should staff be able to view both current and past bookings?

**Improved requirement**

The system shall allow authorized staff to search for and view booking information using a user's name or booking reference, including the facility name, booking date, time and booking status.

**How could it be verified?**

Log in as authorized staff and search for a booking using a user's name or booking reference. Check that the correct booking information is displayed and that unauthorized users cannot access it.

## 4. Functional Requirements

**FR01: The system shall allow users to view the availability of a facility for a selected date and time.**
> Source: Customers
> Verification: Select a facility, date and time and check that the correct availability is displayed.

**FR02: The system shall allow users to book an available facility for a selected date and time.**
> Source: Customers
> Verification: Select an available facility and time and create a booking. Check that the booking is recorded and the facility is no longer shown as available for that time.

**FR03: The system shall allow users to cancel their booking according to the applicable cancellation rules.**
> Source: Customers / Booking Staff
> Verification: Create a booking and cancel it according to the applicable rules. Check that the booking is cancelled correctly.

**FR04: The system shall allow authorised staff to update facility availability and manage booking rules.**
> Source: Booking Staff
> Verification: Log in as authorised staff, update facility availability and booking rules, and check that the changes are saved correctly.

**FR05: The system shall notify users when their booking is confirmed or cancelled.**
> Source: Customers
> Verification: Create a booking and check that the user receives a confirmation notification. Then cancel the booking and check that the user receives a cancellation notification.

**FR06: The system shall allow users to view their own bookings, including the facility name, booking date, time and booking status.**
> Source: Customers
> Verification: Log in as a user and check that they can view their existing bookings with the correct details. Also check that they cannot view another user's bookings.

**FR07: The system shall prevent users from booking a facility if the selected date and time overlap with an existing confirmed booking for the same facility.**
> Source: Booking Staff
> Verification: Create a booking for a facility, then try to book the same facility for an overlapping time. Check that the system prevents the second booking.

**FR08: The system shall allow authorised staff to update booking details, including the facility, date, time and booking status, subject to facility availability.**
> Source: Booking Staff
> Verification: Log in as authorised staff and try to update an existing booking. Check that the changes are saved and conflicting booking times are not allowed.

**FR09: The system shall allow authorised staff to search for and view booking information using a user's name or booking reference, including the facility name, booking date, time and booking status.**
> Source: Booking Staff
> Verification: Log in as authorised staff and search for a booking using a user's name or booking reference. Check that the correct booking information is displayed.

## 5. Quality Requirements

**NFR-01: The system shall protect users' personal and booking information from unauthorised access.**
> Why does it matter? Users' personal information needs to be protected.
> How could it be checked? Test the system using a normal user account and an authorised staff account and check that users cannot access information or functions they are not authorised to access.

**NFR-02: The system shall let users book a facility by themselves.**
> To make booking easier for users and reduce staff workload.
> Ask new users to make a booking and observe whether they can complete it without help.

## 6. Project Application

## 7. Reflection
