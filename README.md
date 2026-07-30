# ✈️ Travel Explorer App

A full-stack travel destination management web application built using **React 19**, **Vite**, **Redux Toolkit**, **React Router DOM v7**, and **JSON Server**.

Travel Explorer allows users to discover destinations, search and filter places by category and budget, manage their favorite destinations, and perform full CRUD (Create, Read, Update, Delete) operations.

---

## 🔗 Live Demo & Links

- 🌐 **Live Web Application (Vercel)**: [https://travel-rose-kappa.vercel.app](https://travel-rose-kappa.vercel.app)
- 🐙 **GitHub Repository**: [https://github.com/Nivedreddy6/Travel-](https://github.com/Nivedreddy6/Travel-)
- ⚡ **Online REST API (My JSON Server)**: [https://my-json-server.typicode.com/Nivedreddy6/Travel-](https://my-json-server.typicode.com/Nivedreddy6/Travel-)

---

## ✨ Features

- **🔐 User Authentication & Protected Routes**: Full Register, Login, and Logout flow with session management via `localStorage` and client-side route protection.
- **🏖️ Destination Catalog & Filtering**: Explore destinations with interactive search by name, filtering by categories (*Beach*, *Hill Station*, *Historical*, *Heritage*), and budget levels (*Low*, *Medium*, *High*).
- **📌 Detailed Destination Views**: View comprehensive destination info including weather, currency, language, ratings, price, duration, best time to visit, and popular attractions.
- **➕ Complete CRUD Functionality**: Add new destinations, edit existing destination details, and remove destinations dynamically updated on the backend REST API.
- **❤️ Favorites System**: Global state management powered by Redux Toolkit with celebratory `canvas-confetti` animations when saving places.
- **🔄 Single Page Application (SPA) Routing**: Configured with `vercel.json` rewrites for smooth client-side routing and page refresh on Vercel deployments.
- **🔌 Hybrid API Architecture**: Automatic switching between local `json-server` (`http://localhost:3000`) for development and GitHub-backed My JSON Server for production.

---

## 🛠️ Tech Stack

- **Frontend**: [React 19](https://react.dev/), [Vite](https://vitejs.dev/)
- **State Management**: [Redux Toolkit](https://redux-toolkit.js.org/) (`@reduxjs/toolkit`, `react-redux`)
- **Routing**: [React Router DOM v7](https://reactrouter.com/)
- **HTTP Client**: [Axios](https://axios-http.com/)
- **Styling & UI Effects**: Vanilla CSS, [Lucide React Icons](https://lucide.dev/), `canvas-confetti`
- **Backend / Database**: `json-server` (watching `db.json`) & [My JSON Server](https://my-json-server.typicode.com/)
- **Deployment**: [Vercel](https://vercel.com/)

---

## 📂 Project Structure

```text
d:/travel/
├── db.json                     # JSON Database storing user and destination records
├── vercel.json                 # Vercel configuration for SPA route rewrites
├── package.json                # Project dependencies and scripts
└── src/
    ├── app/
    │   └── store.js            # Redux Store setup
    ├── components/
    │   ├── DestinationCard.jsx # Reusable destination card component
    │   └── Navbar.jsx          # Top navigation bar
    ├── features/
    │   └── favoriteSlice.js    # Redux slice for managing favorites
    ├── pages/
    │   ├── Home.jsx            # Landing page
    │   ├── Destinations.jsx    # Main destination catalog with filters
    │   ├── DestinationDetails.jsx # Detailed page for individual destination
    │   ├── AddDestination.jsx  # Form to add a new destination
    │   ├── EditDestination.jsx # Form to edit an existing destination
    │   ├── Favorites.jsx       # User's saved favorite destinations
    │   ├── Login.jsx           # User login page
    │   ├── Register.jsx        # User registration page
    │   └── Logout.jsx          # Logout handler
    ├── routes/
    │   ├── AppRoutes.jsx       # Client-side route declarations
    │   └── ProtectedRoute.jsx  # Route guard for authenticated actions
    └── services/
        └── api.js              # Axios instance configured for dev/prod environments
```

---

## 🚀 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) (v18 or higher recommended)
- `npm`

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Nivedreddy6/Travel-.git
   cd travel
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

### Running Locally

1. **Start the API Server**:
   ```bash
   npm run server
   ```
   *(Starts `json-server` on `http://127.0.0.1:3000` watching `db.json`)*

2. **Start the Frontend Dev Server**:
   ```bash
   npm run dev
   ```
   *(Starts Vite dev server on `http://localhost:5173/`)*

3. Open your browser and navigate to `http://localhost:5173`.

### Building for Production

```bash
npm run build
```

---

## 📜 License

This project is open source and available under the [MIT License](LICENSE).
