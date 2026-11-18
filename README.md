# Module 5 - Week 3 Day 2 Homework: Full CRUD with JSON Server (Second Commit)

## Overview
This repository contains the complete **CRUD (Create, Read, Update, Delete)** RESTful API React app for **Module 5 Week 3 Day 2** (**WEB 403/603 Full Stack Web Development**, Westcliff University).

## Features Completed in Second Commit (Homework)
1. **Create (`src/CreateList.js`):**
   - **Create New List** button opens a React-Bootstrap modal with Title & Author inputs.
   - Submits a `POST` request to `http://localhost:5000/posts` via `createList`, resets form state, and reloads the list.
2. **Update (`src/UpdateList.js`):**
   - Row-level **Update** button loads the selected item via `GET /posts/:id` (`getList`) into a modal.
   - Submits a `PUT` request to `http://localhost:5000/posts/:id` (`updateList`) and refreshes the list.
3. **Delete (`src/DeleteList.js`):**
   - Row-level **Delete** button displays the selected item in a confirmation modal with disabled inputs.
   - Submits a `DELETE` request to `http://localhost:5000/posts/:id` (`deleteList`) and refreshes the list.
4. **Updated `src/Lists.js` & `src/App.js`:**
   - Integrated `UpdateList` and `DeleteList` into the table columns and connected all REST handlers (`getLists`, `handleChange`, `createList`, `getList`, `updateList`, `deleteList`).

## How to Run Locally
```bash
cd crud-json-server
npm install
npm run dev
```
Open `http://localhost:3000` to test **Get Lists**, **Create New List**, **Update**, and **Delete** against `http://localhost:5000/posts`.
