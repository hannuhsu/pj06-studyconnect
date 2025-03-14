# pj06-studyconnect

Project Description: A webapp that helps connect college students in the same classes together for studying.

Full Name: Github ID
----------------------
Zhenyu Yu: ZhenyuYu1  
Wesley Chiba: jeffsmithepic  
Maria Saucedo-Flores: Maria-Saucedo  
Shelly Zhu: zhushelly  
Allen Hu: AllenHsm  
Anthony Jin: jinanthony  
Hannah Su: hannuhsu

# Tech Stack

Main Framework: Next.js

Backend:
- Database: Firebase
- Authentication: Firebase / Google OAuth
- Fetching UCSB class info: UCSB API

Deployment: Vercel

# Idea

In the front page of the website, each user is prompted with a Firebase or Google OAuth login for authentication. If login is successful, the webapp will display a list of classes that each user can choose from. The user can filter for a specific class by name or major, and can join each class. Students that join a class can send discussion messages in a chat room where they can connect with other students and share study resources. We are planning to use Firebase for storing user data, Firebase / Google OAuth for authentication, and the UCSB API to fetch class info.

# Roles

- Student:
  - Goal: To connect with other students and help study for classes
  - Permissions: View & browse classes, post messages and discussions
- Instructor:
  - Goal: To facilitate discussion about classes and help students study
  - Permissions: Same as students
 - Administrator:
   - Goal: To ensure class chats are not being misused (remove spam bots, etc)
   - Permissions: Remove users from channel, remove irrelevant content
  
# Installation

### Prerequisites
- Git version 2.43 or above (check using git -v)  
- npm version 10.2 or above (check using npm -v)  

### Dependencies
Frontend: 
- React.js and Next.js
- Tailwind for styling

Backend:
- Database: Firebase
- Authentication: Firebase / Google OAuth

### Installation Steps
Clone the project: `git clone https://github.com/ucsb-cs148-w25/pj06-studyconnect.git`  
Install dependencies: `npm install`  
Run locally: `npm run dev`  
Create a .env.local file in the /study-connect folder with the following environmental variables:
- NEXT_PUBLIC_FIREBASE_API_KEY="<your_key>"
- NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN="<your_key>"
- NEXT_PUBLIC_FIREBASE_PROJECT_ID="<your_key>"
- NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET="<your_key>"
- NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID="<your_key>"
- NEXT_PUBLIC_FIREBASE_APP_ID="<your_key>"
- NEXT_PUBLIC_FIREBASE_MEASUREMENT_ID="<your_key>"
- UCSB_API_KEY="<your_key>"
- FIREBASE_CLIENT_EMAIL="<your_key>"
- FIREBASE_PRIVATE_KEY="<your_key>"
- CLOUDINARY_URL="<your_key>"

You can get the Firebase keys by making a Firebase account and creating a new project here: [Firebase](https://firebase.google.com/)  
You can get a UCSB API key by filling out a request form here: [UCSB API request form](https://developer.ucsb.edu/docs/applications/application-approval-request)  
You can get a cloudinary key by making a free Cloudinary account here [Cloudinary](https://cloudinary.com/) 

Visit site at [localhost:3000](http://localhost:3000/)

# Functionality
1. Login using your @ucsb.edu email and fill out your profile page. View and customize at any time. 
2. View courses in the courses page found on the right side of the header
3. Search courses by subject code or course name
4. Join a course and start chatting

# Known Problems
1. Profile picture clips
2. Posts cannot be deleted except by admins

# Contributing
1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

# License
MIT License

# Deployment
[Deployed on Vercel](https://studyconnect-deploy.vercel.app/)


