# Infosys Springboard Internship 7.0

## Batch 4 — Milestone 1: User Authentication Module

### 1. Project Overview

Milestone 1 focuses on developing a user authentication module using Streamlit, JWT, ngrok, Gmail OTP, and Google Colab. The application provides user registration, login, password recovery, session management, and an admin dashboard.

### 2. Features

- **Login Page:** Authenticate users with their username/email and password.
- **Signup Page:** Register new users with a unique username, email, password, confirmation password, security question, and security answer.
- **Forgot Password:** Recover accounts using either a security question or an email OTP.
- **JWT Session Management:** Generate and validate JWT tokens after successful login.
- **Input Validation:** Validate mandatory fields, email format, password strength, and password confirmation.
- **User Dashboard:** Display a welcome message with the logged-in user's username/email and provide a logout option.
- **Admin Dashboard:** Provide a separate admin login and display registered usernames and email addresses without exposing passwords.
- **Email OTP Verification:** Send a one-time password to the registered email address for account recovery.

### 3. Technology Stack

- **Programming Language:** Python
- **Frontend and Application Framework:** Streamlit
- **Authentication and Session Management:** JSON Web Token (JWT)
- **Development Environment:** Google Colab
- **Public Access:** ngrok
- **Email Verification:** Gmail SMTP and Gmail App Password
- **Secret Management:** Google Colab Secrets

### 4. Application Pages

1. Login Page
2. Signup Page
3. Forgot Password Page
4. User Dashboard
5. Admin Dashboard

### 5. Validation Requirements

- All mandatory fields must be completed before submission.
- Email addresses must follow the specified email format rule.
- Passwords must contain at least eight characters, one uppercase letter, one lowercase letter, one number, and one special symbol.
- Confirm Password must exactly match Password.
- Duplicate usernames must be rejected during signup.
- Login failures must display a generic error message.

### 6. Password Recovery

The application supports two password recovery methods:

**Security Question Method**

- Enter the registered username.
- Answer the security question selected during signup.
- Set a new password that satisfies the password rules.

**Email OTP Method**

- Enter the registered email address.
- Receive a one-time password by email.
- Verify the OTP and set a new password.

After a successful password reset, the user is redirected to the Login page.

### 7. How to Run the Application

1. Open the project notebook in Google Colab.
2. Configure the required credentials in Colab Secrets.
3. Run the notebook cells in order to install dependencies and configure the application.
4. Start the Streamlit application and establish the ngrok tunnel.
5. Open the generated public URL in a browser.
6. Test signup, login, password recovery, the user dashboard, and the admin dashboard.

### 8. Screenshots

Screenshots demonstrating the application will be added after implementation and testing.

- Login Page
- Signup Page
- Forgot Password — Security Question
- Forgot Password — OTP
- OTP Email
- User Dashboard
- Admin Dashboard

Screenshots will be stored in the `screenshots/` folder.

### 9. Security Considerations

- Store JWT secrets, ngrok authentication tokens, email credentials, and other sensitive values in Google Colab Secrets.
- Do not hard-code personal credentials or secrets in the notebook.
- Never display or expose user passwords in the admin dashboard.
- Clear notebook outputs before uploading the notebook to GitHub.
- Verify that no personal credentials, tokens, OTPs, or admin passwords remain in the submitted notebook.

### 10. Project Deliverables

- `README.md` — Project documentation and instructions.
- Jupyter notebook (`.ipynb`) — Application implementation.
- `screenshots/` — Screenshots of the tested application pages.

### 11. Conclusion

This milestone demonstrates the implementation of a user authentication module with registration, login, secure session handling, password recovery, email OTP verification, and administrative user management using Python-based tools.

