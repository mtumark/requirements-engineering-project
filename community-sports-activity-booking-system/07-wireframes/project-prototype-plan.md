# Wireframes

## 1. ACTOR AND GOAL

Actor: User / Customer

Goal: The user wants to find a facility, check its availability, and make a booking for a selected date and time.


## 2. WHY THIS JOURNEY MATTERS

The project involves booking management. At the moment, bookings are handled through phone calls, emails, spreadsheets and calendars. This can cause problems like double bookings, difficulty checking availability, cancellations and no-shows. It can also create more work for staff, especially when the information is not updated properly.

A simple self-service booking system could help users check availability and make bookings more easily. It could also reduce some of the manual work that staff need to do.

The prototype will focus on one important user journey instead of showing all the functions of the system. It is a low-fidelity prototype, which means it shows the basic design and steps of the booking process but is not a working booking system.


## 3. PROPOSED PROTOTYPE SCREENS

SCREEN 1: BROWSE FACILITIES

Purpose:
Allow the user to browse facilities that may be booked, such as sports pitches, halls and courts.

Possible content:
- Facility name or type.
- A short description, if this is confirmed as useful.
- A "View Availability" button.

Requirement link:
- FR01: The system allows users to view availability of a facility for a selected date and time.

Open questions:
- What facility information should be displayed to help users choose?
- Should the system show details such as location, capacity or accessibility?
- What should be shown for a facility that is unavailable or temporarily closed?


SCREEN 2: FACILITY AVAILABILITY

Purpose:
Allow the user to select a facility and check its availability for a date and time.

Possible content:
- Selected facility.
- Date selection.
- Available or unavailable time slots, if availability is shown this way.

Requirement link:
- FR01: The system allows users to view availability of a facility for a selected date and time.

Open questions:
- How should availability be displayed?
- How frequently should availability be updated?
- Should users choose a date first, or select the date and time together?
- What should happen if another user books the same time while the user is making a booking?


SCREEN 3: CHOOSE DATE AND TIME

Purpose:
Allow the user to select the intended booking date, start time and end time.

Possible content:
- Selected facility.
- Booking date.
- Start and end time.
- A way to continue after selecting the details.

Requirement link:
- FR02: The system allows users to book an available facility for a selected date and time.

Open questions:
- Are there minimum or maximum booking durations?
- How far in advance can users book?
- What opening hours or facility-specific booking rules apply?
- What should happen if the selected time is no longer available?


SCREEN 4: REVIEW BOOKING DETAILS

Purpose:
Allow the user to check the selected facility, date and time before submitting the booking.

Possible content:
- Selected facility.
- Booking date and start/end time.
- A "Submit Booking" button.
- A way to go back and change the details.

Requirement links:
- FR02: The system allows users to book an available facility for a selected date and time.
- NFR-02: The system lets users book a facility by themselves.

Open questions:
- Does the user need to provide personal details or sign in before submitting?
- Which details should be displayed for the user to check?
- Is any additional validation required before submission?


SCREEN 5: AFTER SUBMISSION

Purpose:
Show the user what happened after they submitted the booking.

Possible content:
- A neutral message that the booking request or submission has been received.
- The selected facility and date/time, if appropriate.
- A clear next step, once the booking process is confirmed.

Requirement link:
- FR02: The system allows users to book an available facility for a selected date and time.

Open questions:
- Is a booking confirmed immediately, reviewed by staff, or handled another way?
- Should the system send a notification when a booking is confirmed or cancelled?
- What message should be shown if the submission fails?


## 4. OPEN QUESTIONS

The following questions need clarification before the prototype can be treated as a complete representation of the requirements.

1. Who is allowed to make a booking, and is an account or login required?
2. What facility information should be displayed to help users choose?
3. How should availability be displayed and how frequently should it be updated?
4. What should happen if a facility is unavailable or temporarily closed?
5. Are there minimum or maximum booking durations?
6. How far in advance can users book?
7. What opening hours or facility-specific rules apply?
8. What should happen if another user books the selected time while the user is making a booking?
9. What details must users review before submitting a booking?
10. Is a booking confirmed immediately or reviewed by staff?
11. How should cancellations and no-shows be handled?
12. Is payment required, and if so, when?
13. Should the system send notifications, and what events or channels should they cover?
14. What user information is necessary, and how should personal and booking information be protected?


The prototype should contain approximately four to six connected screens. Basic shapes and text are sufficient. The screens do not need to function as a real booking system.

Each screen should be linked to the project requirements where supported. Details that have not been confirmed should be recorded as open questions rather than treated as agreed rules.
