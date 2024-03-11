# Full-Stack 3D Website Development

Welcome to my repository for developing full-stack 3D websites! This repository aims to provide resources, tools, and guidelines for building immersive and interactive web experiences using 3D technologies.

## Table of Contents
1. [Introduction](#introduction)
2. [Technologies Used](#technologies-used)
3. [Getting Started](#getting-started)
4. [Contributing](#contributing)
5. [License](#license)

## Introduction

In today's web development landscape, there's a growing demand for immersive and interactive experiences. Incorporating 3D elements into web design allows developers to create visually stunning and engaging websites. This repository serves as a starting point for developers interested in diving into full-stack 3D website development.

## Getting Started

To begin with, follow these steps:

1. **Create Folder**: Set up a new folder for your project.

2. **Terminal Setup**: Open the terminal in Visual Studio Code and navigate to the newly created folder.

3. **Project Initialization**: Start the project by using:
    ```
    npm create vite@latest ./ -- --template react
    ```

4. **Tailwind CSS Installation**: Install Tailwind CSS for styling:
    ```
    npm install -D tailwindcss
    npx tailwindcss init
    ```

5. **Vite Setup (if using)**: If using Vite, additionally run:
    ```
    npm install --legacy-peer-deps -D tailwindcss postcss autoprefixer
    npx tailwindcss init -p
    ```

6. **React Dependencies Installation**: Install React dependencies:
    ```
    npm install --legacy-peer-deps @react-three/fiber @react-three/drei maath react-tilt react-vertical-timeline-component @emailjs/browser framer-motion react-router-dom
    ```

7. **Source Folder Setup**: Set up the `src` folder with subdirectories for assets, components, utils, constants, and styling.

    *Shout out to this person for sharing useful code snippets:*
    [GitHub Gist](https://gist.github.com/adrianhajdin/b1d33c262941a7e21aad833a1cfc84b1)

8. **Run Development Server**: Once set up, run the development server:
    ```
    npm run dev
    ```
   Access the project using `localhost` on port `5173`.

## Technologies Used

My stack includes the following technologies:

- **Frontend**:
  - Three.js: A JavaScript library for creating and displaying 3D computer graphics in a web browser.
  - WebGL: A JavaScript API for rendering interactive 3D and 2D graphics within any compatible web browser.
  - HTML5/CSS3: Standard markup and styling languages for structuring and styling web pages.
  - JavaScript: The programming language used for client-side scripting.
- **Backend**:
  - Node.js: A JavaScript runtime built on Chrome's V8 JavaScript engine for building scalable network applications.
  - Express.js: A minimal and flexible Node.js web application framework for building web applications and APIs.
  - MongoDB: A NoSQL database for storing data in JSON-like documents with dynamic schemas.
- **Deployment**:
  - Docker: A platform for developing, shipping, and running applications in containers.
  - Kubernetes: An open-source container orchestration platform for automating deployment, scaling, and management of containerized applications.




