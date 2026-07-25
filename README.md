<!--
SEO Keywords: compyle showcase, Compyle applications, app gallery, built with Compyle, Next.js app showcase, Compyle gallery, discover apps, product showcase, app discovery platform, Compyle-built applications
-->

<div align="center">

# compyle-1

[![Next.js](https://img.shields.io/badge/Next.js-16-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=white)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-4-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Drizzle ORM](https://img.shields.io/badge/Drizzle-ORM-C5F74F?style=for-the-badge)](https://orm.drizzle.team/)
[![Neon](https://img.shields.io/badge/Neon-Database-00E59B?style=for-the-badge&logo=neon&logoColor=white)](https://neon.tech/)
[![Better Auth](https://img.shields.io/badge/Better_Auth-Auth-4F46E5?style=for-the-badge)](https://better-auth.com/)
[![shadcn/ui](https://img.shields.io/badge/shadcn%2Fui-Components-000000?style=for-the-badge)](https://ui.shadcn.com/)

**Discover incredible applications built with Compyle. From productivity tools to creative platforms, explore what builders are creating.**

[Live Gallery](https://compyle.tracepanic.com) · [Compyle Platform](https://github.com/yethikrishna/compyle) · [Report Bug](https://github.com/yethikrishna/compyle-1/issues)

</div>

---

## Overview

**compyle-1** is the official showcase gallery for applications built with the Compyle platform. It is a beautifully designed Next.js 16 application featuring a curated gallery of Compyle-built apps, complete with screenshots, descriptions, categories, and user engagement features. The gallery uses Drizzle ORM with Neon serverless Postgres, Better Auth for authentication, ImageKit for media management, Resend for transactional emails, and shadcn/ui with Tailwind CSS v4 for the interface.

## Features

- **App Gallery** - Curated showcase of applications built with Compyle
- **Categories & Filtering** - Browse apps by category, popularity, and recency
- **App Details** - Rich app pages with screenshots, descriptions, and links
- **User Authentication** - Better Auth for secure user accounts and sessions
- **Image Management** - ImageKit integration for optimized image delivery
- **Email Notifications** - Resend for transactional emails and updates
- **SEO Optimized** - next-sitemap for comprehensive sitemap generation
- **Dark/Light Mode** - Theme switching with next-themes
- **Data Tables** - TanStack Table for admin dashboards
- **State Management** - Zustand for lightweight client state
- **Form Handling** - TanStack React Form with Zod validation
- **Analytics** - Vercel Analytics built-in
- **Type-Safe Env** - @t3-oss/env-nextjs for validated environment variables

## Tech Stack

| Category | Technology | Version |
|----------|-----------|---------|
| Framework | Next.js (App Router) | 16.1.0 |
| UI Library | React | 19.2.x |
| Styling | Tailwind CSS | 4.x |
| UI Components | shadcn/ui (New York), Radix UI | Latest |
| Database | Neon (Serverless Postgres) | Latest |
| ORM | Drizzle ORM | 0.45.x |
| Auth | Better Auth | 1.3.x |
| Media | ImageKit | 6.x / 5.x |
| Email | Resend + React Email | 6.x / 1.x |
| Data Fetching | TanStack React Query | 5.x |
| Tables | TanStack React Table | 8.x |
| Forms | TanStack React Form + Zod | 1.x / 4.x |
| State | Zustand | 5.x |
| Charts | Recharts | 2.x |
| SEO | next-sitemap | 4.x |
| Language | TypeScript | 5.x |
| Package Manager | pnpm | Latest |

## Quick Start

### Prerequisites

- Node.js 18+
- pnpm
- A Neon Postgres database
- An ImageKit account
- A Resend account for emails

### Installation

```bash
# Clone the repository
git clone https://github.com/yethikrishna/compyle-1.git
cd compyle-1

# Install dependencies
pnpm install

# Set up environment variables
cp .example.env .env.local
# Edit .env.local with your credentials

# Run database migrations
pnpm db:migrate

# Start development server
pnpm dev
```

### Environment Variables

```env
# Database
DATABASE_URL=your_neon_database_url

# Better Auth
BETTER_AUTH_SECRET=your_auth_secret
BETTER_AUTH_URL=http://localhost:3000

# ImageKit
NEXT_PUBLIC_IMAGEKIT_URL_ENDPOINT=your_imagekit_url
IMAGEKIT_PRIVATE_KEY=your_imagekit_private_key
IMAGEKIT_PUBLIC_KEY=your_imagekit_public_key

# Resend
RESEND_API_KEY=your_resend_api_key

# App URL
NEXT_PUBLIC_APP_URL=http://localhost:3000
```

### Database Commands

```bash
# Generate migrations
pnpm db:generate

# Run migrations
pnpm db:migrate

# Push schema changes
pnpm db:push

# Open Drizzle Studio
pnpm db:studio
```

### Development

```bash
pnpm dev      # Start dev server
pnpm build    # Build for production
pnpm start    # Start production server
pnpm lint     # Run ESLint
```

## Project Structure

```
compyle-1/
├── app/                    # Next.js App Router pages
├── components/            # React components
│   └── ui/               # shadcn/ui components
├── data/                  # Static data and configurations
├── db/                    # Database schema and config
│   └── schema.ts         # Drizzle schema definitions
├── emails/                # React Email templates
├── hooks/                 # Custom React hooks
├── icons/                 # Custom icon components
├── lib/                   # Utility functions
├── providers/             # React context providers
├── public/                # Static assets
├── server/                # Server-side logic
├── store/                 # Zustand state stores
├── schema/                # Validation schemas
├── types/                 # TypeScript type definitions
├── drizzle.config.ts      # Drizzle configuration
├── next.config.ts         # Next.js configuration
├── next-sitemap.config.js # Sitemap configuration
└── package.json           # Dependencies
```

## Deployment

Deployed at [compyle.tracepanic.com](https://compyle.tracepanic.com).

### Vercel Deployment

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/yethikrishna/compyle-1)

After deploying, run migrations:
```bash
pnpm db:migrate
```

## Contributing

Contributions are welcome! Please feel free to submit pull requests.

1. Fork the repository
2. Create a feature branch
3. Make changes with tests if applicable
4. Submit a pull request

## Related Projects

- [compyle](https://github.com/yethikrishna/compyle) - The main Compyle app building platform
- [yetisai](https://github.com/yethikrishna/yetisai) - Yeti AI platform
- [indu-foundation](https://github.com/yethikrishna/indu-foundation) - INDU programming language

---

<div align="center">

Built with passion by [Yethikrishna R](https://github.com/yethikrishna)

</div>
