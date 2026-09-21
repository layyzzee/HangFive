# Hang8

A responsive, browser-based Hangman game built with React and Vite. This application was developed as a front-end portfolio project to demonstrate clean component architecture, deterministic state management, and optimized asset bundling.

## Live Demo

The application is deployed and available to play directly in the browser:
[Hang8 Live Deployment](https://github.io)

## Project Overview

Hang8 translates the traditional mechanics of the Hangman word-guessing game into a reactive web application. The core objective of the project was to build a self-contained front-end application that handles real-time user input, tracks application state transitions safely, and provides a seamless user experience across mobile, tablet, and desktop viewports.

## Core Features

- **Interactive Input Matrix:** Features a dynamic on-screen keyboard that maps layout states directly to user selections while preventing duplicate inputs.
- **Deterministic Win/Loss Evaluation:** Continuous validation routines automatically intercept game states to determine victory or defeat conditions.
- **Conditional Interface Lifecycle:** Seamlessly transitions between active gameplay, success states, and failure states without causing full browser reloads.
- **Responsive Layout Design:** Built with modern CSS layout modules to guarantee structural fluidness on any screen size.
- **Automated Deployment Pipeline:** Integrated with GitHub Actions workflows to automate production compilation and hosting via GitHub Pages.

## Technical Stack

- **Framework:** React (Functional Architecture and Hooks)
- **Build Tooling:** Vite
- **Programming Language:** JavaScript (ES6+)
- **Styling Methodology:** Custom CSS (Flexbox, Grid, and Media Queries)
- **CI/CD and Hosting:** GitHub Actions and GitHub Pages

## Engineering Competencies Demonstrated

### Component Architecture
The application is structured into decoupled, single-responsibility React components. This modularity ensures high readability, enforces a unidirectional data flow, and simplifies testing or scaling individual UI layers.

### State Synchronization
Leverages React state hooks to coordinate asynchronous mutations across separate game elements. A single letter guess simultaneously triggers updates to the hidden word array, disables matching keys in the input grid, and updates the structural countdown of the gallows graphics.

### Application Performance and Optimization
Utilizes Vite's lightning-fast bundling engine to compile production assets. The final build utilizes aggressive code minification and asset tree-shaking, resulting in minimal load times and optimal Core Web Vitals.

## Local Development and Installation

To inspect, run, or extend this project locally, ensure you have Node.js installed on your machine, then complete the following steps:

1. Clone the repository to your local environment:
   ```bash
   git clone https://github.com
   cd Hang8
   ```

2. Install the necessary project dependencies:
   ```bash
   npm install
   ```

3. Launch the local development server:
   ```bash
   npm run dev
   ```
   Open the local host URL provided in your terminal output (typically `http://localhost:5173`) to view the application.

### Compilation for Production

To generate an optimized, production-ready build distribution:
```bash
npm run build
```
The compiled, production-ready static assets will be output to the `/dist` directory.

## Architectural Key Takeaways

Developing Hang8 provided deep practical experience in managing structural UI states and handling domestic event loops in client-side applications. Key learnings involved refining patterns around lifting state up to mutual parent components, maintaining immutable state update patterns, and properly structuring project configuration utilities like ESLint and Vite plugins.
