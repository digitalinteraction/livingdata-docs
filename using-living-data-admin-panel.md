# Living Data Admin Panel

> The Living Data admin panel is accessible at [https://mylivingdata.com](https://mylivingdata.com)

As an administrator, you should have access to the Living Data web site, which includes administration functions for keeping track of participants and devices.

## Reset Password

## Import Participants

The system is designed to run independently of any other participant system, so participants need to be imported before any deployment begins.

1. Import participants using a CSV file with the following headings: 
   1. id - student identifier, or number. This must match the id imported into Intake24.

   2. firstname

   3. lastname

   4. email - email of participant so that we can send them password reset and introduction emails.

   5. group - some kind of identifier for the deployment group they are part of, can be anything as long as participants in the same group have the same value.

   6. collect - Collection time for this group \(i.e. the time at which the device should start recording data\)

   7. return - Return time for this group \(i.e. the time at which the device should stop recording data\).

## Print Functions



