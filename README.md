

## To start setting up the project

Step 1: Clone the repo

```bash
git clone https://github.com/trulymittal/role-based-access-control
```

Step 2: cd into the cloned repo and run:

```bash
npm install
```

Step 3: Put your credentials in the .env file.

```bash
PORT=3000
MONGODB_URI=YOUR_MONGODB_URI(example: mongodb://localhost:27017)
DB_NAME=YOUR_DB_NAME
```

Step 4: Install MongoDB (Linux Ubuntu)

See <https://docs.mongodb.com/manual/installation/> for more infos

Step 5: Run Mongo daemon

```bash
sudo service mongod start
```

Step 6: Start the app by

```bash
npm start
```


Descriptions:


1. **Express.js**: A fast and lightweight web framework for Node.js that simplifies the process of building robust APIs and web applications. It provides a rich set of features for web and mobile applications, making it a popular choice for backend development.

2. **EJS Templating Engine**: Embedded JavaScript (EJS) allows developers to generate HTML with plain JavaScript. It integrates seamlessly with Express.js, enabling dynamic content rendering by embedding variables and JavaScript logic directly into HTML.

3. **Styling**: Custom CSS is used to design and style the application. Libraries like Bootstrap, Bulma, and Tailwind CSS can also be integrated to provide pre-styled components and utility classes for faster and responsive web development.

4. **Passport.js for Local Authentication**: Implements local authentication using email and password. Passport.js is a middleware that simplifies user authentication and supports multiple strategies (e.g., local, OAuth, etc.). It helps secure access to specific parts of the application.

5. **User Roles**: The system will have role-based access control with predefined roles such as Admin, Moderator, and Client. These roles dictate the permissions for accessing or modifying specific routes or resources.

6. **Authorization**: Implement role-based authorization to control access to specific routes based on user roles. For instance, only Admins can manage user accounts, Moderators can approve content, and Clients can view restricted data.

7. **Mongoose**: An Object Data Modeling (ODM) library for MongoDB and Node.js. It provides a schema-based solution to model your application data, perform validations, and interact with MongoDB efficiently.

8. **Express Sessions**: Sessions help maintain user state between HTTP requests by storing data server-side. Express-session middleware will be used to manage session data securely.

9. **Mongo Store for Persistent Sessions**: Use a MongoDB-backed session store to persist session data, ensuring that users stay logged in even after a server reboot or restart.

10. **Redirect to the Same Page After Login**: Implement logic to redirect users to the page they initially requested before logging in, enhancing the user experience.

11. **Server-Side Input Validation**: Validate user inputs such as email, password, and other form fields on the server side using libraries like express-validator. This prevents malicious or incorrect data from being processed.

12. **Flash Messages**: Temporary messages displayed to users for notifications like "Login Successful," "Invalid Credentials," or "Session Expired." These are typically managed with packages like `connect-flash`.

13. **Error Handling**: Create middleware to handle HTTP errors such as 404 (Page Not Found), 500 (Internal Server Error), and other client/server errors, ensuring the application gracefully handles unexpected conditions.

14. **Extras**: Additional features could include implementing password reset functionality, account locking after multiple failed login attempts, and a dashboard for users to manage their profiles.

