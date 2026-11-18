# Module 5 - Week 3 Day 2 Exercise Demo: CRUD with JSON Server

## Overview
This repository contains the completed **Module 5 Week 3 Day 2 In-Class Exercise/Demo** for **WEB 403/603 Full Stack Web Development** at Westcliff University.

It demonstrates fetching RESTful API data in React from a local `json-server` database (`db.json` on port `5000`) and running both the React app and JSON server together with `concurrently`.

## Features Implemented
- **`db.json`**: Local JSON database containing the `posts` book list.
- **`package.json`**: Configured `json-server` and `concurrently` devDependencies with `"json-server"` and `"dev"` scripts.
- **`src/App.js`**: `getLists` handler using `fetch("http://localhost:5000/posts")` and conditional loading state rendering.
- **`src/Lists.js`**: Displays fetched JSON records in a Bootstrap striped table (`#`, `Title`, `Author`, `Update`, `Delete`).

## How to Run Locally
```bash
cd crud-json-server
npm install
npm run dev
```
Open `http://localhost:3000` and click **Get Lists** to load posts from `http://localhost:5000/posts`.
