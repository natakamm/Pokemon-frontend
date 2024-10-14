The frontend of the Pokemon game is a React application that allows players to select a Pokémon from a list of Pokémon fetched from the PokeAPI. The Pokémon are divided by type, and each type has a unique color scheme to match the Pokémon's characteristics. The battle mechanics are based on the selected Pokémon's attributes like HP, Attack, and Defense, making the outcome of each fight determined by the strength of the Pokémon.

Players also enjoy the immersive experience of Pokémon cries, which play when a Pokémon is selected or during battles. The user is prompted to enter a unique username when playing the game, which gets displayed on the leaderboard after a match. Although there is no real login functionality, the username is used to track the player's performance (wins and losses).

# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

### Install Vite

`npm create vite@latest new-react-app -- --template react`

### Navigate into your project directory:

`cd new-react-app`

### Install Dependencies

`npm install`

### Install and Configure Tailwind CSS

Next, we will install Tailwind CSS

### Install Tailwind CSS

`npm install -D tailwindcss postcss autoprefixer`

### Initialize Tailwind CSS

`npx tailwindcss init -p`

### Configure Tailwind

### In the tailwind.config.js file, replace the content with the following:

```/** @type {import('tailwindcss').Config} */
export default {
content: ['./index.html', './src/**/\*.{js,ts,jsx,tsx}'],
theme: {
extend: {}
},
plugins: []
};
```

### Add Tailwind Directives

Open the index.css file located in the src folder, and replace its content with the Tailwind CSS directives:

@tailwind base;
@tailwind components;
@tailwind utilities;

### Install Daisy UI

`npm i -D daisyui`

### Configure Daisy UI

In your tailwind.config.js file, add daisyui to the plugins array:

```/** @type {import('tailwindcss').Config} */
import daisyui from "daisyui"
export default {
content: ['./index.html', './src/**/\*.{js,ts,jsx,tsx}'],
theme: {
extend: {}
},
plugins: [daisyui]
};
```

Check out the various UI components from [Daisy](https://daisyui.com/components/) here.
