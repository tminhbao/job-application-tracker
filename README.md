# 🎯 CareerTrack — Modern Job Application Tracker

An all-in-one, production-ready job application tracking system designed to streamline your career search. Built with the latest **Next.js 16 (App Router)**, **MongoDB**, **TypeScript**, and **Tailwind CSS**.

---

## 🌟 Overview

Searching for a job can quickly become overwhelming with dozens of applications across multiple platforms. **CareerTrack** provides a centralized, intuitive dashboard to help job seekers organize, track, and analyze their job application status in real-time.

### ✨ Key Features

- 📊 **Interactive Analytics Dashboard**: Visual statistics on application statuses (Applied, Interviewing, Offered, Rejected).
- 📝 **Full Application CRUD**: Create, read, update, and delete application entries with rich details (Job Title, Company, Salary Range, Location, Job URL, Notes).
- 🔍 **Advanced Filtering & Search**: Instant filtering by status, date applied, or company name.
- ⚡ **Next.js 16 App Router & Server Actions**: Blazing fast rendering and seamless database mutations without extra API boilerplate.
- 🗄️ **MongoDB & Mongoose**: Secure and scalable document storage for application data.
- 🎨 **Modern Responsive UI**: Built with Tailwind CSS and Shadcn UI components for high accessibility and dark mode aesthetics.
- 🔐 **Authentication & Security**: Protected client and server routes ensuring personal application data stays private.

---

## 🛠️ Tech Stack

- **Framework**: Next.js 16 (React 19)
- **Language**: TypeScript
- **Database**: MongoDB & Mongoose
- **Styling**: Tailwind CSS
- **Deployment**: Vercel

---

## 🚀 Getting Started

Follow these steps to set up and run the project locally on your machine.

### Prerequisites

Ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v18.0 or higher)
- [npm](https://www.npmjs.com/) or [pnpm](https://pnpm.io/)
- A free [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) database cluster

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/job-application-tracker.git
cd job-application-tracker
```

### 2. Install Dependencies

```bash
npm install
# or
pnpm install
```

### 3. Configure Environment Variables

Create a `.env.local` file in the root folder and configure your MongoDB connection URL:

```env
MONGODB_URI=mongodb+srv://<username>:<password>@cluster0.mongodb.net/job_tracker?retryWrites=true&w=majority
NEXT_PUBLIC_APP_URL=http://localhost:3000
```

> **Note**: Make sure to replace `<username>` and `<password>` with your actual MongoDB Atlas credentials.

### 4. Run the Development Server

```bash
npm run dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to view the application.

---

## 📁 Project Structure

```text
├── app/                  # Next.js 16 App Router (pages & layouts)
│   ├── (auth)/           # Authentication routes
│   ├── dashboard/        # Dashboard view & tracking management
│   ├── api/              # Route handlers / API routes
│   └── layout.tsx        # Global layout
├── components/           # Reusable UI components
│   ├── ui/               # Base UI components
│   └── tracker/          # Specific components for tracking logic
├── lib/                  # Database connections and utility functions
│   ├── mongodb.ts        # MongoDB client configuration
│   └── actions/          # Next.js Server Actions
├── models/               # Mongoose schemas (Job, User, etc.)
└── public/               # Static assets
```

---

## 🌐 Deployment

The easiest way to deploy this Next.js app is via the [Vercel Platform](https://vercel.com/new).

1. Push your code to GitHub.
2. Import the repository into Vercel.
3. Set your Environment Variables (`MONGODB_URI`).
4. Click **Deploy**.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

Special thanks to the open-source community and educational resources for inspiring this project workflow. <sup>[[ref](https://www.youtube.com/watch?v=vCIsrOGNhas)]</sup>
