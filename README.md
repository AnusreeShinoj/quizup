QuizUp – Interactive Quiz Web Application

QuizUp is a full-stack web application that makes learning and self-assessment engaging through interactive quizzes. Users can create, publish, discover, share, and attempt quizzes while tracking their performance, identifying weak topics, and improving their knowledge.

✨ Features

- User Authentication – Register and log in securely.
- Create Quizzes – Create quizzes with multiple-choice questions, options, correct answers, explanations, topics, and marks.
- Quiz Management – Edit, publish, unpublish, and delete quizzes.
- Discover Quizzes – Explore public quizzes by subject, topic, difficulty, and exam category.
- Share Quizzes – Share quizzes using links or unique codes.
- Interactive Quiz Attempts – Answer questions, navigate between them, and submit responses.
- Automatic Evaluation – Calculate scores and percentages automatically.
- Performance Analysis – View topic-wise accuracy and identify strengths and weaknesses.
- Quiz History – Review previous attempts and results.
- Smart Recommendations – Receive rule-based quiz recommendations based on performance and topics with less than 50% accuracy.

🛠️ Technology Stack

Component| Technology
Frontend| React, HTML, CSS, JavaScript
Backend| Node.js, Express.js
Database| MongoDB
Database Integration| Mongoose
Authentication| Secure password hashing and server-side authentication

📂 Project Structure

QuizUp/
├── client/
│   ├── public/
│   └── src/
│       ├── components/
│       ├── pages/
│       ├── services/
│       └── styles/
├── server/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   └── server.js
├── .gitignore
└── README.md

The directory structure may vary depending on the implementation.

⚙️ Getting Started

Prerequisites

- "Node.js" (https://nodejs.org/)
- "MongoDB Atlas" (https://www.mongodb.com/cloud/atlas) account
- "Git" (https://git-scm.com/)
- "Visual Studio Code" (https://code.visualstudio.com/) or another code editor

Installation

1. Clone the repository

git clone YOUR_REPOSITORY_URL
cd QuizUp

Replace "YOUR_REPOSITORY_URL" with your GitHub repository URL.

2. Install backend dependencies

cd server
npm install

3. Configure environment variables

Create a ".env" file in the backend directory:

PORT=5000
MONGODB_URI=your_mongodb_atlas_connection_string
JWT_SECRET=your_long_random_secret
CLIENT_URL=http://localhost:5173

Replace the placeholder values with your actual configuration. Never commit your ".env" file or expose database credentials and secrets.

4. Start the backend

npm run dev

5. Install and start the frontend

Open a separate terminal:

cd client
npm install
npm run dev

Use the commands and folder paths specified in the actual project if they differ from these examples.

🗄️ Database

QuizUp uses MongoDB to store application data, including:

- User accounts
- Quiz details and questions
- Quiz attempts and submitted answers
- Scores and topic-wise performance results

The backend uses Mongoose to manage database models and interactions.

🧠 Recommendation System

QuizUp uses a rule-based recommendation system implemented in JavaScript. It analyses quiz performance, identifies topics where accuracy is below 50%, and recommends relevant published quizzes when available.

The recommendation system does not require AI or machine-learning models.

🔐 Security

- Store passwords as secure hashes.
- Keep database credentials and secrets on the server.
- Allow quiz creators to manage only their own quizzes.
- Restrict access to private quizzes.
- Do not expose correct answers before submission.
- Calculate and validate scores on the server.

🎯 Objectives

- Make quiz creation and participation simple and engaging.
- Automate evaluation and result generation.
- Help users understand their topic-wise performance.
- Maintain quiz history for progress tracking.
- Recommend quizzes based on individual learning needs.

🚀 Future Enhancements

- Leaderboards and competitive quiz modes
- Additional question types
- Enhanced analytics and progress visualizations
- Quiz export and reporting
- Improved accessibility and user experience# quizup
a full stack quiz platform for creating ,sharing,and attempting quizzes,with automatic scoring,topic wise performance  analysis ,quix history and rule based recommendations
