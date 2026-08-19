# Goodreads-Style MERN App

A full-stack MERN clone of core Goodreads functionality: an admin panel for
managing books, authors, and categories, and a user-facing side for building
reading lists (Read / Currently Reading / Want to Read) and leaving reviews and
ratings.

## Features

**Admin**
- Full CRUD on books, authors, and categories
- Group books into collections
- Admin-only auth-gated access

**Users**
- Signup/login (JWT-based auth)
- Personal reading lists with per-book status (Read / Currently Reading / Want to Read)
- Reviews and star ratings on books
- Filter books by category or author

## Tech Stack

- **Backend**: Node.js, Express, MongoDB (Mongoose), JWT auth, bcrypt, Multer (uploads)
- **Frontend**: React, TypeScript, Vite, Reactstrap, Redux

## API Routes

```
/books        book CRUD
/authors      author CRUD
/categories   category CRUD
/users        signup / login
```

(`UserBook` relates users ↔ books with a reading `state`, review, and rating.)

## Getting Started

```bash
# Backend
cd Backend
npm install
# set MONGO_URI and JWT_SECRET_KEY in a .env file
npm start

# Frontend
cd Frontend
npm install
npm run dev
```
