# ejs-crud
MVC with EJS standalone for prod

## Render + Google OAuth 2.0 Setup
- Have your Google OAuth2.0 API credentials ready.
- Deploy to Render
- Build Command:
```
npm install
```
- Start Command
```
node server.js
```
- Add `DATABASE_URL` environment variable with the connection from your Neon.
- Add a `clientID` environment variable with the client ID from Google.
- Add a `clientSecret` environment variable with the secret from Google.
- Deploy
- After the deploy is done, copy the URL to the app over to the Google Cloud Console.
- Add it as a JavaScript origin.
```
https://your-app.onrender.com
```
- Add a redirect (note its http not https!)
```
http://your-app.onrender.com/auth/google/callback
```
