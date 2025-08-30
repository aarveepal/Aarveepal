# Overview

This is a professional portfolio website for Aarvee Pal, an MBA candidate at IIM Kashipur. The application is built as a single-page application showcasing his academic projects, professional skills, certificates, and creative portfolio. The site features a modern, clean design with sections for his live projects (brand management, product management, HR), certificates, skills, and a contact form for potential collaborators or employers.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **React SPA**: Built with React 18 using functional components and hooks
- **Routing**: Uses Wouter for lightweight client-side routing
- **Styling**: Tailwind CSS with shadcn/ui component library for consistent design
- **State Management**: React Query for server state management and React hooks for local state
- **Form Handling**: React Hook Form with Zod validation for type-safe form submissions
- **Build Tool**: Vite for fast development and optimized production builds

## Backend Architecture
- **Server Framework**: Express.js with TypeScript for type safety
- **Database ORM**: Drizzle ORM with PostgreSQL dialect for type-safe database operations
- **Database Provider**: Neon Database (serverless PostgreSQL)
- **File Uploads**: Multer for handling PDF certificate uploads with file validation
- **Development Setup**: Custom Vite integration for seamless development experience

## Data Storage Solutions
- **Primary Database**: PostgreSQL via Neon Database for production scalability
- **Schema Design**: Three main entities - users, contacts, and certificates
- **File Storage**: Local file system for PDF certificates with organized directory structure
- **In-Memory Fallback**: MemStorage class provides development/testing capability without database

## Authentication and Authorization
- **Current State**: Basic user schema exists but authentication is not actively implemented
- **Session Management**: Express sessions configured with PostgreSQL store (connect-pg-simple)
- **Security**: Basic input validation using Zod schemas for API endpoints

## Component Architecture
- **Design System**: shadcn/ui components with Radix UI primitives for accessibility
- **Layout Pattern**: Section-based layout with smooth scrolling navigation
- **Responsive Design**: Mobile-first approach with Tailwind responsive utilities
- **Component Structure**: Organized by feature with reusable UI components

# External Dependencies

## Database and Storage
- **Neon Database**: Serverless PostgreSQL for production data storage
- **Drizzle Kit**: Database migrations and schema management
- **Multer**: File upload handling for certificate PDFs

## UI and Styling
- **Tailwind CSS**: Utility-first CSS framework for styling
- **shadcn/ui**: Pre-built component library based on Radix UI
- **Radix UI**: Accessible component primitives for complex UI elements
- **Lucide React**: Icon library for consistent iconography

## Development and Build Tools
- **Vite**: Build tool and development server with React plugin
- **TypeScript**: Type safety across frontend and backend
- **ESBuild**: Fast bundling for production server build
- **PostCSS**: CSS processing with Tailwind and Autoprefixer

## Form and Data Management
- **React Hook Form**: Form state management and validation
- **React Query (TanStack Query)**: Server state management and caching
- **Zod**: Runtime type validation for forms and API endpoints
- **React Router (Wouter)**: Lightweight client-side routing

## Communication and Notifications
- **Contact Form Integration**: Ready for email service integration (nodemailer placeholder)
- **Toast Notifications**: User feedback for form submissions and actions

## Development Environment
- **Replit Integration**: Specialized plugins for Replit development environment
- **Hot Module Replacement**: Fast refresh during development
- **Error Overlay**: Runtime error display in development mode