# Ganitsaar online classes

Google sign-in. Only 1molharne@gmail.com can create or delete classes. Everyone can view and join.

## Add to your Replit project
1. Copy `server.js` and the whole `public/` folder (or just `classes.html` and `room.html` into your existing public folder).
   If your site already has its own server, keep it and copy the routes from `server.js` instead.
2. Replit -> Secrets -> add `GOOGLE_CLIENT_ID` (see below).
3. Run command: `node server.js`  (no npm install needed).
4. Link to `/classes.html` from your menu.

## Google client ID
Google Cloud Console -> APIs & Services -> OAuth consent screen (External) -> Credentials ->
Create OAuth client ID -> Web application -> Authorized JavaScript origins:
`https://maharashtra-board-math-learning-website--1molharne.replit.app`

## Notes
- Classes are saved in `classes.json`. Set `DATA_DIR` to a persistent folder if your deployment resets files.
- The teacher check runs on the server for every create and delete request.
