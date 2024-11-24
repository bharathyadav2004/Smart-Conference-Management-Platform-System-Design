# Non-Functional Test Cases
Non-functional tests for the Smart Conference Management Platform (SCMP) could involve:
•	Performance Testing: Measure the response time and system stability under high load during peak event hours (e.g., 5000+ concurrent users accessing the platform for registration or session participation).
•	Security Testing: Validate that participant and organizer credentials are encrypted during login, ensure secure payment gateway integration for event registrations, and check compliance with GDPR for data storage and access permissions.
•	Usability Testing: Ensure the platform's user interface is intuitive, providing easy navigation for both organizers and participants. The UI should be accessible for all users, including those with disabilities.
•	Scalability Testing: Assess how well the platform scales when new events, sessions, and participants are continuously added over time without degradation in performance.
•	Reliability Testing: Verify that the platform remains stable and functional over extended periods of usage during long conferences and across multiple devices (mobile, web, etc.).
•	Compatibility Testing: Ensure the SCMP is compatible with various web browsers, operating systems, and devices, providing a seamless experience regardless of platform.

#Sequence Diagrams and Test Execution

For testing purposes, the sequence diagrams can cover scenarios like:
1.	Event Creation Flow: Organizer initiates event creation → Inputs details → Event saved in the system → Confirmation sent to organizer
2.	Participant Registration Flow: Participant searches for event → Registers → Payment processed → Ticket and confirmation email sent

# Test Suite Structure

•	Test Suite 1: Event Creation & Registration
o	Test cases include event creation, participant registration, payment processing
•	Test Suite 2: Session Management
o	Test cases include session creation, speaker assignment, and session scheduling
•	Test Suite 3: Notification and Alerts
o	Test cases cover email and SMS notifications during various actions like registration and event updates
•	Test Suite 4: Analytics and Feedback
o	Test cases on AI-powered analytics, feedback submission, and insights generation


Test ID	Test Description	Preconditions	Steps	Expected Result	Status
TC1	Test event creation	Organizer logged in	1. Login as organizer, 
2. Navigate to event creation, 
3. Input event details, 4. Save event	Event created successfully, listed on the dashboard	Pass
TC2	Test participant registration	Event is created	1. Login as participant, 
2. Search for event, 
3. Register, 
4. Complete payment	Participant registered; confirmation email sent	Pass
TC3	Test session creation and speaker assign	Event is created, Organizer in	1. Login, 
2. Navigate to session management, 
3. Create session, 
4. Assign speaker	Session created; speaker assigned	Pass
TC4	Test notification sending	Participant registered	1. Register for event, 2. Trigger email notification on confirmation	Confirmation email sent to participant	Pass
TC5	Test system under high load	5000+ users accessing platform	1. Simulate high load, 
2. Monitor response times	Platform response within 2 seconds	Pass

 
