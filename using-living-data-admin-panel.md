# Using Living Data Admin Panel

> The Living Data admin panel is accessible at [https://mylivingdata.com](https://mylivingdata.com)

As an administrator, you should have access to the Living Data web site, which includes administration functions for keeping track of participants and devices.

## Reset Password

Enter your administration email address into to website to receive a new login link.s

## Import Participants

The system is designed to run independently of any other participant system, so participants need to be imported before any deployment begins.

1. [ ] **Import participants using a CSV file with the following headings:** 
2. id - student identifier, or number. This must match the id imported into Intake24.
3. firstname
4. lastname
5. email - email of participant so that we can send them password reset and introduction emails.
6. group - some kind of identifier for the deployment group they are part of, can be anything as long as participants in the same group have the same value.
7. collect - Collection time for this group \(i.e. the time at which the device should start recording data\)
8. return - Return time for this group \(i.e. the time at which the device should stop recording data\).
9. [ ] Import participants into Intake24
10. [ ] Export participant login links from Intake24
11. [ ] **Upload login links to Living Data**

## Email Participants

Once participants are setup in the system using the steps above, you can initiate emailing them all with their introduction email, which includes a unique link for them to login.

Just visit [https://mylivingdata.com/users/sendintro/1](https://mylivingdata.com/users/sendintro/1) in your browser once you have logged in. Emails wil only be sent once, independent on how many times you have visited this link.

**DO NOT PRINT DUPLEX!**

## Print Functions

We advise setting up your sync workflow before any deployment starts.

You can print out the following documents:

* Box Labels:
  * Inidividual pages with deployment group information which can be used for labelling boxes of envelopes ready for collection.
* Registration Documents:
  * For a specific deployment group, individual pages for each participant which should be inserted into an envelope. These documents are used to program activity sensors for participants.
* Sign-out Sheet:
  * Printable document for a deployment group that should be used to sign-out devices when they are being collected by participants.
* Sign-In Sheet:
  * Printable document for a deployment group that should be used to sing back in devices when they are being returned by participants.

## Status List

The status list shows the current status of all participants. You can use this list to identify devices that have not returned, participants who are currently wearing sensors and other useful information to aid in the workflow.

To email a specific group of people, `filter` the list to display them, and then select `Export`

Selecting the `email` export option allows the text to be pasted into an email client directly.

