# NLW Agents - Frontend

Frontend application for NLW Agents, developed during a Rocketseat event. This React application provides an interface for creating rooms, managing questions, and recording audio interactions.

## 🚀 Tech Stack

### Core Technologies

- **React 19** - Modern React with latest features
- **TypeScript** - Type-safe JavaScript development
- **Vite** - Fast build tool and development server
- **TailwindCSS v4** - Utility-first CSS framework

### State Management & Data Fetching

- **TanStack Query** - Server state management and data fetching
- **React Hook Form** - Performant form library with validation
- **Zod** - Runtime schema validation

### UI Components & Styling

- **Radix UI** - Unstyled, accessible UI primitives
- **Shadcn/ui** - Re-usable component library
- **Class Variance Authority (CVA)** - Component variant styling
- **Lucide React** - Beautiful icon library
- **Tailwind Merge** - Utility for merging Tailwind classes

### Routing & Navigation

- **React Router DOM v7** - Client-side routing

### Utilities

- **Day.js** - Date manipulation library
- **Biome** - Fast linter and formatter

## 🏗️ Architecture & Design Patterns

### Project Structure

```
src/
├── components/          # Reusable UI components
│   ├── ui/             # Base UI components (buttons, inputs, etc.)
│   └── *.tsx           # Feature-specific components
├── pages/              # Route components
├── http/               # API layer
│   ├── types/          # API response/request types
│   └── use-*.ts        # Custom hooks for data fetching
├── lib/                # Utility functions
└── main.tsx            # Application entry point
```

### Design Patterns

1. **Custom Hooks Pattern**: API calls encapsulated in custom hooks using TanStack Query
2. **Component Composition**: Using Radix UI primitives for accessible, unstyled components
3. **Variant-based Styling**: CVA for creating component variants with consistent styling
4. **Type-first Development**: Full TypeScript coverage with proper API typing
5. **Form Validation**: React Hook Form with Zod schemas for robust form handling

## 🛠️ Setup & Installation

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn package manager

### Installation

1. **Clone the repository**

   ```bash
   git clone <repository-url>
   cd nlw-agents-web
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Configure environment**

   - Ensure the backend API is running on `http://localhost:3333`
   - Update API URLs in the HTTP hooks if using a different backend URL

4. **Start development server**

   ```bash
   npm run dev
   ```

5. **Access the application**
   - Open your browser to `http://localhost:5173`

### Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run Biome linter

## 🎨 UI Components

The project uses a custom component library built on top of Radix UI and styled with TailwindCSS. Components are located in `src/components/ui/` and follow the Shadcn/ui pattern.

### Key Features

- **Accessible by default** - Built on Radix UI primitives
- **Customizable variants** - Using CVA for consistent styling
- **TypeScript support** - Full type safety for all components
- **Modern styling** - TailwindCSS v4 with CSS variables

## 🔧 Configuration

### TailwindCSS

- Configuration: `components.json` and Vite config
- Base color: Zinc
- CSS variables enabled for theming

### Path Aliases

- `@/*` - Points to `src/*` directory
- Configured in `vite.config.ts` and `tsconfig.json`

### Component Library

- Style: New York (Shadcn/ui)
- Icon library: Lucide React
- Base components: Radix UI primitives

## 🌐 API Integration

The application communicates with a backend API running on `localhost:3333`. API calls are managed through custom hooks in the `src/http/` directory using TanStack Query for:

- Caching and background updates
- Loading and error states
- Request deduplication
- Optimistic updates

## 🎯 Key Features

- **Room Management** - Create and list rooms
- **Question System** - Submit and manage questions within rooms
- **Audio Recording** - Record audio interactions in rooms
- **Real-time Updates** - Automatic data synchronization
- **Responsive Design** - Mobile-friendly interface

---

_This project was developed during a Rocketseat NLW (Next Level Week) event, showcasing modern React development practices and patterns._
