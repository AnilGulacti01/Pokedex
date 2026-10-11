# Overview

This is a Pokédex web application built as a full-stack project with a React frontend and Express backend. The application allows users to browse and view detailed information about Pokémon, including their stats, abilities, moves, and sprites. It features a responsive design with a Pokédex-style interface and multi-language support.

# User Preferences

Preferred communication style: Simple, everyday language.

# System Architecture

## Frontend Architecture
- **Framework**: React with TypeScript using Vite as the build tool
- **Routing**: Wouter for client-side routing
- **State Management**: TanStack Query (React Query) for server state management and caching
- **UI Components**: Radix UI primitives with shadcn/ui component library
- **Styling**: Tailwind CSS with CSS custom properties for theming
- **Type Safety**: Full TypeScript implementation with strict configuration

## Backend Architecture
- **Runtime**: Node.js with Express.js framework
- **Language**: TypeScript with ES modules
- **Development**: tsx for development server with hot reloading
- **API Structure**: RESTful API with `/api` prefix routing
- **Error Handling**: Centralized error handling middleware
- **Request Logging**: Custom middleware for API request logging with response capture

## Data Storage Solutions
- **Database**: PostgreSQL configured via Drizzle ORM
- **Schema Management**: Drizzle Kit for migrations and schema management
- **Connection**: Neon serverless PostgreSQL adapter
- **Fallback Storage**: In-memory storage implementation for development
- **Session Management**: PostgreSQL session store with connect-pg-simple

## Authentication and Authorization
- **User Schema**: Basic user model with username/password fields
- **Session Storage**: PostgreSQL-backed sessions
- **Password Security**: Prepared for hashed password storage
- **User Management**: CRUD operations interface defined in storage layer

## Design System
- **Component Library**: shadcn/ui with New York style variant
- **Theme System**: CSS custom properties with light/dark mode support
- **Typography**: Custom font stack including Segoe UI, DM Sans, Fira Code, and Geist Mono
- **Responsive Design**: Mobile-first approach with Tailwind breakpoints
- **Accessibility**: Radix UI primitives ensure WCAG compliance

## Development Tools
- **Build System**: Vite with React plugin and custom error overlay
- **Code Quality**: TypeScript strict mode with comprehensive type checking
- **Hot Reload**: Vite HMR with runtime error modal for development
- **Path Mapping**: Absolute imports with @ aliases for clean imports

# External Dependencies

## Third-Party APIs
- **PokéAPI**: Primary data source for Pokémon information (https://pokeapi.co/api/v2)
  - Pokemon list and details
  - Abilities, moves, and type information
  - Sprite images and artwork
  - Multi-language support for names and descriptions

## UI and Component Libraries
- **Radix UI**: Headless UI primitives for accessibility and behavior
- **shadcn/ui**: Pre-built component library built on Radix UI
- **Lucide React**: Icon library for consistent iconography
- **class-variance-authority**: Utility for component variant management

## Development and Build Tools
- **Vite**: Fast build tool with HMR support
- **TanStack Query**: Server state management and caching
- **Wouter**: Lightweight routing library
- **Tailwind CSS**: Utility-first CSS framework
- **PostCSS**: CSS processing with Tailwind and Autoprefixer

## Database and ORM
- **Drizzle ORM**: Type-safe database toolkit
- **Neon Database**: Serverless PostgreSQL provider
- **Drizzle Kit**: Schema management and migration tool

## External Services Integration
- **Replit Platform**: Development environment integration with custom plugins
- **Font Services**: Google Fonts integration for typography
- **Image Resources**: Pokemon Showdown sprites for type icons