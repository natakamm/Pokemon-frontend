#Pokémon Game
The frontend of the Pokémon game is a React application created using Vite. It utilizes React Router for navigation between different pages, providing a seamless user experience.

### Features
#### Homepage:

- Displays a list of available Pokémon retrieved from the PokeAPI.
- Each Pokémon is clickable and leads to the Pokémon Details Page.

#### Pokémon Details Page:

- Shows detailed information about the selected Pokémon, including stats, types, and abilities.
- Includes a button to add the Pokémon to the user’s roster.

#### Battle Page:

- Allows users to engage in battles with random Pokémon.
- Battle dynamics are based on Pokémon stats and types, incorporating type advantages/disadvantages, where the higher stat wins the round.
- Tracks the user’s wins and losses, assigning points or experience (XP) for each win.

#### Leaderboard Page:

- Displays a leaderboard with the top players based on their scores.
- Users can enter their name, and their score is persisted in the database after a battle.
- Includes appropriate handling of form input and validation.

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
