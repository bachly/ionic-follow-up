Ionic Follow Up

An app to manage how often a contact should be followed up

Basic fucntions:
- User logins with email address
- User creates a group and assign leaders
- Leaders login with email address
- Leaders CRUD a contact and set up a follow-up cadence
- Cadence can be daily, weekly, fortnightly, monthly or quarterly.
    - The app shows the follow-up status in 3 colours: green, yellow, red.
        - Green means the contact has been followed-up within the cadence.
        - Yellow means a follow-up was missed once.
        - Red means a follow-up was missed twice.
- Leaders should try to keep all contacts in green status.

Advanced functions:
- Display a weekly calendar and show whom needs to be followed-up in each week.
- A system notification to show who needs to be followed-up this week.

Sharability:
- Invites other users to unlock Intermediate functions

Objects:
- Users - email address, audit
- Group - owner, leaders, groupName, Contacts, audit
- Contact 
    - name
    - description
    - bio (picture, dob, marital status, suburb, family members, interests, etc...)
    - cadence, cadenceStarts
    - notes (description, audit)
    - audit (actionType, actionedAt, actionedBy, actionDescription)

Permissions:
- A user can CRUD the contacts of the group in which they are one of the leaders or admins
- A user who is the admin of the group can CRUD the group
- A user can see the follow-up status of the contacts
- A user can share a link to the summary page of a contact
- Admin can transfer contact from one group to another

Technical:
App connects to Stripe to take payments.
App connects to Firebase for data storage and authentication.
App is hosted on Ionic Appflow for easy distribution to App Stores.