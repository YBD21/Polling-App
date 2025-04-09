# Voting App 🗳️

A real-time collaborative voting application that allows users to create polls, nominate options, and vote on them. ✨

## Features 🌟

- **Poll Creation** 📝: Create a new poll with a specific topic
- **Waiting Room** 🚪: Participants can join a poll using a unique poll ID
- **Nominations** ✋: Participants can suggest options for voting
- **Real-time Updates** ⚡: All changes are synchronized in real-time using Socket.IO
- **Voting System** 📊: Participants can rank their preferences
- **Results Visualization** 📈: View voting results after completion
- **Admin Controls** 👑: Poll creators have special permissions:
  - Remove participants
  - Remove nominations
  - Start/close polls
  - Cancel polls

## Tech Stack 🛠️

- **Frontend** 💻: React with Valtio for state management
- **Backend** 🔧: Node.js with Socket.IO for real-time communication
- **UI Components** 🎨: Custom components with Storybook for development
- **Styling** 🎭: Tailwind CSS

## Installation 📥

1. Clone the repository
2. Install dependencies:

```bash
# Install server dependencies
cd server
npm install

# Install client dependencies
cd ../client
npm install
```

## Running the Application 🚀

### Development Mode 🔧

```bash
# Start the server
cd server
npm run dev

# Start the client in another terminal
cd client
npm start
```

### Production Mode 🏭

```bash
# Build the client
cd client
npm run build

# Start the server
cd ../server
npm start
```

## Usage 📱

1. **Create a Poll** 🆕:

   - Enter your name and a poll topic
   - Share the generated Poll ID with participants

2. **Join a Poll** 🔗:

   - Enter your name and the Poll ID to join
   - Wait for the admin to start the voting

3. **Nomination Phase** 🙋:

   - Add nominations for voting options
   - Admin can remove inappropriate nominations

4. **Voting Phase** ✅:

   - Rank your preferences
   - Submit your vote

5. **Results** 📊:
   - View the final results after everyone has voted

## Project Structure 📁

- `client/`: Frontend React application 🖥️

  - `components/`: Reusable UI components
  - `pages/`: Main page components
  - `stories/`: Storybook component stories
  - `state.ts`: Global state management
  - `socket-io.ts`: Socket connection handling

- `server/`: Backend server (Node.js) 🔌

  - API routes and Socket.IO handlers

- `shared/`: Shared types and utilities 🔄
