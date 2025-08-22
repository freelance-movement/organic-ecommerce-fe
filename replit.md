# Overview

VietRoot is a Vietnamese organic products e-commerce platform showcasing authentic agricultural products from Vietnamese farmers. The application features a modern, responsive homepage with a nature-inspired design emphasizing freshness, sustainability, and cultural authenticity. The platform aims to connect consumers with high-quality organic products while promoting Vietnamese agricultural heritage.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
The frontend is built using React with TypeScript, utilizing a component-based architecture with modern UI patterns:

- **React Router**: Uses Wouter for lightweight client-side routing
- **UI Components**: Implements shadcn/ui component library with Radix UI primitives for accessibility and consistency
- **Styling**: Tailwind CSS with custom VietRoot brand colors (greens and earth tones) and CSS custom properties for theming
- **State Management**: TanStack React Query for server state management with custom query client configuration
- **Form Handling**: React Hook Form with Zod validation schemas for type-safe form management

## Backend Architecture
The backend follows a layered Express.js architecture with TypeScript:

- **Server Framework**: Express.js with middleware for logging, error handling, and request processing
- **Storage Layer**: Abstracted storage interface supporting both in-memory storage (development) and database implementations
- **Development Setup**: Vite integration for hot module replacement and development server proxy
- **Build Process**: ESBuild for server bundling and Vite for client bundling

## Database Design
The application uses Drizzle ORM with PostgreSQL:

- **ORM**: Drizzle ORM for type-safe database operations with generated TypeScript types
- **Schema**: Centralized schema definitions in shared directory for type consistency across client and server
- **Migrations**: Drizzle Kit for database migrations and schema management
- **Database Provider**: Configured for Neon Database (serverless PostgreSQL)

## Development and Build System
Modern tooling stack optimized for developer experience:

- **Build Tool**: Vite for fast development server and optimized production builds
- **TypeScript**: Strict TypeScript configuration with path mapping for clean imports
- **Package Management**: NPM with lock file for consistent dependency resolution
- **Hot Reload**: Vite HMR with React Fast Refresh for instant development feedback

# External Dependencies

## Database Services
- **Neon Database**: Serverless PostgreSQL provider for production database hosting
- **Drizzle ORM**: Type-safe database toolkit with PostgreSQL dialect support

## UI and Component Libraries
- **shadcn/ui**: Modern React component library built on Radix UI primitives
- **Radix UI**: Unstyled, accessible UI components for complex interactions
- **Tailwind CSS**: Utility-first CSS framework with custom brand color extensions
- **Lucide React**: Icon library for consistent iconography throughout the application

## Development and Build Tools
- **Vite**: Modern build tool with TypeScript support and development server
- **ESBuild**: Fast JavaScript bundler for server-side code compilation
- **PostCSS**: CSS processing with Tailwind CSS and Autoprefixer plugins
- **Replit Integration**: Development environment plugins for cloud-based coding

## Runtime and Utilities
- **TanStack React Query**: Server state management with caching and synchronization
- **React Hook Form**: Performant form library with validation integration
- **Zod**: TypeScript-first schema validation for runtime type checking
- **date-fns**: Date manipulation library for formatting and calculations
- **Wouter**: Minimalist router for React applications