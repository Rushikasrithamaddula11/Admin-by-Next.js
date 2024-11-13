# Admin-by-Next.js
🌟 Welcome to the Admin Dashboard Assignment! This project is built with Next.js and API integration to provide an admin interface for a social media platform. It includes features for user management, content moderation, and analytics.

## Project Overview

In this project, you will find a responsive admin dashboard with the following core features:

- **User Management**: View, track, and manage users' activity, referrals, and their role.
- **Content Moderation**: Monitor daily views, shares, comments, and posts to ensure the content follows platform guidelines.
- **Analytics**: Visualize and analyze user activity and content engagement using charts and graphs.

## Features

### 1. User Management
- View and manage users, track their activities, and identify key metrics such as active users and creators.

### 2. Content Moderation
- Monitor posts in real-time with key metrics such as views, shares, comments, and post exits.

### 3. Analytics
- View interactive charts showing user engagement and platform activity over daily or monthly periods. Visualize likes, shares, comments, and private messages.

## Tech Stack

- **Frontend**: [Next.js](https://nextjs.org/)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/) for responsive and utility-first design.
- **Data Visualization**: [Chart.js](https://www.chartjs.org/) for analytics charts and graphs.
- **API Data Fetching**: [SWR](https://swr.vercel.app/) for fetching and caching API data.

## Getting Started

Follow the steps below to set up the project on your local machine and get the admin dashboard up and running.

### 1. Clone the Repository

To begin, clone the repository using the following command:

```bash
git clone https://github.com/YourGitHubUsername/Admindashboard.git
cd Admindashboard
```

### 2. Install Dependencies

After cloning the repository, you need to install the necessary dependencies for the project. Run the following command to install them:

```bash
npm install
```

This will install all required packages defined in `package.json`, including `Next.js`, `Tailwind CSS`, `Chart.js`, and `SWR`.

### 3. Set Up Environment Variables

Create an `.env.local` file at the root of the project to store sensitive or environment-specific information, such as API URLs or keys. Here's an example of what you might need to include in this file:

```bash
NEXT_PUBLIC_API_URL=https://api.socialverseapp.com/admin/dashboard
```

Make sure to replace the value of `NEXT_PUBLIC_API_URL` with the actual API URL you're using for your application. This allows the frontend to interact with the backend properly.

### 4. Run the Development Server

Once the dependencies are installed and environment variables are set, you can run the development server to preview your dashboard locally.

```bash
npm run dev
```

This will start a local server at `http://localhost:3000`. Open your browser and go to that address to view the admin dashboard in action.

### 5. Build and Deploy (Optional)

If you're ready to deploy your project to a production environment, use the following commands to build and deploy the application:

- **Build the application**: This prepares the app for production by optimizing performance and assets.

  ```bash
  npm run build
  ```

- **Start the production server**: Once the build is complete, start the production server to serve the optimized app.

  ```bash
  npm run start
  ```

You can deploy the built app on platforms like Vercel, Netlify, or any other provider that supports Next.js.

---

## Project Structure

The project is organized as follows:

```
/pages
  /analytics.tsx          # Analytics page with charts and graphs
  /moderation.tsx         # Content moderation page to manage posts
  /users.tsx              # User management page
/app
  /components
    /AnalyticsChart.tsx   # Chart.js component for analytics visualization
    /PostTable.tsx        # Table component for viewing and managing posts
    /Sidebar.tsx          # Sidebar component for navigation
    /UserTable.tsx        # Table component for user management
/tailwind.config.js       # Tailwind CSS configuration
/next.config.js           # Next.js configuration
/package.json             # Project dependencies and scripts
```

---

## Dependencies

### 1. **Next.js**

- Next.js is used for building the React-based server-side rendered web application.
- Official Docs: [Next.js](https://nextjs.org/)

### 2. **Tailwind CSS**

- Tailwind CSS is used for styling the components with utility-first CSS classes.
- Official Docs: [Tailwind CSS](https://tailwindcss.com/)

### 3. **Chart.js**

- Chart.js is used for data visualization, providing dynamic and interactive charts for displaying analytics data.
- Official Docs: [Chart.js](https://www.chartjs.org/)

### 4. **SWR**

- SWR is used for fetching data from APIs and caching the responses for performance optimization.
- Official Docs: [SWR](https://swr.vercel.app/)

---

## Features

### User Management

The **User Management** section allows administrators to:
- View a list of users.
- Track user activity, including the number of posts, referrals, and active status.
- Assign and manage user roles (e.g., Admin, Moderator, User).

The user data is fetched using the **SWR** hook from the backend API, and displayed in a **UserTable** component.

### Content Moderation

The **Content Moderation** section helps admins:
- Monitor posts and track metrics like views, shares, comments, and engagement.
- Ensure the content adheres to platform guidelines.

Post data is fetched using the **SWR** hook, and displayed in a **PostTable** component.

### Analytics

The **Analytics** section visualizes user and content engagement over time. 
- Admins can view trends and patterns in user behavior, such as the number of views, likes, shares, and comments.
- Charts are rendered using **Chart.js** for interactive, real-time data visualization.

---

## Additional Notes

### Responsiveness

This project uses **Tailwind CSS** for responsive design. The layout is mobile-first, ensuring that the admin dashboard is fully functional on smaller screens. 

You can customize the breakpoints and layouts as per your needs by modifying the Tailwind configuration file `tailwind.config.js`.

### API Integration

The dashboard integrates with the provided API (`NEXT_PUBLIC_API_URL`) to fetch data for users, posts, and analytics. The data is fetched dynamically using **SWR**, which handles caching and revalidation to ensure optimal performance.

---

### Submit the Following:

- **GitHub Repository Link**: https://github.com/Rushikasrithamaddula11/Admin-by-Next.js
