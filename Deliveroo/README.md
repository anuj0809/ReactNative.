<div align="center">

  <img src="https://user-images.githubusercontent.com/99184393/196014260-dfc68631-1abb-4635-ac6d-787ad0805dcd.png" alt="logo" width="200" height="auto" />
  
  # Deliveroo Clone with REACT NATIVE!
  
  <p>
Deliveroo Clone with REACT NATIVE! (Navigation, Redux, Tailwind CSS & Sanity.io)
  </p>
  
<!-- Table of Contents -->

## :notebook_with_decorative_cover: Table of Contents

- [About the Project](#star2-about-the-project)
  - [Screenshots](#camera-screenshots)
  - [Tech Stack](#space_invader-tech-stack)
- [Getting Started](#toolbox-getting-started)
  - [Prerequisites](#bangbang-prerequisites)
  - [Installation](#gear-installation)
  - [Run Locally](#running-run-locally)
  - [Deployment](#triangular_flag_on_post-deployment)
- [Contact](#handshake-contact)

<!-- About the Project -->

### :space_invader: Tech Stack

<details>
  <summary>Client</summary>
  <ul>
    <li><a href="https://#/">Javascript</a></li>
    <li><a href="https://docs.expo.dev/workflow/expo-cli">Expo</a></li>
    <li><a href="https://reactnative.dev">React Native</a></li>
     <li><a href="https://tailwindcss.com/">TailwindCSS</a></li>
  </ul>
</details>

<details>
<summary>Database</summary>
  <ul>
    <li><a href="https://www.sanity.io">Sanity</a></li>
  </ul>
</details>

## :toolbox: Getting Started

### :bangbang: Prerequisites

- Sign up for a Sanity account <a href='https://www.sanity.io'>HERE</a>
- Install Node JS in your computer <a href='https://nodejs.org/en/'>HERE</a>

### :gear: Installation

Install my-project with expo

Installing Expo CLI

```
npm install --global expo-cli
```

Initializing the project

```
npx create-expo-app deliveroo-clone
```

```
cd deliveroo-clone
```

Install dependencies

### Setup Tailwind CSS

```
npm install tailwindcss-react-native
npm install --save-dev tailwindcss
```

Tailwindcss requires a `tailwind.config.js` file with the content section configured to include the paths to all of your components and any other source files that contain Tailwind class names.

```
// tailwind.config.js
module.exports = {
  content: [
    "./screens/**/*.{js,ts,jsx,tsx}",
    "./pages/**/*.{js,ts,jsx,tsx}",
    "./components/**/*.{js,ts,jsx,tsx}",
  ],
  // ...
};
```

Add `TailwindProvider` at the top level of your application. The `TailwindProvider` creates the context for reactive styles and the atomic style objects.

```
import { TailwindProvider } from "tailwindcss-react-native";

function MyAppsProviders({ children }) {
  return <TailwindProvider>{children}</TailwindProvider>;
}
```

##### Configure your babel.config.js

```
// babel.config.js
module.exports = {
  plugins: ["tailwindcss-react-native/babel"],
};
```

Install dependencies

<!-- Run Locally -->

### :running: Run Locally

Clone the project

```bash
  git clone
```

change directory

```bash
  cd Deliveroo-Clone
```

Install dependencies

```bash
  npx expo install
```

Start the server

```bash
  npx expo start
```

<hr />

### Creating a Build

- Optimize the assets for speed - `npx expo-optimize` (formerly expo optimize)
- Bundle the project for production - `npx expo export:web` (`expo build:web` in the legacy Expo CLI).
- Creates a production ready static bundle in the `web-build/` directory. Don't edit this folder directly.
- If you make any changes to your project, you'll need to re-build for production.
- For more help use `npx expo export:web --help`
- <a href="https://docs.expo.dev/eas" target="_blank">More Info</a>

<!-- Deployment -->

### :triangular_flag_on_post: Deployment

To deploy this project run

#### Expo Publish

publish your project

```
expo publish
```
