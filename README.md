# Help, help! Where am I?

Node-RED flow that contains functionality for figuring out where a patient is located, and dispatching ambulances to the location by sending navigation details to ambulance drivers via Google Glass

## Getting started

### Prerequisites
* A cellphone with internet acccess
* A pair of Google Glasses
  1. *(Handled by course instructors)* The user account connected to the Glasses must be signed in at http://glassproxy.mybluemix.net/auth
  2. *(Handled by course instructors)* The userID of the account must be inserted into the URL of all HTTP requests made to glassproxy in the Node-RED flow. 
    * E.g. http://glassproxy.mybluemix.net/timeline/117059099648984892989
    * Check out this video to find out what your Google userID is:
      https://www.youtube.com/watch?v=dkPHxRDp9wY#t=47

### Deploy the example
1. Register for a trial account at http://bluemix.net (IBM's new PaaS offering, launched in July 2014)
2. Log in
3. Click on "CREATE AN APP"
4. Choose the Boilerplate Node-RED Starter
5. Give your app a name and click "Create"
6. After a few minutes your app will be running (App Health: Your app is running)
7. Go to: \<your_app_name\>.mybluemix.net
8. Click on "Go to your Node-RED flow editor"
9. In this GitHub repo: copy the text in exercise1.flow
10. In your Node-RED flow editor click on the menu button (top right)
11. Choose Import From -> Clipboard
12. Paste the text your copied in 9.
13. Click deploy

### Running the example
1. Open a browser and go to \<your_app_name\>.mybluemix.net/map
2. Open a browser on your cellphone and go to \<your_app_name\>.mybluemix.net/client
  * *OR* register for a trial account at http://www.twilio.com and insert your Twilio API key and your phone number into the SMS node. Click the Inject button on Send SMS to patient
3. In /client enter the patient's name and click "Start tracking"
4. View the patient's position in /map
5. Click the marker of the patient to dispatch an ambulance (Google Glass notification) 
