This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Supabase Integration

#### Ran from :~/solidity/supabase/supabase-nextjs

This application demonstrates a full-featured authentication and user management system built with Next.js 14 (App Router) and Supabase. It includes:

### Features
- 🔐 Email & Password Authentication
- 📝 User Profile Management
- 🖼️ Avatar Upload & Management
- 🔄 Server-Side Session Handling
- 🛡️ Protected Routes
- 🔒 Secure API Routes

### Authentication Flow
- Sign Up: Users can create new accounts with email and password
- Sign In: Existing users can log in securely
- Sign Out: Users can end their sessions
- Email Verification: New users receive verification emails
- Password Reset: Users can reset forgotten passwords

### User Profile Features
- Profile Information: Users can view and edit their:
  - Full Name
  - Username
  - Website
  - Avatar
- Real-time Updates: Profile changes are reflected immediately
- Data Persistence: All user data is stored in Supabase

### Technical Implementation
- Server Components: Leverages Next.js 14 server components for optimal performance
- Client Components: Uses React client components for interactive features
- Middleware: Implements Supabase auth middleware for session management
- Type Safety: Full TypeScript implementation
- Environment Variables: Secure configuration management

### Directory Structure
```
src/
├── app/                    # Next.js app router
│   ├── account/           # Protected account pages
│   ├── auth/              # Authentication routes
│   └── actions.ts         # Server actions
├── utils/
│   └── supabase/         # Supabase utility functions
│       ├── client.ts     # Browser client
│       ├── server.ts     # Server client
│       └── middleware.ts # Auth middleware
```

## Getting Started

1. Set up your Supabase project and get your credentials
2. Create a `.env.local` file with:
```env
NEXT_PUBLIC_SUPABASE_URL=your-project-url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your-anon-key
```

3. Run the development server:
```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
