
# Resume Builder App

## Overview

The Resume Builder App is a full-stack web application designed to help users create professional resumes quickly and easily. This application allows users to input their details, choose from various templates, and download their resumes in a formatted PDF.

## Features

- **User Registration & Authentication:** Secure login and registration system.
- **Resume Templates:** A variety of customizable resume templates.
- **Real-time Preview:** Users can see a live preview of their resume as they input data.
- **PDF Export:** Allows users to download their resume as a PDF.
- **Responsive Design:** Mobile-first design ensures usability on all device sizes.

## Tech Stack

- **Frontend:**
  - React.js
  - Redux
  - Bootstrap
  - Axios

- **Backend:**
  - Node.js
  - Express.js
  - MongoDB (for storing user data)

- **Other Dependencies:**
  - JWT for authentication
  - Mongoose for MongoDB object modeling
  - Multer for file uploads (if applicable)

## Getting Started

### Prerequisites

- Node.js (v14.x or later)
- npm (v6.x or later)
- MongoDB (local or cloud instance)

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/resume-builder-app.git
   cd resume-builder-app
   ```

2. **Install dependencies:**

   ```bash
   # Install backend dependencies
   npm install

   # Install frontend dependencies
   cd client
   npm install
   ```

3. **Set up environment variables:**

   Create a `.env` file in the root of the project and add the following variables:

   ```env
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret_key
   ```

4. **Run the application:**

   ```bash
   # Run the backend server
   npm run server

   # Run the frontend development server
   cd client
   npm start
   ```

   The app should now be running at `http://localhost:3000`.

### Usage

1. Register or log in to your account.
2. Fill in your personal details, education, work experience, and skills.
3. Choose a resume template from the available options.
4. Preview your resume in real-time.
5. Download your resume as a PDF.

### Testing

To run the tests, use the following command:

```bash
npm run test
```

### Project Structure

```bash
resume-builder-app/
│
├── client/                 # Frontend (React)
│   ├── public/             # Public files
│   ├── src/                # Source files
│   │   ├── components/     # React components
│   │   ├── redux/          # Redux store and actions
│   │   ├── styles/         # CSS styles
│   │   ├── utils/          # Utility functions
│   │   └── App.js          # Main React component
│   └── package.json        # Frontend dependencies
│
├── config/                 # Configuration files
├── controllers/            # Express.js controllers
├── models/                 # Mongoose models
├── routes/                 # Express.js routes
├── middleware/             # Custom middleware
├── server.js               # Main server file
├── package.json            # Backend dependencies
└── .env                    # Environment variables
```

