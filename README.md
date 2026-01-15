# Web Movies 🎬 (React + Vite)

Web Movies is a simple React app built with **Vite** that shows **popular movies** using the **TMDb (The Movie Database) API**.  
Movies are displayed as cards, and the app uses **React Router** for navigation.

> This project is mainly for practicing React fundamentals: **components, props, state, useEffect, routing, and (optional) Context for favorites**.

---

## ✨ Features

- ✅ Fetch & display **Popular Movies** from TMDb
- ✅ Movie cards with **poster, title, release year**
- ✅ Navigation with **React Router**
  - `/` → Home
  - `/favorites` → Favorites page
- ✅ Clean component-based UI (props + reusable components)
- 🚧 Search feature (UI exists, you can wire it to API)
- 🚧 Favorites feature (button/UI exists, you can complete with Context + LocalStorage)

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
