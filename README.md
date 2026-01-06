# DialogflowCX-_Sample_TableBooking_Data-_to_Store_In_FireStore
This is a sample node.js webhook code for storing the table booking data to a cloud firestore database.
To do this, 1st we need to grant the IAM permissions to our CLoud Storage.

      **Go to IAM & Admin: In the Google Cloud Console, go to the IAM page.**

      Grant Permissions: * Find the service account email you identified in Step 1.

      Click the "Edit" (pencil) icon.

      Click "Add Another Role."

      Search for and select Cloud Datastore User (this is the standard role for Firestore access).

Run this below code in cloud shell:-
     gcloud functions deploy helloHttp \
  --runtime nodejs20 \
  --entry-point helloHttp \
  --trigger-http \
  --allow-unauthenticated \
  --region us-central1

  If it asks for authenticate with project ID - follow the steps given in cloudshell.[like- give projectID] and save.


  If your webhook wants to read paramerts, while calling paramters use `   ` symbol to call it. Not a parameter, what ever you want to call use this ` symbol only.

  Examples:-- 
       1- To call the text to display in the output:--             `The weather in ${weatherDetails.location} is ${weatherDetails.weather_descriptions} with a temperature of ${weatherDetails.temperature}.`

          2- To cal the usrl:-  const weatherUrl = `https://api.weatherstack.com/current?query=${encodeURIComponent(location)}&access_key=04fc2b59d4c3ccae0def30222a7280ff`;

