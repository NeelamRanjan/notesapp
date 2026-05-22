<<<<<<< HEAD

# notesapp

# Deploy &amp; host React app using AWS Amplify

# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Oxc](https://oxc.rs)
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/)

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.

> > > > > > > b74c9de (first commit)

## Overview

AWS Amplify offers a Git-based CI/CD workflow for building, deploying, and hosting single-page web applications or static sites with serverless backends. When connected to a Git repository, Amplify determines the build settings for both the frontend framework and any configured serverless backend resources, and automatically deploys updates with every code commit.

## Step 1

### Create React Application

```
npm create vite@latest notesapp -- --template react
cd notesapp
npm install
npm run dev

```

### Create a new repository in GitHub and push the code to repo 

Open a new terminal window, navigate to your app's root folder (notesapp), and run the following commands to initialize a git and push the application to the new GitHub repo - 

```
git init
git add .
git commit -m "first commit"
git remote add origin git@github.com:<your-username>/notesapp.git 
git branch -M main
git push -u origin main

```
### install the Apmlify Packages 

```
npm create amplify@latest -y

```
### Push your changes to Github 

```
git add .
git commit -m 'installing amplify'
git push origin main

```
### Deploy the app with Amplify


