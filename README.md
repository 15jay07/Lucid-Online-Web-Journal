# Lucid – Online Web Journal

Lucid is a full-stack online journaling application that allows users to record their daily thoughts, organize journal entries, track their moods, and visualize emotional patterns through analytics.

## Features

- User authentication and account management
- Create, edit, and delete journal entries
- Organize journal entries into collections
- Save and manage journal drafts
- Mood tracking with mood scores
- Interactive mood analytics dashboard
- Mood-related image integration using Pixabay API
- Route protection and request security

## Technology Stack

| Category | Technologies |
|---|---|
| Frontend | React.js, Next.js, JavaScript |
| Styling | Tailwind CSS |
| Authentication | Clerk |
| Database | PostgreSQL |
| ORM | Prisma |
| Security | Arcjet |
| API Integration | Pixabay API |
| Data Visualization | Recharts |

## Project Structure

```text
Lucid-Online-Web-Journal/
├── actions/       # Server-side application operations
├── app/           # Application pages and layouts
├── components/    # Reusable UI components
├── data/          # Static application data
├── hooks/         # Custom React hooks
├── lib/           # Database and utility functions
├── prisma/        # Database schema and migrations
├── public/        # Static assets
├── middleware.js  # Authentication and security middleware
└── package.json   # Dependencies and scripts
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/15jay07/Lucid-Online-Web-Journal.git
cd Lucid-Online-Web-Journal
```

### 2. Install dependencies

```bash
npm install
```

### 3. Configure environment variables

Create a `.env.local` file in the project root.

Add the following variables with your own credentials:

```env
DATABASE_URL="your_postgresql_connection_string"

NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY="your_clerk_publishable_key"
CLERK_SECRET_KEY="your_clerk_secret_key"

ARCJET_KEY="your_arcjet_key"
PIXABAY_API_KEY="your_pixabay_api_key"
```

Never commit actual API keys or database credentials.

### 4. Generate Prisma Client

```bash
npx prisma generate
```

### 5. Run database migrations

```bash
npx prisma migrate deploy
```

### 6. Start the development server

```bash
npm run dev
```

Open http://localhost:3000 in your browser.

## Database Design

The application uses PostgreSQL with Prisma ORM.

Main database models:

- User
- Collection
- Entry
- Draft

These models manage user accounts, journal collections, individual entries, and saved drafts.

## Author

**Jay Shankar Giri**

GitHub: [15jay07](https://github.com/15jay07)
