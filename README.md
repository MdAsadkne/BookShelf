# BookShelf | Personal reading tracker

Track your next chapter, favorite genres, and finished reads. This portfolio app includes a responsive React interface, a Spring Boot REST API, and H2 persistence.

> Demo content is fictional and stored locally in the live frontend.

## Live demo

[Open BookShelf](https://mdasadkne.github.io/BookShelf/)

## Features

- Create, edit, search, filter, and remove books.
- Track genre, author, pages, due dates, and workflow status.
- Responsive React UI with sample data and browser-local demo persistence.
- Spring Boot CRUD API with validation and H2 storage for local development.

## Stack

React 19, Vite 8, Java 17, Spring Boot 3.5.6, Spring Data JPA, Validation, H2, GitHub Actions, GitHub Pages.

## Run locally

Requirements: Node.js 22+, Java 17+, Maven 3.9+.

```sh
cd frontend
npm ci
npm run dev
```

Start the API in another terminal with `cd backend && mvn spring-boot:run`. Set `VITE_API_BASE_URL=http://localhost:8080/api` in `frontend/.env.local` to use it. Without this setting the live app uses browser storage.

## API

`GET /api/entries`, `GET /api/entries/{id}`, `POST /api/entries`, `PUT /api/entries/{id}`, `PATCH /api/entries/{id}/status?status=ACTIVE`, and `DELETE /api/entries/{id}`.

## Scope

This is an educational portfolio demo. It has no accounts, shared workspaces, or production data.

MIT license.
