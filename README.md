# Running a local instance
This application uses Vite to run a local dev server and to execute a build.

Step: 1
- from terminal execute `npm install`
Step: 2
- to start local dev server execute `npm run dev`

# Acceptance Criteria

A user should be able to enter a valid email address and a password in the form input fields, and see that the submit button become active. The submit button should be disabled until the following criteria are met:

- The email address must be in a valid format. For the purposes of this exercise, a valid format looks like: example@mail.com, with a name of at least one character, followed by an @ symbol, followed by a domain of at least one character, followed by .com.

- The password must be at least 6 characters long.

Once the submit button is active, it can be clicked and a user will be presented with a prompt that says “Login successful!”

Finally, when the user is typing their password, it should obfuscate the characters they are entering so that it appears as “*” character.
