# VibeCheck API + Button Smash UI

This project contains a small Express-based backend and a simple browser frontend that interact through JSON API calls.

---

## Included Components

### Backend
- Node.js + Express server  
- CORS enabled  
- Routes that return text responses, vibe messages, and a smash counter  
- A secret endpoint that requires a code  

### Frontend
- HTML page with interactive buttons  
- JavaScript file that sends `fetch()` requests to the backend  
- Output area that displays API responses  
- Button that increments the smash counter  

---

## Repository Structure
```
backend/
frontend/
```

---

## API Endpoints

- `GET /api/fortune` → Returns a random fortune  
- `GET /api/joke` → Returns a random joke  
- `GET /api/vibe?mood=happy|tired|stressed` → Returns a vibe message and emoji  
- `POST /api/smash` → Increments the smash counter  
- `GET /api/smashes` → Returns the current smash count  
- `GET /api/secret?code=411L` → Returns a hidden message if the code is correct  

---

## How to Execute

### 1. Setup Backend
```
cd backend
npm install
node index.js
```

Server runs on:  
`http://localhost:3000`

### 2. Run Frontend
- Open `frontend/index.html` in your browser  
- Click any button to send requests to the backend  
- The JSON response will appear on the page  
