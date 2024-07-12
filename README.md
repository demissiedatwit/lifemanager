# AI Native Student Copilot Platform

## Overview
The AI Native Student Copilot Platform is an innovative tool designed to assist Wentworth Institute of Technology students by integrating data from LeopardWeb and Brightspace. It provides personalized academic support through an AI-powered chat interface.

## Features
- Secure sign-in for Wentworth students (@wit.edu emails only)
- Data integration with LeopardWeb and Brightspace
- AI-powered chat interface for academic assistance
- File upload and management system
- Personalized content generation
- Intelligent tutoring and Q&A
- Automated feedback and grading
- Interactive visual learning aids
- Adaptive learning paths

## Tech Stack
- Frontend: React.js with Tailwind CSS
- Backend: Firebase Cloud Functions (Node.js)
- Database: Firebase Firestore
- Authentication: Firebase Authentication
- File Storage: Firebase Storage
- Web Scraping: Puppeteer
- Deployment: Google Cloud Platform

## Setup
1. Clone the repository
2. Install dependencies:
   ```
   npm install
   cd functions
   npm install
   ```
3. Set up Firebase:
   - Create a Firebase project
   - Enable Firestore, Storage, and Authentication
   - Add your Firebase config to `src/firebaseConfig.js`
4. Deploy Firebase functions:
   ```
   firebase deploy --only functions
   ```
5. Run the app locally:
   ```
   npm start
   ```

## Testing
- Use Firebase emulators for local testing:
  ```
  firebase emulators:start
  ```
- Test Cloud Functions:
  ```
  firebase functions:shell
  ```

## Deployment
- Deploy to Firebase Hosting:
  ```
  npm run build
  firebase deploy --only hosting
  ```

## Security Considerations
- Ensure proper Firebase security rules are in place
- Handle sensitive data (like passwords) securely
- Implement rate limiting on Cloud Functions
- Regularly update dependencies

## Future Enhancements
- Implement machine learning models for better personalization
- Expand to support other educational institutions
- Develop mobile applications for iOS and Android

## Contributors
- Daniel Demissie Tadesse

## License
MIT

## Disclaimer
This project is for educational purposes only. Ensure you have permission to access and use data from LeopardWeb and Brightspace before deploying to production.
