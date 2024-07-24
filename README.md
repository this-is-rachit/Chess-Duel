# Chess-Duel

Chess-Duel is a real-time chess game implemented using Node.js, Express, and Socket.io, with a front-end built in plain JavaScript. Players can engage in a duel by connecting to the server and making moves, while spectators can watch the game in progress.

## Features

- **Real-time gameplay**: Moves are synchronized across all clients in real-time using Socket.io.
- **Drag-and-drop interface**: Players can drag and drop pieces on the board to make moves.
- **Automatic updates**: The chessboard updates automatically after each move.
- **Player roles**: The game assigns roles to players (White or Black) and lets others join as spectators.

## Technologies Used

- **Server**: Node.js, Express, Socket.io
- **Client**: Vanilla JavaScript, HTML/CSS
- **Chess Logic**: `chess.js`

## Getting Started

### Prerequisites
Make sure you have [Node.js](https://nodejs.org/) installed.

### Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/this-is-rachit/Chess-Duel.git
    cd chess-duel
    ```

2. Install dependencies:
    ```bash
    npm install
    ```

### Running the Server
To start the server, run:
```bash
npm start
```
This will start the Express server on http://localhost:3000.

### Running the Client
The client-side code is served from the same server, so you just need to open http://localhost:3000 in your web browser to start playing.

## Code Overview

1. app.js: 
-Sets up an Express server and Socket.io.
-Manages player connections and game state.
-Handles move validation and broadcasts moves to clients.

2. public/script.js:
-Handles the rendering of the chessboard.
-Manages drag-and-drop functionality for moving pieces.
-Updates the chessboard and handles game state synchronization with the server.

3. public/styles.css
-Contains styling for the chessboard and pieces.

## How to Play

1. Open http://localhost:3000 in multiple tabs or different browsers.
2. The first player to connect will be assigned the White pieces, the second player will get the Black pieces, and others will join as spectators.
3. Drag and drop pieces to make your moves.
4. The game automatically updates the board and announces the winner if checkmate occurs.

## Learn More

To learn more about the technologies used, refer to the following resources:
1. Next.js Documentation - Learn about Next.js features and API.
2. Learn Next.js - An interactive Next.js tutorial.
3. Socket.io Documentation - Learn about Socket.io for real-time web applications.
4. Chess.js Documentation - Learn about the chess logic used in the game.

## Contributing

Feel free to fork the repository and submit pull requests. Contributions are welcome!

## Acknowledgements

-Thanks to the authors of chess.js for providing the chess logic.
-Thanks to Socket.io for enabling real-time communication.
