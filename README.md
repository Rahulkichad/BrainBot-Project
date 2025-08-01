# Board Game Project

This project appears to be a full-stack application, primarily built with Next.js for the frontend and likely integrating backend functionalities within the Next.js framework itself, given the presence of backend-related dependencies in the frontend's `package.json`.

## Project Overview

This application seems to involve a board game, possibly with features like user authentication, real-time interactions (indicated by `socket.io-client`), and AI integration (indicated by `@google/generative-ai` and `openai`). The use of `chessboardjs` and `chess.js` suggests a chess-related game.

## Features (Inferred)

*   **User Authentication:** Secure user login and registration.
*   **Board Game Interface:** Interactive chessboard display and game logic.
*   **AI Integration:** Possible AI opponent or game analysis using Gemini and OpenAI APIs.
*   **Real-time Communication:** Live updates and interactions between players.
*   **Database Integration:** Data storage and retrieval using MongoDB (via Mongoose).
*   **Email Notifications:** Sending emails, possibly for account verification or game updates.
*   **IP Geolocation:** Potentially for regional content or analytics.

## Technologies Used

### Frontend (Next.js)

*   **Framework:** Next.js
*   **UI Components:** Radix UI, Tailwind CSS, `class-variance-authority`, `clsx`, `tailwind-merge`, `tailwindcss-animate`
*   **Chess Libraries:** `@chrisoakman/chessboardjs`, `chess.js`, `chessboardjs`, `chessboardjsx`, `react-chessboard`
*   **AI/Generative Models:** `@google/generative-ai`, `openai`
*   **State Management/Utilities:** `axios`, `react-hot-toast`, `react-icons`, `framer-motion`
*   **Authentication:** `bcryptjs`, `jsonwebtoken`, `cookies`
*   **Other:** `jquery`, `react-compound-timer`, `react-contenteditable`, `@uiw/react-textarea-code-editor`

### Backend (Integrated within Next.js)

*   **Server Framework:** Express.js
*   **Database:** MongoDB (via Mongoose)
*   **Authentication:** `bcryptjs`, `jsonwebtoken`
*   **Email Service:** Nodemailer
*   **Utilities:** `body-parser`, `dotenv`, `geoip-lite`, `request-ip`, `socket.io-client`

### Development Tools

*   TypeScript
*   ESLint
*   Autoprefixer
*   PostCSS

## Setup and Installation

To set up the project locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Rahulkichad/BrainBot-Project
    cd boradgame
    ```

2.  **Navigate to the frontend directory:**
    ```bash
    cd frontend
    ```

3.  **Install dependencies:**
    ```bash
    npm install
    # or
    yarn install
    ```

4.  **Configure Environment Variables:**
    Create a `.env` file in the `frontend/` directory and another in the `backend/` directory (if separate backend logic exists outside Next.js API routes) with necessary environment variables. Based on the provided context, you have a `GEMINI_API_KEY` in `frontend/.env`.

    Example `frontend/.env`:
    ```
    GEMINI_API_KEY=YOUR_GEMINI_API_KEY
    # Add other necessary environment variables here (e.g., MongoDB URI, JWT Secret, etc.)
    ```

    Example `backend/.env` (if applicable):
    ```
    # Add backend specific environment variables here
    ```

## Running the Project

1.  **Start the development server:**
    ```bash
    cd frontend
    npm run dev
    # or
    yarn dev
    ```

    The application should now be running at `http://localhost:3000` (or another port if configured).

## Project Structure
