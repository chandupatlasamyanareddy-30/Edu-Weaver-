# Edu-Weaver-

**Turn boring topics into epic stories.**

Edu-Weaver is an AI-powered educational tool that transforms dry, complex subjects into engaging narratives. By combining storytelling with active recall (quizzes), it helps students learn faster and retain information longer.

## 🚀 Features

-   **AI Story Generation**: Instantly creates short, educational stories based on any user-provided topic.
-   **Genre Selection**: Customize the learning experience with genres like *Sci-Fi, Fantasy, Mystery,* and *Comedy*.
-   **Interactive Quizzes**: Automatically generates a 3-question multiple-choice quiz based on the story to test comprehension.
-   **Instant Feedback**: Powered by the Groq Llama-3-70b model for lightning-fast responses.
-   **Responsive Design**: Built with Tailwind CSS for a beautiful experience on mobile and desktop.

## 🛠️ Tech Stack

-   **Frontend**: [Next.js 14](https://nextjs.org/) (React framework)
-   **Styling**: [Tailwind CSS](https://tailwindcss.com/)
-   **Language**: TypeScript
-   **AI Model**: [Groq](https://groq.com/) (Llama-3-70b-versatile)
-   **Deployment**: Vercel

## 📂 Project Structure

The project uses the Next.js App Router. The backend logic is separated into distinct API routes to handle story and quiz generation independently.

text
src/app
├── page.tsx               # Frontend UI (Inputs, Story Display, Quiz Button)
└── api
    ├── chat               # Story Generation Endpoint
    │   └── route.ts       # POST: Accepts { topic, genre } -> Returns { story }
    └── quiz               # Quiz Generation Endpoint

    ⚡ Getting Started
Follow these steps to run the project locally.

1. Prerequisites
Node.js (v18 or higher) installed.

A free API Key from Groq Console.

2. Clone the Repository
Bash
git clone [https://github.com/your-username/edu-weaver.git]
cd edu-weaver


4. Install Dependencies
Bash
npm install
yarn install
4. Set up Environment Variables
Create a .env.local file in the root directory and add your Groq API key:
GROQ_API_KEY=gsk_your_actual_api_key_here


5. Run the Development Server
Bash
npm run dev
vercel dev
Open http://localhost:3000 with your browser to see the result.

How to Use
Enter a Topic: Type in any subject you want to learn about (e.g., "Photosynthesis", "Black Holes", "The French Revolution").

Pick a Genre: Select a style for your story (Sci-Fi, Fantasy, Mystery, etc.).

Generate: Click "Generate Story" and read the AI-crafted narrative.

Test Yourself: Scroll down and click "Test My Knowledge" to take a pop quiz generated from the story content.

🔮 Future Roadmap
 Voice Narration: Text-to-speech integration to listen to stories.

AI Illustrations: Generate images for each story chapter.

User Accounts: Save favorite stories and track quiz scores.

📄 License
This project is open-source and available under the MIT License.
