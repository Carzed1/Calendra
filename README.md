
# Calendra - A Modern Calendly Clone

A full-stack scheduling application built with Next.js 15, featuring seamless calendar integration, user authentication, and a modern UI.

##  Tech Stack

### Frontend
- **Next.js 15** - React framework with App Router and server components
- **React 19** - Latest React with concurrent features
- **TypeScript** - Type-safe JavaScript superset
- **Tailwind CSS v4** - Utility-first CSS framework
- **Shadcn UI** - Beautiful, accessible component library

### Backend & Database
- **Drizzle ORM** - Type-safe SQL ORM for TypeScript
- **Neon** - Serverless Postgres database with branching

### Authentication & Integrations
- **Clerk** - Complete authentication and user management
- **Google Calendar API** - Calendar synchronization and event management

##  Getting Started

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn
- A Neon database account
- Google Cloud Console project (for Calendar API)
- Clerk account for authentication

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Carzed1/Calendra.git
   cd Calendra
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   
   Create a `.env.local` file in the root directory:
   ```env
   # Clerk Authentication
   NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
   CLERK_SECRET_KEY=your_clerk_secret_key
   NEXT_PUBLIC_CLERK_SIGN_IN_URL=/login
   NEXT_PUBLIC_CLERK_SIGN_UP_URL=/register
   NEXT_PUBLIC_CLERK_SIGN_IN_FORCE_REDIRECT_URL=/events
   NEXT_PUBLIC_CLERK_SIGN_UP_FORCE_REDIRECT_URL=/events
   
   # Database
   DATABASE_URL=your_neon_database_connection_string
   
   # Google Calendar Integration
   GOOGLE_OAUTH_CLIENT_ID=your_google_oauth_client_id
   GOOGLE_OAUTH_CLIENT_SECRET=your_google_oauth_client_secret
   GOOGLE_OAUTH_REDIRECT_URL=your_google_oauth_redirect_url
   ```

4. **Run database migrations**
   ```bash
   npm run db:migrate
   ```

5. **Start the development server**
   ```bash
   npm run dev
   ```

6. **Open your browser**
   
   Navigate to [http://localhost:3000](http://localhost:3000)


