# Apple Replica Website

This project is a replica of the Apple website, built using React and Tailwind CSS. It features a dynamic and interactive user interface that showcases various Apple products, particularly the iPhone 15 Pro. The project includes components for navigation, hero sections, highlights, and a video carousel, all designed to provide a seamless and engaging user experience.

## Demo
![WebsiteDemo](ScreenRecording.gif)

# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Features

- **Responsive Design**: Utilizes Tailwind CSS to ensure the website is fully responsive and looks great on all devices.
- **Dynamic Video Carousel**: A GSAP-powered video carousel that plays highlight videos of the iPhone 15 Pro, complete with progress indicators and playback controls.
- **Interactive Hero Section**: Features a hero section with a video background that adapts based on screen size, and includes smooth animations for text and call-to-action buttons.
- **Navigation Bar**: A sleek and minimalistic navigation bar that includes links to various sections of the website and icons for search and shopping bag.
- **Highlights Section**: Displays key features and highlights of the iPhone 15 Pro with smooth animations and links to watch related videos.

## Installation
Install dependencies:

```sh
npm install
```

## Usage

1. Start the development server:
    ```sh
    npm run dev
    ```
2. Open your browser and navigate to `http://localhost:5173/` to view the website.

## Code Overview

### VideoCarousel Component

The `VideoCarousel` component is designed to provide a seamless video playback experience within a carousel interface. Key features include:

- **Video Playback Control**: The component can play and pause videos based on user interactions and application state.
- **Progress Bar Animation**: Utilizes GSAP to animate a progress bar that reflects the current playback position of the video.
- **State Management**: Manages video playback state, including handling when videos end and transitioning to the next video in the carousel.

### ModelView Component
The `ModelView` component integrates 3D models into the website using `three.js` and `@react-three/fiber`. Key features include:

- **3D Model Rendering**: Renders interactive 3D models of Apple products.
- **Lighting and Shadows**: Utilizes `three.js` lighting to create realistic shadows and highlights.
- **Loader Component**: Displays a loading indicator while 3D models are being loaded.

### Lights Component
The `Lights` component sets up the lighting for the 3D scene. Key features include:

- **Ambient Light**: Provides overall illumination to the scene.
- **Directional Light**: Simulates sunlight, casting shadows and highlights on the 3D models.