# ParkEASE - Frontend

> A modern, intelligent parking management system that simplifies urban parking through real-time spot availability, seamless reservations, and digital ticket validation.

## Project Overview

**ParkEASE** is a comprehensive web-based parking reservation platform designed to optimize urban parking management. This repository contains the frontend application built with Angular 19, providing users with an intuitive interface to discover, reserve, and manage parking spots across multiple cities.

The system addresses common urban parking challenges by offering real-time availability tracking, advance reservations, and streamlined ticket management, reducing time spent searching for parking and improving overall urban mobility.

## Key Features

### Authentication & User Management

- Secure user registration and login system
- JWT-based authentication with automatic token management
- Password reset functionality
- Protected routes with authentication guards
- Session persistence and automatic renewal

### Parking Spot Management

- Browse available parking spots by city
- Real-time availability status
- Detailed spot information and pricing
- Support for both standard and bus parking
- Location-based search capabilities

### Reservation System

- Intuitive booking interface with date/time selection
- Dedicated reservation forms for cars and buses
- Reservation history and management dashboard
- Booking modifications and cancellations
- Automated confirmation system

### Ticket Validation

- Digital ticket generation and management
- QR code-based validation system
- Real-time ticket status updates
- Electronic receipt storage

### User Experience

- Responsive design optimized for all devices
- Material Design components for consistent UI
- Intuitive navigation with clear user flows
- Real-time feedback and error handling
- Accessibility-first approach

## Project Structure

```
parcheggio-frontend/
├── src/
│   ├── app/
│   │   ├── components/          # Feature components
│   │   │   ├── auth-modal/      # Authentication modal dialog
│   │   │   ├── contact/         # Contact page
│   │   │   ├── home/            # Landing page
│   │   │   ├── info/            # Information page
│   │   │   ├── login/           # Login form
│   │   │   ├── register/        # Registration form
│   │   │   ├── reset-password/  # Password recovery
│   │   │   ├── parking-spot-list/    # Parking spot browser
│   │   │   ├── reservation-form/     # Car reservation form
│   │   │   ├── reservation-bus-form/ # Bus reservation form
│   │   │   ├── reservation-list/     # User reservations dashboard
│   │   │   └── ticket-validation/    # Ticket validation interface
│   │   │
│   │   ├── services/            # Core services
│   │   │   ├── auth.service.ts         # Authentication logic
│   │   │   ├── auth.guard.ts           # Route protection
│   │   │   ├── jwt.interceptor.ts      # JWT token injection
│   │   │   ├── debug.interceptor.ts    # HTTP debugging
│   │   │   ├── parking-spot.service.ts # Parking spot data
│   │   │   └── city.service.ts         # City management
│   │   │
│   │   ├── app.component.*      # Root component
│   │   ├── app.config.ts        # Application configuration
│   │   └── app.routes.ts        # Routing configuration
│   │
│   ├── assets/                  # Static resources
│   ├── index.html               # Main HTML file
│   ├── main.ts                  # Application entry point
│   └── styles.css               # Global styles
│
├── angular.json                 # Angular CLI configuration
├── package.json                 # Dependencies and scripts
├── tsconfig.json                # TypeScript configuration
└── Dockerfile                   # Container configuration
```

## Technology Stack

### Core Framework

- **Angular 19.2** - Latest Angular framework with standalone components
- **TypeScript** - Type-safe development
- **RxJS 7.8** - Reactive programming for async operations

### UI/UX

- **Angular Material 19.2** - Material Design component library
- **Angular CDK** - Component development kit for custom components
- **CSS3** - Custom styling and animations

### Development Tools

- **Angular CLI 19.2** - Command-line interface for project management
- **Karma** - Unit testing framework
- **Jasmine** - Testing library

### Architecture Patterns

- **Standalone Components** - Modern Angular architecture
- **Reactive Forms** - Type-safe form handling
- **HTTP Interceptors** - Centralized request/response handling
- **Route Guards** - Navigation security
- **Service-based Architecture** - Separation of concerns

## Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn
- Angular CLI 19.2.5

### Installation

```bash
# Clone the repository
git clone <repository-url>
cd ParkEASE_FE/parcheggio-frontend

# Install dependencies
npm install
```

### Development Server

This project was generated using [Angular CLI](https://github.com/angular/angular-cli) version 19.2.5.

## Development server

To start a local development server, run:

```bash
ng serve
```

Once the server is running, open your browser and navigate to `http://localhost:4200/`. The application will automatically reload whenever you modify any of the source files.

## Code scaffolding

Angular CLI includes powerful code scaffolding tools. To generate a new component, run:

```bash
ng generate component component-name
```

For a complete list of available schematics (such as `components`, `directives`, or `pipes`), run:

```bash
ng generate --help
```

## Building

To build the project run:

```bash
ng build
```

This will compile your project and store the build artifacts in the `dist/` directory. By default, the production build optimizes your application for performance and speed.

## Running unit tests

To execute unit tests with the [Karma](https://karma-runner.github.io) test runner, use the following command:

```bash
ng test
```

## Running end-to-end tests

For end-to-end (e2e) testing, run:

```bash
ng e2e
```

Angular CLI does not come with an end-to-end testing framework by default. You can choose one that suits your needs.

## Additional Resources

For more information on using the Angular CLI, including detailed command references, visit the [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli) page.
