# RPM.AI - Research & Practice Med.AI

RPM.AI is an intelligent platform designed specifically for medical students and researchers to get complex medical topics explained through text and speech-to-text functionality, with a secure authentication system for privacy protection.

[[Video Title][https:/gitMedStudentAssistant.webm]](https://github.com/sakshamagarwalm2/RPM.AI/blob/main/Public/MedStudentAssistant.webm)

## Table of Contents
- [Project Description](#project-description)
- [Features](#features)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Technologies Used](#technologies-used)
- [Future Enhancements](#future-enhancements)
- [Credits](#credits)
- [License](#license)

## Project Description

RPM.AI (Research & Practice Med.AI) aims to bridge the gap between complex medical knowledge and students/researchers by providing an intuitive AI-powered platform. Medical topics often involve intricate concepts that can be challenging to grasp. This application leverages advanced natural language processing to break down complex topics into understandable explanations.

The platform provides both text-based and speech-to-text interfaces, allowing users to interact in their preferred way. A robust authentication system ensures that user data and queries remain private and secure, which is particularly important in the medical field.

## Features

- **AI-Powered Explanations**: Get detailed explanations for complex medical topics using Llama 3.3-70b via Groq API
- **Dual Input Methods**: Text and speech-to-text functionality for flexible interaction
- **Secure Authentication**: Clerk API for user authentication and security
- **Responsive Design**: Works seamlessly across devices of various screen sizes
- **Protected Routes**: Ensures secure access to user-specific content

## Project Structure

```
src/
├── components/
│   ├── ui/
│   │   ├── Header.tsx
│   │   └── ProtectedRoute.tsx
│   └── pages/
│       ├── ChatPage.tsx
│       ├── HomePage.tsx
│       └── SignIn.tsx
├── App.tsx
├── groqService.ts
├── index.css
├── main.tsx
├── vite-env.d.ts
├── .env.example
├── .gitignore
├── eslint.config.js
└── index.html
```

## Installation

Follow these steps to set up the project locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/rpm-ai.git
   cd project
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create your environment file:
   ```bash
   cp .env.example .env
   ```

4. Add your API credentials to the `.env` file:
   ```
   VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key_here
   VITE_GROQ_API_KEY=your_groq_api_key_here
   ```

5. Start the development server:
   ```bash
   npm run dev
   ```

## Usage

1. **Sign In**: Create an account or sign in using the Clerk authentication system
2. **Home Page**: Navigate through the available options on the home page
3. **Chat Interface**: Use the chat interface to:
   - Type your medical questions directly
   - Click the microphone icon to use speech-to-text functionality
   - Review AI-generated explanations from Llama 3.3-70b served through Groq API
   - Save important explanations for future reference

Example prompts:
- "Explain the pathophysiology of diabetic ketoacidosis"
- "What are the mechanisms of action for beta-blockers?"
- "Describe the neurological pathways involved in Parkinson's disease"

## Technologies Used

- **Frontend**: React with TypeScript using Vite as build tool
- **UI Components**: Custom UI components with responsive design
- **Authentication**: Clerk API for secure user management and authentication
- **AI Infrastructure**: Groq API for accessing the Llama 3.3-70b model with low-latency responses
- **AI Model**: Llama 3.3-70b for high-quality medical information processing
- **Speech Recognition**: Web Speech API for speech-to-text functionality
- **Styling**: CSS with modern styling approaches
- **No Database**: The application operates without a database, focusing on real-time AI interactions

## Future Enhancements

- Medical literature citation for explanations
- User history tracking for reviewing past queries
- Specialized modes for different medical specialties
- Export functionality for saving explanations as PDF
- Collaborative features for study groups
- Offline mode for access without internet connection

## License

This project is licensed under the terms of the [Llama License](https://github.com/meta-llama/llama/blob/main/LICENSE).
