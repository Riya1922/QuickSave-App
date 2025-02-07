#QuickSave App
# React + Vite + TailwindCSS Template

This template provides a minimal setup for building a React application using Vite. It includes Hot Module Replacement (HMR) for fast refresh, Tailwind CSS for utility-first styling, and ESLint for code linting.

## Features
- **Vite**: Ultra-fast development and build tooling.
- **React**: Latest version for building modern UI components.
- **Tailwind CSS**: Utility-first CSS framework for building custom designs without leaving your HTML.
- **ESLint**: A pluggable linter tool for ensuring code quality.
- **Redux Toolkit**: State management with slices and reducers.
- **React Hot Toast**: For elegant notifications in your application.
- **React Router DOM**: Declarative routing for React.

---

## Installation

### Step 1: Create a Vite project

1. Install Vite globally (if not already installed):

   ```bash
   npm create vite@latest
   ```

2. When prompted, choose the following:
   - Project name: `paste`
   - Framework: `React`
   - Variant: `JavaScript` or `TypeScript` as per your preference.

3. Navigate into the project directory:

   ```bash
   cd paste
   ```

### Step 2: Install Tailwind CSS

To add Tailwind CSS to your Vite + React project, follow these steps:

1. Install Tailwind CSS and its dependencies:

   ```bash
   npm install -D tailwindcss postcss autoprefixer
   ```

2. Initialize Tailwind configuration:

   ```bash
   npx tailwindcss init
   ```

   This will create a `tailwind.config.js` file in your project.

3. Update the `tailwind.config.js` file with the following content to specify which files Tailwind should scan:

   ```js
   /** @type {import('tailwindcss').Config} */
   export default {
     content: [
       './index.html',
       './src/**/*.{js,ts,jsx,tsx}',
     ],
     theme: {
       extend: {},
     },
     plugins: [],
   }
   ```

4. Add the following lines to your `src/index.css` (or `src/main.css` if you’re using that):

   ```css
   @tailwind base;
   @tailwind components;
   @tailwind utilities;
   ```

### Step 3: Install Required Packages

Install the project dependencies:

```bash
npm install
```

### Step 4: Run the Project

Start the development server with the following command:

```bash
npm run dev
```

This command will launch the development server, and your project will be available at `http://localhost:5173`.

---

## Scripts

- **`npm run dev`**: Starts the Vite development server with HMR.
- **`npm run build`**: Builds the project for production.
- **`npm run preview`**: Serves the production build for preview.
- **`npm run lint`**: Lints your code using ESLint.

---

## Project Structure

Here is the basic structure of the project:

```
paste/
│
├── node_modules/
├── public/
├── src/
│   ├── assets/
│   ├── components/
│   ├── pages/
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
│
├── .eslintrc.js
├── tailwind.config.js
├── postcss.config.js
├── vite.config.js
└── package.json
```

---

## Tailwind CSS Configuration

The `tailwind.config.js` file is configured to scan all the files in the `src` directory for Tailwind CSS classes and allows you to customize the theme and plugins.

```js
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    './index.html',
    './src/**/*.{js,ts,jsx,tsx}',
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

---

