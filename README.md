![Design & development](https://github.com/yassine-ahmed/eLearning-Platform/blob/main/Frontend/public/thumbnail.png)

# eLearning platform (YACOD) with Clerk

This project is an enterprise-level full-stack online learning platform built with modern web technologies. It leverages [Clerk](https://clerk.com) for authentication and user management, providing a seamless and secure experience for users.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Architecture](#architecture)
- [Installation](#installation)
- [Usage](#usage)

## Features

- **User Authentication and Management**: Implemented using Clerk for secure and efficient user handling.
- **Course Management**: Create, update, and delete courses with rich content.
- **Video Playback**: Integrate video content seamlessly within courses.
- **File Uploads**: Support for uploading course materials and resources.
- **Payment Processing**: Handle course payments securely using Stripe.
- **Scalable Backend**: Built with AWS services for scalability and reliability.

## Technologies Used

### Frontend

- **React**: JavaScript library for building user interfaces.
- **Shadcn**: UI components and design system.
- **React Hook Form**: Form management.
- **Zod**: Schema validation.
- **Redux Toolkit**: State management.
- **React FilePond**: File upload component.
- **React Player**: Media player component.
- **Stripe**: Payment processing.

### Backend

- **AWS DynamoDB**: NoSQL database service.
- **Dynamoose**: Modeling tool for DynamoDB.
- **AWS S3**: Object storage service.
- **AWS CloudFront**: Content delivery network.
- **AWS ECR**: Container registry.
- **Docker**: Containerization platform.

## Architecture

The system architecture is designed for scalability and performance. It includes a React frontend interfacing with a backend powered by AWS services. User authentication is managed by Clerk, while course data is stored in DynamoDB. Media content is served through S3 and CloudFront, ensuring efficient delivery.

For a visual representation of the architecture and workflows, refer to the [Project Diagrams](https://miro.com/app/board/uXjVLB-4pok=/).

## Installation

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/yassine-ahmed/eLearning-Platform.git

2. **Navigate to the Project Directory**:

   ```bash
   cd eLearning-Platform

3. **Install Dependencies**:

   ```bash
   npm install

3. **Set Up Environment Variables**:
Create a .env file in the root directory and add the necessary environment variables as per the .env.example file.

3. **Start the Development Server**:

   ```bash
   npm run dev

### Usage

- **Access the Application**: Navigate to http://localhost:3000 in your browser.
- **User Registration and Login**: Use Clerk's authentication system to register and log in.
- **Course Management**: Create and manage courses through the dashboard.
- **Content Upload**: Upload course materials and videos.
- **Payment Processing**: Test payment functionalities using Stripe's test environment.
