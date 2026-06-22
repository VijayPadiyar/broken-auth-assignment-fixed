# The Silent Server (Backend Debugging Assignment)

## Assignment Objective

The goal is to fix the broken authentication endpoints so that a user can:
1.  **Login** to get a session ID and OTP.
2.  **Verify the OTP** to get a valid session cookie.
3.  **Exchange the Session** for a JWT Access Token.
4.  **Access Protected Routes** using the token.

## Expected Output

After fixing the bugs, you should be able to run the following sequence successfully:

1.  **Login**: Receive a `loginSessionId` and see an OTP in the server logs.
2.  **Verify OTP**: Receive a session cookie (`session_token`).
3.  **Get Token**: Exchange the session cookie for a JWT (`access_token`).
4.  **Access Protected Route**: Use the JWT to get a 200 OK response with user details and a **unique Success Flag**.
