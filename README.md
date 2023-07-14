Project Documentation
This documentation provides instructions on how to clone and set up the AI Chatbot project locally, as well as an overview of its functionality and the project files.

Cloning the Project
To clone the project repository locally, follow these steps:

Open your terminal or command prompt.
Navigate to the directory where you want to clone the project.
Run the following command:
git clone <repository-url>
Replace <repository-url> with the URL of your project repository on GitHub.
Project Setup
Before running the project, make sure you have the following prerequisites installed:

Node.js (LTS version)
npm (Node Package Manager)
To set up the project, follow these steps:

Open your terminal or command prompt.
Navigate to the project's root directory.
Run the following command to install the project dependencies:
npm install
Create a .env.local file in the project's root directory.
Add the following environment variables to the .env.local file:
PINECONE_API_KEY="..."
PINECONE_INDEX_NAME="..."
OPENAI_API_KEY="..."
Replace the ... with the corresponding API keys and index names obtained from Pinecone and OpenAI.
Running the Project
To run the project locally, follow these steps:

Make sure you are in the project's root directory in your terminal or command prompt.
Run the following command:
npm run dev
This command starts the Next.js development server and makes the project accessible at http://localhost:3000.
Project Files
Here's a brief overview of the main files and directories in the project:

pages/index.tsx: The homepage of the application. It contains the main UI components, including the PDF dropzone and chat interface.
api/addData/route.ts: Defines the /api/addData route, which handles the uploading and processing of PDF files to train the chatbot.
api/chat/route.ts: Defines the /api/chat route, which handles user prompts and generates chatbot responses using the trained model.
src/app/globals.css: The global CSS file for styling the application.
src/app/layout.tsx: Defines the layout component for the application, including the metadata.
src/app/api/: Directory containing the API route files.
src/app/components/: Directory containing reusable UI components used throughout the application.
src/app/utils/: Directory containing utility functions and helper files.
Please refer to the source code and inline comments for more detailed explanations of each file's functionality.