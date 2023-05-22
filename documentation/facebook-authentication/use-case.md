# Authentication with Facebook

> ## Data

- Access Token

> ## Default flow

1. ⏳ Get data (name, email, and Facebook ID) from Facebook API
2. ⏳ Check if there is a user with the email received above
3. ⏳ Create an account for the user with the data received Facebook
4. ⏳ Create an access token, from the user ID, with a 30-minute expiration
5. ⏳ Return the generated access token

> ## Alternate flow

- User already exists

  3.1. ⏳ Update the user account with the data received Facebook (Facebook ID and name - only update the name if the user account does not have a name)

> ## Exception flow

- Invalid or expired token

  1.1. ⏳ Return an authentication error
