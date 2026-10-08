# 🏏 BPL Official

> A modern, responsive cricket tournament web application built with **Next.js, React, TypeScript, Redux Toolkit, SCSS, and modern frontend technologies**.

**BPL Official** is a cricket tournament web application designed to provide a centralized platform for **teams, players, matches, auctions, points tables, galleries, live scores, and tournament administration**.

The application follows a **modular, feature-based architecture** with reusable components, centralized state management, service layers, TypeScript type definitions, responsive SCSS styling, and scalable project organization.

---

## 🌐 Live Application

**BPL Official:**
https://bpl-official.vercel.app/

---

# ✨ Features

* 🏏 BPL tournament information
* 👥 Teams and team information
* 🧑‍💼 Player information
* 🏟️ Match information
* 🔴 Live match and score support
* 🔨 Auction management
* 💰 Bid and purse tracking
* 📊 Points table
* 🖼️ Tournament gallery
* 🛠️ Admin dashboard
* 🔐 Authentication architecture
* 🔄 API service integration
* ⚡ Real-time communication with Socket.IO
* 🧠 Application state management
* 🎨 Responsive SCSS architecture
* 📱 Mobile-friendly interface
* 💻 Desktop and tablet support
* 🎬 Smooth animations with Framer Motion
* 🔔 Toast notifications with Sonner
* 🚨 Interactive alerts with SweetAlert2
* 📝 Form handling with Formik and React Hook Form
* ✅ Schema validation with Yup and Zod
* 🖼️ Image optimization with Next.js and Sharp
* 📘 Type-safe development with TypeScript
* 🧩 Reusable UI components
* 📦 Modular feature-based architecture

---

# 🛠️ Tech Stack

## Frontend

| Technology    | Purpose         |
| ------------- | --------------- |
| Next.js 16    | React framework |
| React 19      | UI development  |
| TypeScript    | Static typing   |
| SCSS / Sass   | Styling         |
| React Icons   | Icons           |
| Framer Motion | Animations      |

## State Management

| Technology    | Purpose                                   |
| ------------- | ----------------------------------------- |
| Redux Toolkit | Application state management              |
| React Redux   | React-Redux integration                   |
| RTK Query     | API fetching, caching and synchronization |

## Forms & Validation

| Technology      | Purpose              |
| --------------- | -------------------- |
| Formik          | Form management      |
| React Hook Form | Form management      |
| Yup             | Schema validation    |
| Zod             | Type-safe validation |

## Real-Time & Communication

| Technology | Purpose                 |
| ---------- | ----------------------- |
| Socket.IO  | Real-time communication |

## UI Feedback

| Technology  | Purpose                         |
| ----------- | ------------------------------- |
| Sonner      | Toast notifications             |
| SweetAlert2 | Alerts and confirmation dialogs |

## Image Processing

| Technology | Purpose            |
| ---------- | ------------------ |
| Sharp      | Image optimization |

## Development

| Technology     | Purpose            |
| -------------- | ------------------ |
| ESLint         | Code quality       |
| TypeScript     | Type checking      |
| React Compiler | React optimization |

---

# 🏗️ Architecture

BPL Official follows a **feature-based and modular frontend architecture**.

The application separates:

```text
Routing
   ↓
Features
   ↓
Components
   ↓
Hooks
   ↓
Services / Store
   ↓
API / External Services
```

This structure helps keep the application:

* Modular
* Reusable
* Maintainable
* Scalable
* Type-safe
* Easy to understand

---

# 📁 Project Structure

```text
bpl-official/
│
├── public/
│   └── assets/
│       └── images/
│           └── logo/
│
├── src/
│   │
│   ├── app/
│   │   ├── layout.tsx
│   │   ├── page.tsx
│   │   ├── globals.scss
│   │   │
│   │   ├── teams/
│   │   │   └── page.tsx
│   │   │
│   │   ├── matches/
│   │   │   └── page.tsx
│   │   │
│   │   ├── auction/
│   │   │   └── page.tsx
│   │   │
│   │   ├── points-table/
│   │   │   └── page.tsx
│   │   │
│   │   ├── gallery/
│   │   │   └── page.tsx
│   │   │
│   │   ├── admin/
│   │   │   └── page.tsx
│   │   │
│   │   ├── loading.tsx
│   │   ├── error.tsx
│   │   └── not-found.tsx
│   │
│   ├── features/
│   │   │
│   │   ├── home/
│   │   │   ├── index.home.tsx
│   │   │   └── components/
│   │   │       ├── Hero.tsx
│   │   │       ├── LiveMatch.tsx
│   │   │       ├── UpcomingMatches.tsx
│   │   │       ├── PointsTablePreview.tsx
│   │   │       └── Sponsors.tsx
│   │   │
│   │   ├── teams/
│   │   │   ├── index.teams.tsx
│   │   │   └── components/
│   │   │       ├── TeamCard.tsx
│   │   │       ├── TeamGrid.tsx
│   │   │       └── TeamDetails.tsx
│   │   │
│   │   ├── matches/
│   │   │   ├── index.matches.tsx
│   │   │   └── components/
│   │   │       ├── MatchCard.tsx
│   │   │       ├── MatchList.tsx
│   │   │       └── LiveScore.tsx
│   │   │
│   │   ├── auction/
│   │   │   ├── index.auction.tsx
│   │   │   └── components/
│   │   │       ├── AuctionCard.tsx
│   │   │       ├── BidPanel.tsx
│   │   │       └── PurseTracker.tsx
│   │   │
│   │   ├── points-table/
│   │   │   ├── index.points-table.tsx
│   │   │   └── components/
│   │   │       └── PointsTable.tsx
│   │   │
│   │   ├── gallery/
│   │   │   ├── index.gallery.tsx
│   │   │   └── components/
│   │   │       └── GalleryGrid.tsx
│   │   │
│   │   └── admin/
│   │       ├── index.admin.tsx
│   │       └── components/
│   │           ├── Dashboard.tsx
│   │           ├── MatchManager.tsx
│   │           ├── TeamManager.tsx
│   │           └── AuctionManager.tsx
│   │
│   ├── components/
│   │   │
│   │   ├── layout/
│   │   │   ├── Navbar.tsx
│   │   │   ├── Footer.tsx
│   │   │   └── Sidebar.tsx
│   │   │
│   │   ├── common/
│   │   │   ├── EmptyState.tsx
│   │   │   ├── Loader.tsx
│   │   │   └── ErrorMessage.tsx
│   │   │
│   │   └── ui/
│   │       ├── Button.tsx
│   │       ├── Card.tsx
│   │       ├── Input.tsx
│   │       ├── Modal.tsx
│   │       ├── Table.tsx
│   │       └── Badge.tsx
│   │
│   ├── hooks/
│   │   ├── useSocket.ts
│   │   ├── useTheme.ts
│   │   ├── useDebounce.ts
│   │   └── useLocalStorage.ts
│   │
│   ├── services/
│   │   ├── api.ts
│   │   ├── team.service.ts
│   │   ├── player.service.ts
│   │   ├── match.service.ts
│   │   ├── auction.service.ts
│   │   ├── score.service.ts
│   │   └── auth.service.ts
│   │
│   ├── store/
│   │   ├── auth.store.ts
│   │   ├── match.store.ts
│   │   ├── team.store.ts
│   │   └── theme.store.ts
│   │
│   ├── lib/
│   │   ├── prisma.ts
│   │   ├── socket.ts
│   │   ├── auth.ts
│   │   └── validations.ts
│   │
│   ├── types/
│   │   ├── team.types.ts
│   │   ├── player.types.ts
│   │   ├── match.types.ts
│   │   ├── auction.types.ts
│   │   ├── score.types.ts
│   │   └── api.types.ts
│   │
│   ├── constants/
│   │   ├── routes.constants.ts
│   │   ├── theme.constants.ts
│   │   ├── api.constants.ts
│   │   └── app.constants.ts
│   │
│   ├── utils/
│   │   ├── formatDate.ts
│   │   ├── slugify.ts
│   │   ├── calculateNRR.ts
│   │   └── helpers.ts
│   │
│   └── styles/
│       ├── abstracts/
│       │   ├── _variables.scss
│       │   ├── _mixins.scss
│       │   └── _breakpoints.scss
│       │
│       ├── base/
│       │   ├── _reset.scss
│       │   ├── _typography.scss
│       │   └── _global.scss
│       │
│       ├── components/
│       │
│       └── features/
│           ├── home/
│           ├── teams/
│           ├── matches/
│           ├── auction/
│           ├── points-table/
│           ├── gallery/
│           └── admin/
│
├── .env.local
├── .gitignore
├── eslint.config.mjs
├── next.config.ts
├── package.json
├── package-lock.json
├── tsconfig.json
└── README.md
```

---

# 📂 Architecture Breakdown

## `app/`

The `app` directory contains the **Next.js App Router** structure.

```text
app/
├── layout.tsx
├── page.tsx
├── teams/
├── matches/
├── auction/
├── points-table/
├── gallery/
└── admin/
```

### Responsibilities

* Application routing
* Page entry points
* Root layout
* Global styles
* Loading UI
* Error handling
* 404 handling

### Routes

| Route           | Purpose            |
| --------------- | ------------------ |
| `/`             | Home page          |
| `/teams`        | Teams              |
| `/matches`      | Matches            |
| `/auction`      | Auction            |
| `/points-table` | Points table       |
| `/gallery`      | Tournament gallery |
| `/admin`        | Administration     |

---

# 🧩 Features

The `features` directory contains the application's primary business modules.

```text
features/
├── home/
├── teams/
├── matches/
├── auction/
├── points-table/
├── gallery/
└── admin/
```

Each feature contains its own entry component and feature-specific components.

This keeps business functionality isolated and makes it easier to extend the application.

---

# 🏠 Home Feature

```text
features/home/
│
├── index.home.tsx
│
└── components/
    ├── Hero.tsx
    ├── LiveMatch.tsx
    ├── UpcomingMatches.tsx
    ├── PointsTablePreview.tsx
    └── Sponsors.tsx
```

The home feature provides:

* Tournament hero section
* Live match information
* Upcoming matches
* Points table preview
* Sponsors section

---

# 👥 Teams Feature

```text
features/teams/
│
├── index.teams.tsx
│
└── components/
    ├── TeamCard.tsx
    ├── TeamGrid.tsx
    └── TeamDetails.tsx
```

Responsible for:

* Team listing
* Team cards
* Team grid
* Team details
* Team-related information

---

# 🏟️ Matches Feature

```text
features/matches/
│
├── index.matches.tsx
│
└── components/
    ├── MatchCard.tsx
    ├── MatchList.tsx
    └── LiveScore.tsx
```

Responsible for:

* Match listing
* Match cards
* Match information
* Live score display
* Match status

---

# 🔨 Auction Feature

```text
features/auction/
│
├── index.auction.tsx
│
└── components/
    ├── AuctionCard.tsx
    ├── BidPanel.tsx
    └── PurseTracker.tsx
```

Responsible for:

* Auction information
* Player auction cards
* Bidding interface
* Team purse tracking
* Auction management

---

# 📊 Points Table Feature

```text
features/points-table/
│
├── index.points-table.tsx
│
└── components/
    └── PointsTable.tsx
```

Responsible for displaying tournament standings such as:

* Team position
* Matches played
* Wins
* Losses
* Points
* Net Run Rate

---

# 🖼️ Gallery Feature

```text
features/gallery/
│
├── index.gallery.tsx
│
└── components/
    └── GalleryGrid.tsx
```

Responsible for:

* Tournament images
* Match images
* Team images
* Gallery grid
* Responsive image presentation

---

# 🛠️ Admin Feature

```text
features/admin/
│
├── index.admin.tsx
│
└── components/
    ├── Dashboard.tsx
    ├── MatchManager.tsx
    ├── TeamManager.tsx
    └── AuctionManager.tsx
```

The admin module provides a structure for managing:

* Tournament dashboard
* Teams
* Matches
* Auctions
* Tournament information

---

# 🧱 Shared Components

The `components` directory contains reusable components used throughout the application.

```text
components/
│
├── layout/
├── common/
└── ui/
```

## Layout Components

```text
Navbar.tsx
Footer.tsx
Sidebar.tsx
```

Used for application-wide layout and navigation.

## Common Components

```text
EmptyState.tsx
Loader.tsx
ErrorMessage.tsx
```

Used for common application states.

## UI Components

```text
Button.tsx
Card.tsx
Input.tsx
Modal.tsx
Table.tsx
Badge.tsx
```

Reusable UI building blocks used across multiple features.

---

# 🪝 Custom Hooks

The `hooks` directory contains reusable React hooks.

```text
hooks/
├── useSocket.ts
├── useTheme.ts
├── useDebounce.ts
└── useLocalStorage.ts
```

### `useSocket.ts`

Handles Socket.IO-related client behavior.

### `useTheme.ts`

Manages theme-related functionality.

### `useDebounce.ts`

Provides debouncing functionality for operations such as search.

### `useLocalStorage.ts`

Provides a reusable interface for browser local storage.

---

# 🌐 Services

The `services` directory handles communication with external APIs and application services.

```text
services/
├── api.ts
├── team.service.ts
├── player.service.ts
├── match.service.ts
├── auction.service.ts
├── score.service.ts
└── auth.service.ts
```

### Responsibilities

* API requests
* Team operations
* Player operations
* Match operations
* Auction operations
* Score operations
* Authentication operations

Keeping these operations outside UI components improves maintainability.

---

# 🧠 Store

The `store` directory contains application-level state.

```text
store/
├── auth.store.ts
├── match.store.ts
├── team.store.ts
└── theme.store.ts
```

### State Areas

* Authentication
* Match state
* Team state
* Theme state

The store should contain **client-side application state**, while server/API data can be handled through the project's API layer and RTK Query where applicable.

---

# 🔧 Lib

The `lib` directory contains core integrations and shared application logic.

```text
lib/
├── prisma.ts
├── socket.ts
├── auth.ts
└── validations.ts
```

### Includes

* Prisma configuration
* Socket configuration
* Authentication utilities
* Validation logic

---

# 📘 TypeScript Types

The `types` directory contains reusable TypeScript definitions.

```text
types/
├── team.types.ts
├── player.types.ts
├── match.types.ts
├── auction.types.ts
├── score.types.ts
└── api.types.ts
```

This provides a centralized location for domain-specific types.

---

# 📌 Constants

The `constants` directory contains application-wide constant values.

```text
constants/
├── routes.constants.ts
├── theme.constants.ts
├── api.constants.ts
└── app.constants.ts
```

### Examples

* Application routes
* API configuration
* Theme configuration
* Application-level constants

---

# 🛠️ Utilities

The `utils` directory contains reusable helper functions.

```text
utils/
├── formatDate.ts
├── slugify.ts
├── calculateNRR.ts
└── helpers.ts
```

### Examples

* Date formatting
* Slug generation
* Net Run Rate calculation
* General helper functions

---

# 🎨 SCSS Architecture

The project uses **Sass/SCSS** with a structured styling system.

```text
styles/
│
├── abstracts/
│   ├── _variables.scss
│   ├── _mixins.scss
│   └── _breakpoints.scss
│
├── base/
│   ├── _reset.scss
│   ├── _typography.scss
│   └── _global.scss
│
├── components/
│
└── features/
    ├── home/
    ├── teams/
    ├── matches/
    ├── auction/
    ├── points-table/
    ├── gallery/
    └── admin/
```

## Abstracts

Contains reusable SCSS resources:

* Variables
* Mixins
* Breakpoints

## Base

Contains foundational styles:

* CSS reset
* Typography
* Global styles

## Components

Contains styles for shared UI components.

## Features

Contains feature-specific styles.

---

# 🔄 Application Data Flow

The application follows a layered architecture:

```text
                    ┌─────────────────┐
                    │   Next.js App   │
                    │     Router      │
                    └────────┬────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │    Features     │
                    │ Home / Teams /  │
                    │ Matches / etc.  │
                    └────────┬────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │   Components    │
                    └────────┬────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │ Custom Hooks    │
                    └────────┬────────┘
                             │
                   ┌─────────┴─────────┐
                   ▼                   ▼
             ┌───────────┐       ┌───────────┐
             │  Store    │       │ Services  │
             └─────┬─────┘       └─────┬─────┘
                   │                   │
                   └─────────┬─────────┘
                             ▼
                    ┌─────────────────┐
                    │ API / External  │
                    │    Services     │
                    └─────────────────┘
```

---

# 🔄 Feature Development Pattern

A typical feature can follow this pattern:

```text
Route
  ↓
Feature Entry
  ↓
Feature Components
  ↓
Custom Hooks
  ↓
Store / Service
  ↓
API
  ↓
Data
```

This separation helps prevent business logic from becoming tightly coupled to UI components.

---

# 📱 Responsive Design

The application is designed for:

```text
📱 Mobile
   ↓
📱 Tablet
   ↓
💻 Laptop
   ↓
🖥️ Desktop
```

Responsive considerations include:

* Navigation
* Cards
* Tables
* Match information
* Team sections
* Auction panels
* Gallery
* Forms
* Typography
* Spacing

---

# 🎬 Animations

**Framer Motion** is used for interactive animations and transitions.

Possible application areas include:

* Page transitions
* Card animations
* Modal transitions
* Navigation
* Auction interactions
* Loading states
* Interactive UI elements

---

# 📝 Forms & Validation

The project includes multiple form libraries and validation tools.

### Formik

Used for structured form management.

### React Hook Form

Used for performant form handling.

### Yup

Used for schema-based validation.

### Zod

Used for TypeScript-friendly runtime validation.

---

# 🔔 Notifications

## Sonner

Used for toast-style notifications.

Typical use cases:

```text
Success
Error
Warning
Information
```

## SweetAlert2

Used for:

```text
Confirmation dialogs
Delete confirmations
Important actions
Payment confirmations
Error dialogs
```

---

# 🔌 Real-Time Communication

The application includes **Socket.IO** for real-time functionality.

Potential use cases include:

* Live scores
* Live match status
* Auction updates
* Real-time notifications
* Match events

Relevant files:

```text
hooks/useSocket.ts
lib/socket.ts
services/score.service.ts
```

---

# 🖼️ Image Optimization

The application uses Next.js image handling with **Sharp**.

Project assets are organized under:

```text
public/assets/images/
```

Example:

```text
public/
└── assets/
    └── images/
        └── logo/
```

---

# ⚙️ Installation

## Prerequisites

Install the following:

* Node.js
* npm
* Git

Verify installation:

```bash
node -v
npm -v
git --version
```

---

# 📥 Clone the Repository

```bash
git clone https://github.com/amolpawar24/BPL-Official.git
```

Navigate into the project:

```bash
cd BPL-Official
```

---

# 📦 Install Dependencies

```bash
npm install
```

---

# 🔐 Environment Configuration

Create a local environment file:

```text
.env.local
```

Example:

```env
NEXT_PUBLIC_API_URL=your_api_url
NEXT_PUBLIC_SOCKET_URL=your_socket_url
```

Add any required project-specific environment variables to this file.

> Never commit private credentials, API keys, database credentials, or secrets to GitHub.

---

# ▶️ Run the Development Server

```bash
npm run dev
```

Then open:

```text
http://localhost:3000
```

---

# 🏗️ Production Build

Create a production build:

```bash
npm run build
```

Run the production server:

```bash
npm run start
```

---

# 🔍 Linting

Run ESLint:

```bash
npm run lint
```

---

# 📜 Available Scripts

| Command         | Description                           |
| --------------- | ------------------------------------- |
| `npm run dev`   | Starts the Next.js development server |
| `npm run build` | Creates the production build          |
| `npm run start` | Starts the production server          |
| `npm run lint`  | Runs ESLint                           |

---

# 📦 Dependencies

The project uses the following major packages:

```text
Next.js
React
React DOM
TypeScript
Redux Toolkit
React Redux
Formik
React Hook Form
Framer Motion
React Icons
Sass
Sharp
Socket.IO
Sonner
SweetAlert2
Yup
Zod
```

---

# 🚀 Deployment

The application is deployed using **Vercel**.

### Deployment Flow

```text
Local Development
       │
       ▼
      Git
       │
       ▼
    GitHub
       │
       ▼
    Vercel
       │
       ▼
  Production
```

Before deployment:

```bash
npm run lint
npm run build
```

Make sure all production environment variables are configured in the deployment platform.

---

# 🔐 Security Considerations

The application should follow basic security practices:

* Do not expose private API keys
* Do not commit `.env.local`
* Validate user input
* Validate API responses
* Protect admin functionality
* Use secure authentication
* Validate payment requests on the server
* Never trust client-side payment status
* Sanitize user-generated content where required

---

# ⚡ Performance Considerations

The project uses modern Next.js and frontend practices to improve performance.

Key areas include:

* Next.js App Router
* Image optimization
* Component reuse
* API caching
* Efficient state management
* Lazy loading where appropriate
* Optimized assets
* Responsive rendering
* Minimal unnecessary re-renders

---

# 🧪 Testing Strategy

Testing can be introduced across multiple levels:

```text
Unit Tests
     ↓
Component Tests
     ↓
Integration Tests
     ↓
API Tests
     ↓
End-to-End Tests
```

Important areas to test include:

* Utility functions
* Components
* Forms
* Validation
* Store logic
* API services
* Match functionality
* Auction functionality
* Authentication
* Payment workflows

---

# 🧱 Development Principles

## ♻️ Reusability

Create reusable components instead of duplicating UI code.

## 🧩 Modularity

Keep feature-specific functionality inside its respective feature module.

## 📘 Type Safety

Use TypeScript for components, API data, state, and domain models.

## 🎯 Separation of Concerns

Keep:

```text
UI
Logic
Services
State
Types
Utilities
Styles
```

properly separated.

## 📈 Scalability

The architecture allows new modules to be added without restructuring the entire application.

---

# 🔨 Feature Development Workflow

A typical feature development process:

```text
1. Define feature requirements
          ↓
2. Create TypeScript types
          ↓
3. Create service/API layer
          ↓
4. Add state management if required
          ↓
5. Create custom hooks
          ↓
6. Build feature components
          ↓
7. Add SCSS styles
          ↓
8. Integrate with Next.js route
          ↓
9. Test functionality
          ↓
10. Run lint
          ↓
11. Run production build
          ↓
12. Commit and push changes
```

---

# 🌿 Git Workflow

Create a feature branch:

```bash
git checkout -b feature/player-module
```

Check changes:

```bash
git status
```

Stage changes:

```bash
git add .
```

Commit changes:

```bash
git commit -m "Add player module"
```

Push the branch:

```bash
git push -u origin feature/player-module
```

---

# 🔮 Future Scope

Potential future improvements include:

* 🔐 Complete authentication system
* 👤 User profiles
* 🛡️ Role-based access control
* 🏏 Advanced team management
* 🧑‍💼 Player management
* 🔴 Live score updates
* 🔨 Advanced auction system
* 💰 Payment integration
* 📊 Advanced player statistics
* 🏆 Tournament management
* 🔔 Real-time notifications
* 💬 Live match commentary
* 📰 Tournament news
* 📸 Advanced media gallery
* 📈 Tournament analytics
* 🛠️ Complete admin dashboard
* 📱 Progressive Web App support

---

# 📊 Project Status

| Feature            | Status |
| ------------------ | ------ |
| Next.js Setup      | ✅      |
| React Setup        | ✅      |
| TypeScript         | ✅      |
| SCSS Architecture  | ✅      |
| Responsive UI      | ✅      |
| Home Page          | ✅      |
| Teams              | 🚧     |
| Matches            | 🚧     |
| Auction            | 🚧     |
| Points Table       | 🚧     |
| Gallery            | 🚧     |
| Admin Dashboard    | 🚧     |
| Real-Time Features | 🚧     |
| Authentication     | 🚧     |
| Payment System     | 🚧     |

> Project status may change as development continues.

---

# 📌 Project Information

| Category         | Details              |
| ---------------- | -------------------- |
| Project          | BPL Official         |
| Framework        | Next.js              |
| UI Library       | React                |
| Language         | TypeScript           |
| Styling          | SCSS                 |
| State Management | Redux Toolkit        |
| API Data         | RTK Query / Services |
| Real-Time        | Socket.IO            |
| Animations       | Framer Motion        |
| Deployment       | Vercel               |

---

# 🤝 Contributing

This repository is primarily maintained as a project repository.

For development changes:

```text
Create Branch
     ↓
Implement Feature
     ↓
Test
     ↓
Run Lint
     ↓
Run Build
     ↓
Commit
     ↓
Push
```

---

# 📄 License

This project currently does not include an open-source license.

---

# 🏏 BPL Official

**A modern cricket tournament platform built with Next.js, React, TypeScript, Redux Toolkit, SCSS, and scalable frontend architecture.**

**Built to manage and present the BPL experience through teams, matches, auctions, scores, standings, galleries, and administration.**
