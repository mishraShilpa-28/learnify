# Learning Management System (LMS) with MERN Stack

This is a full-stack Learning Management System (LMS) application built using the MERN stack (MongoDB, Express.js, React.js, Node.js). The project is based on a YouTube tutorial by Surendrakumar Patel and provides a platform where users can register, log in, browse and enroll in courses, and track their learning progress. Instructors can create and manage courses, add lessons, and monitor performance through an admin dashboard.

## Project Description

The LMS is designed to facilitate online education with distinct roles for students and instructors. Students can explore courses, enroll in them, and track their progress, while instructors can create, edit, and manage courses. The application features a responsive UI with light and dark mode support, secure payment integration via Stripe, and protected routes to ensure proper access control.

## Features

- **User Authentication**:
  - Register and log in with email and password.
  - Edit profile details (e.g., name, profile picture).
  - Logout functionality.
- **Course Management**:
  - Instructors can create, edit, publish, and unpublish courses.
  - Course details include title, subtitle, description, price, category, level (beginner, intermediate, advanced), and thumbnail.
- **Lesson Management**:
  - Instructors can add video lessons to courses.
  - Lessons can be marked as free (e.g., introductory) or private (locked for non-enrolled users).
- **Enrollment and Progress Tracking**:
  - Students can enroll in courses via Stripe payment.
  - View course content and mark lessons as completed or incomplete.
  - "My Learning" section to track enrolled courses and progress.
- **Search and Filtering**:
  - Search courses by keyword (e.g., "Docker", "MongoDB").
  - Filter courses by category (e.g., Frontend Development, Data Science).
  - Sort courses by price (low to high or high to low).
- **Payment Integration**:
  - Secure course purchases using Stripe payment gateway.
  - Test payments supported with dummy card details (e.g., 4242 4242 4242 4242).
- **Admin Dashboard**:
  - Instructors can view total revenue (e.g., ₹1237 as shown in demo) and course enrollments.
  - Manage all published and draft courses.
  - Graphical representation of course sales (to be implemented fully in code).
- **UI Features**:
  - Responsive design for mobile and desktop.
  - Light and dark mode toggle.
  - Skeleton loading screens for better UX during data fetching.
- **Security**:
  - Protected routes: Only logged-in users can access course details, progress pages, and search functionality.
  - Admin routes restricted to instructors only.
  - Double security on progress pages to ensure only enrolled users can access content.

## Technologies Used

- **MongoDB**: Database for storing user data, courses, and lessons.
- **Express.js**: Backend API framework.
- **React.js**: Frontend user interface.
- **Node.js**: Server-side runtime environment.
- **Stripe**: Payment processing.
- **Tailwind CSS**: Styling (assumed based on modern UI practices in demo).

## Installation Instructions

1. **Clone the Repository**:

    ```bash
    git clone https://github.com/mishraShilpa-28/learnify.git
    ```

2. **Navigate to the Project Directory**:

    ```bash
    cd learnify
    ```

3. **Install Backend Dependencies**:

    ```bash
    cd server && npm install && cd ../
    ```

4. **Install Frontend Dependencies**:

    ```bash
   cd client && npm install && cd ../
   ```

5. **Set Up Environment Variables**:
   - Create a `.env` file in the `server` directory.
   - Add variables such as:

    ```bash
    PORT=8080

    # mongodb setup
    MONGO_URI=
    SECRET_KEY=

    # cloudinary setup
    API_KEY=
    API_SECRET=
    CLOUD_NAME=

    # stripe setup
    STRIPE_SECRET_KEY=
    STRIPE_PUBLISHABLE_KEY=
    ```

6. **Run the Backend Server**:
    - Open a new terminal for server

   ```bash
   npm run dev
   ```

7. **Run the Frontend Server**:
    - Open a new terminal for client

   ```bash
   npm run dev
   ```

## Live Demo

[Link to Live Demo](#) *(Note: Replace with actual link when available)*

## Additional Notes

- The project includes a mobile-responsive navigation bar with options like Dashboard, My Learning, and Profile.
- Courses are displayed with details such as enrollment count, creation date, and instructor name.
- The demo showcases real-time updates (e.g., profile changes, lesson completion) with loading animations for a smooth user experience.
- Minor bugs (e.g., light/dark mode inconsistencies) are noted and fixed in the tutorial, ensuring a polished final product.
