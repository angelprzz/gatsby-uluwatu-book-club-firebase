# Uluwatu Book Club - **Firebase Functions**

This project will allow you to run **Firebase Functions** in the **Uluwatu Book Club** project.

**Full code at https://github.com/angelprzz/gatsby-uluwatu-book-club**

## How to install
1. Download or clone the project.
2. Go to `./functions` and install the dependencies with `npm install`.
3. Open **Google Cloud Platform** and select your Firebase project.
4. Go to **Identity and Access Management (IAM) API** and click on "Enable".
5. Navigate to **IAM Access**, go to the row with the name of "App Engine default service account" and click on the pen icon on the right.
6. Inside the **Edit permissions** tab add three roles:
    - Editor
    - Service Account Token Creator
    - Storage Object Creator


7. Back in the project, run `firebase login` and sign in with your Firebase account (you will need to have the Firebase CLI installed. You can install it with `npm install -g firebase-tools`).
8. Run `firebase deploy --only functions` to deploy the functions to your Firebase project.
