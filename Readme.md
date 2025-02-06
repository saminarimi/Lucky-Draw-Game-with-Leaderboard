1️⃣ Basic Flow of the Game
User Registration: Users enter their name in a form and click "Join the Draw".
Lucky Draw Mechanism: After a set interval (or on button click), the system picks a random winner.
Winner Announcement: The winner's name appears on the screen with animations and sound effects.
Leaderboard Update: The leaderboard stores and displays the winners.
Repeat the Draw: The process can be repeated to pick more winners.
2️⃣ Frontend (HTML, CSS, JavaScript)
👨‍💻 User Interface Components
✔ Form to Enter Name – Users type their name and submit.
✔ "Pick a Winner" Button – Manually triggers the draw.
✔ Spinning Wheel Animation (Optional) – Visually selects a winner.
✔ Winner Announcement Section – Displays the selected winner with effects.
✔ Leaderboard Table – Shows past winners ranked by number of wins.

🔁 Frontend JavaScript Functionality
Store participants in an array of objects { name: "Alice", wins: 2 }
Use array loops to check if a user is already in the game.
Use Math.random() to pick a random winner.
Use if-else conditions to prevent duplicate winners in a single round.
Dynamically update the leaderboard after each draw.
3️⃣ Backend (Node.js, Express, JSON/MongoDB)
🗄 Backend API Endpoints
Method Endpoint Functionality
POST /join Add user to the lucky draw list
GET /draw Pick a random winner from the list
GET /leaderboard Retrieve top winners
DELETE /reset Clear all participants and reset the game
🛠 Backend Logic
When a user joins the draw, their name is stored in a database (MongoDB/JSON file).
The draw logic fetches all participants and selects a winner using a random function.
Winners are stored in the leaderboard, and their win count increases if they win multiple times.
The system prevents duplicate names and ensures fairness using if-else conditions.
4️⃣ Bonus Features (Make it More Fun!)
✅ 🎵 Sound Effects – Play an exciting sound when a winner is chosen.
✅ 🎨 Animations – Use CSS/JS to make a spinning wheel effect.
✅ 🕒 Auto Draw Timer – Automatically picks a winner every 30 seconds.
✅ 💎 Extra Entries – Let users earn bonus entries by clicking a "Try Again" button.
✅ 🌍 Multiplayer Mode – Allow multiple users to join via WebSockets (real-time updates).
