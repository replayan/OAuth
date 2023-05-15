# OAuth Project using Node.js, EJS, and Google OAuth v2

This project allows users to securely and easily log in to your website or application using their Google credentials. With the power of OAuth, users can grant access to their Google account without having to share their password with your application.

## Getting Started

To get started, clone this repository to your local machine. Make sure you have Node.js installed and run the following command to install the required dependencies:

```bash
npm install
```

Next, create a new Google Cloud Platform project and enable the Google OAuth API. Then, create a new OAuth 2.0 client ID and configure it to use `http://localhost:3000/auth/google/callback` as an authorized redirect URI.

Once you have your OAuth credentials, create a `.env` file in the root directory of the project and add the following variables:

```bash
GOOGLE_CLIENT_ID=<your_client_id>
GOOGLE_CLIENT_SECRET=<your_client_secret>
```

## Running the Project

To start the server, run the following command:

```bash
npm start
```

This will start the server on `http://localhost:3000`.

Visit `http://localhost:3000/login` to see the Google OAuth login button in action. After logging in with your Google credentials, you will be redirected to the home page.

## Customizing the Project

The project is built using Node.js and EJS, so you can easily customize it to fit your needs. The views are located in the `views` directory and the server code is located in the `app.js` file.

If you want to add additional OAuth providers, simply add the appropriate configuration to `passport.js` and update the login view to include the new provider button.

## Contributing

Contributions are welcome! If you find a bug or want to add a new feature, please open an issue or submit a pull request.
