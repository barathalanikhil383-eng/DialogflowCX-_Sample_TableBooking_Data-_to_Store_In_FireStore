# DialogflowCX-_Sample_TableBooking_Data-_to_Store_In_FireStore
This is a sample node.js webhook code for storing the table booking data to a cloud firestore database.
To do this, 1st we need to grant the IAM permissions to our CLoud Storage.

      **Go to IAM & Admin: In the Google Cloud Console, go to the IAM page.**

      Grant Permissions: * Find the service account email you identified in Step 1.

      Click the "Edit" (pencil) icon.

      Click "Add Another Role."

      Search for and select Cloud Datastore User (this is the standard role for Firestore access).
