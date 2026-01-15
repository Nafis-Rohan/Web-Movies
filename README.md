# Web Movies 🎬 (React + Vite)

Web Movies is a simple React app built with **Vite** that shows **popular movies** using the **TMDb (The Movie Database) API**.  
Movies are displayed as cards, and the app uses **React Router** for navigation.

> This project is mainly for practicing React fundamentals: **components, props, state, useEffect, routing, and (optional) Context for favorites**.

---

## ✨ Features

- **Popular movies list:** The Home page fetches a list of popular movies from the TMDb API using the `getPopularMovies` function:contentReference[oaicite:0]{index=0} and displays them as cards.
- **Search movies:** The search form on the Home page is fully functional; when you type a query and submit, it calls `searchMovies(searchQuery)` to fetch matching results and updates the movie list:contentReference[oaicite:1]{index=1}.
- **Add/remove favourites:** Each movie card includes a heart button. Clicking the button toggles the favourite state using context functions `addToFavorites` and `removeFromFavorites`:contentReference[oaicite:2]{index=2}. The button highlights for favourites.
- **Favourites persistence:** Favourites are stored in localStorage. The `MovieContext` loads favourites on mount and writes any changes back to localStorage:contentReference[oaicite:3]{index=3}.
- **View favourites:** The `/favorites` route displays a grid of your favourite movies. If there are no favourites, it shows a friendly message:contentReference[oaicite:4]{index=4}.
- **Client‑side routing:** Uses React Router to navigate between Home and Favourites pages:contentReference[oaicite:5]{index=5}.
- **Environment‑based API key:** The API key is read from `import.meta.env.VITE_TMDB_API_KEY` in `src/services/api.js`:contentReference[oaicite:6]{index=6}.
- **Persisted context:** The `MovieProvider` wraps the whole app in `App.jsx`, making the favourites state accessible across components:contentReference[oaicite:7]{index=7}.

---

## 🧰 Tech Stack

- **React** (Vite)
- **React Router DOM**
- **TMDb API**
- CSS (custom)

---

## 🚀 Getting Started

### 1) Clone the repository

```bash
git clone https://github.com/Nafis-Rohan/Web-Movies.git
cd Web-Movies
```

### 2) Install dependencies

```bash
npm install
```

### 3) Create .env (project root)

Create a file named .env beside package.json and add: 'VITE_TMDB_API_KEY=YOUR_TMDB_API_KEY'

### 4) Run the project

```bash
npm run dev
```

## 🔐 Protect Your API Key (Important)

Add this to your `.gitignore` so your key never goes to GitHub:

```gitignore
.env
.env.*
```
