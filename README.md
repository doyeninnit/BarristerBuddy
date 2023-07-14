# Barrister Buddy Project Documentation

This documentation provides instructions on how to clone and set up the AI Chatbot project locally, as well as an overview of its functionality and the project files.

## Getting Started

### Prerequisites

1. Open your terminal or command prompt.
2. Navigate to the directory where you want to clone the project.
3. Run the following command:

git clone <repository-url>


## Project Setup

Before running the project, make sure you have the following prerequisites installed:

- Node.js (LTS version)
- npm (Node Package Manager)

### Cloning the Repository

Execute the following steps to clone the repository:

```shell
# Open terminal
# Navigate to the desired directory
git clone https://github.com/Nashons/BarristerBuddy.git
```

### Project Setup

The following steps will guide you through setting up the project:

```shell
# Open terminal
# Navigate to the project's root directory
npm install

# Create .env.local file in the project's root directory and setup environment variables
echo 'PINECONE_API_KEY="..."\nPINECONE_INDEX_NAME="..."\nOPENAI_API_KEY="..."' >> .env.local
```

## Running the Project

To run the project locally, follow these steps:

```shell
# Make sure you're in the project's root directory
npm run dev
```

This command starts the Next.js development server and the project can be accessed at `http://localhost:3000`.

## Project Structure

The project comprises the following main files and directories:

- `pages/index.tsx`: This is the application's homepage containing the main UI components like the PDF dropzone and chat interface.
- `api/addData/route.ts`: Defines the `/api/addData` route for uploading and processing of PDF files for training the chatbot.
- `api/chat/route.ts`: Defines the `/api/chat` route to handle user prompts and generate responses from the trained model.
- `src/app/globals.css`: The application's global CSS file for styling.
- `src/app/layout.tsx`: Defines the layout component of the application including the metadata.
- `src/app/api/`: This directory contains all the API route files.
- `src/app/components/`: This directory contains reusable UI components used in the application.
- `src/app/utils/`: This directory contains utility functions and helper files.

For more detailed explanations of each file's functionality, please refer to the source code and inline comments.