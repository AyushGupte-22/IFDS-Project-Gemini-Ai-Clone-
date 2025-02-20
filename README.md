# AI Bot with Voice Assistance

## 📌 Project Overview
This project is an **AI-powered chatbot with a voice assistant** that listens to user queries and responds in a natural, conversational manner. It features a **Speech-to-Speech (S2S) system** and supports **multi-language recognition**, ensuring that the bot detects the language spoken by the user and responds in the same language. 

### 🔥 Unique Challenge
- The end-user can speak in any language (Hindi, Marathi, English, Telugu, etc.), and the bot should respond in the same language.
- The bot must have a **character and a backstory** and should only answer in ways that align with its persona. For example:
  - A **rude banker** who hesitates to answer customer queries.
  - A **soft and humble actor** who enjoys interacting with fans.
  
The bot will **strictly stick to its character** and **only respond to queries related to its backstory**.

---

## 🚀 Tech Stack
- **Frontend:** React.js (with Vite for fast development)
- **Backend:** Node.js / Express.js (optional for API handling)
- **AI Model:** Google Gemini AI (for text processing and response generation)
- **Speech Processing:** Web Speech API / Google Speech-to-Text
- **Database (if required):** Firebase / MongoDB
- **Authentication:** Firebase Auth (optional)

---

## 🛠️ Installation & Setup

### 1️⃣ Install Dependencies (Yarn)
First, ensure that **Yarn** is installed. If not, install it globally:
```sh
npm install --global yarn
```
Then, navigate to the project directory and install dependencies:
```sh
yarn install
```

### 2️⃣ Set Up API Keys
Create a `.env` file in the root directory and add your Google API key:
```ini
VITE_GEMINI_API_KEY=your_google_api_key_here
```
Make sure to replace `your_google_api_key_here` with a valid API key from Google.

### 3️⃣ Start the Development Server
Run the following command to start the project:
```sh
yarn dev
```
The project will be accessible at `http://localhost:5173` (default Vite port).

---

## 🔧 Features
✅ **Multi-language support** (Detects and responds in the user's language)
✅ **Speech-to-Speech (S2S) System** (Listens and responds with voice output)
✅ **Character-based responses** (The bot follows a unique persona and backstory)
✅ **Google Gemini AI Integration** (For generating intelligent responses)
✅ **Customizable chatbot behavior** (Modify the character's personality easily)

---

## 🔍 Folder Structure
```
📂 AI-Bot-Voice-Assistant
│── 📂 src
│   ├── 📂 components       # UI components
│   ├── 📂 config           # API configurations
│   ├── 📂 assets           # Static files
│   ├── 📂 utils            # Helper functions
│   ├── 📜 App.jsx          # Main application file
│   ├── 📜 VoiceAssistant.jsx # Handles speech input and output
│   ├── 📜 Context.jsx      # Context API for state management
│── 📜 .env                 # API keys and environment variables
│── 📜 README.md            # Documentation
│── 📜 package.json         # Project metadata and dependencies
```

---

## 🛠️ Troubleshooting
### 1️⃣ **Vite Import Errors**
If you get an error like:
```
Failed to resolve import "@/config/gemini.js"
```
Try changing the import path:
```js
import run from "../config/gemini.js"; // Use relative path
```

### 2️⃣ **Invalid API Key Error**
If you see:
```
API key not valid. Please pass a valid API key.
```
- Make sure you have added the correct **Google Gemini API Key** in the `.env` file.
- Restart the server after adding the key:
  ```sh
  yarn dev
  ```

### 3️⃣ **Yarn Command Not Found**
If `yarn` is not recognized, install it globally:
```sh
npm install --global yarn
```
Then retry:
```sh
yarn install
```

---

## 🤖 Future Enhancements
- 🎤 **Better Voice Processing** (Using TensorFlow or OpenAI Whisper for speech recognition)
- 🔥 **Personalized AI Models** (Train custom models for more realistic responses)
- 📲 **Mobile App Support** (React Native version for mobile users)
- 🌎 **More Language Support** (Expand beyond Hindi, Marathi, English, Telugu)

---

## 🤝 Contributing
Want to improve this project? Feel free to fork and submit a PR!
```sh
git clone https://github.com/your-username/AI-Bot-Voice-Assistant.git
cd AI-Bot-Voice-Assistant
yarn install
```

---

## 📜 License
This project is licensed under the **MIT License**.




# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh
