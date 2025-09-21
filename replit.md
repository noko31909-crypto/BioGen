# Biography Builder Application

## Overview

A full-stack web application for creating and managing professional biographies. Users can generate structured biographical profiles with sections for background, achievements, skills, and goals. The application features a modern React frontend with shadcn/ui components and an Express.js backend with PostgreSQL database integration.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React with TypeScript and Vite for fast development and building
- **UI Components**: shadcn/ui component library built on Radix UI primitives
- **Styling**: Tailwind CSS with custom CSS variables for theming
- **State Management**: TanStack Query for server state management and caching
- **Routing**: Wouter for lightweight client-side routing
- **Form Management**: React Hook Form with Zod validation resolvers

### Backend Architecture
- **Framework**: Express.js with TypeScript for type-safe server development
- **Database**: PostgreSQL with Drizzle ORM for type-safe database operations
- **Schema Management**: Drizzle Kit for database migrations and schema management
- **Validation**: Zod schemas for runtime type validation and API request/response validation
- **Storage Pattern**: Interface-based storage abstraction with in-memory implementation for development

### Database Design
- **Users Table**: Basic user authentication with username/password
- **Profiles Table**: Biography data with structured fields (name, background, achievements, skills, goals)
- **Timestamps**: Automatic creation and update tracking for profiles
- **Primary Keys**: UUID-based identifiers for all entities

### API Architecture
- **REST Endpoints**: Standard CRUD operations for profiles
- **Error Handling**: Centralized error middleware with proper HTTP status codes
- **Request Logging**: Detailed logging for API requests with response times
- **Validation Middleware**: Zod schema validation for all incoming requests

### Development Environment
- **Build System**: Vite for frontend bundling, esbuild for backend compilation
- **Development Server**: Hot module replacement and automatic restart capabilities
- **Type Checking**: Shared TypeScript configuration across frontend, backend, and shared modules
- **Code Organization**: Monorepo structure with shared schema definitions

## External Dependencies

### Database Services
- **Neon Database**: Serverless PostgreSQL hosting (@neondatabase/serverless)
- **Connection Pooling**: Built-in connection management for serverless environments

### UI and Styling
- **Radix UI**: Comprehensive set of unstyled, accessible UI components
- **Tailwind CSS**: Utility-first CSS framework with custom design tokens
- **Lucide React**: Icon library for consistent iconography
- **Google Fonts**: Inter, Crimson Text, and Fira Code font families

### Form and Validation
- **React Hook Form**: Performance-focused form library with minimal re-renders
- **Zod**: TypeScript-first schema validation for runtime safety
- **Hookform Resolvers**: Integration bridge between React Hook Form and Zod

### Development Tools
- **Replit Plugins**: Integration with Replit development environment
- **PostCSS**: CSS processing with Tailwind and Autoprefixer plugins
- **TypeScript**: Static type checking across the entire application stack

### Runtime Libraries
- **Date-fns**: Date manipulation and formatting utilities
- **Class Variance Authority**: Type-safe CSS class composition
- **CLSX**: Conditional CSS class concatenation utility
- **Nanoid**: URL-safe unique ID generation