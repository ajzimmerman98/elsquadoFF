# elsquadoFF

## Project Summary
A website for the el squado fantasy football leauge. Will be able to track league stats as well as league history

## Tech Stack
### Frontend
  - VueJS - A progressive JavaScript framework for building user interfaces. It's lightweight, flexible, and works well with Python backends
      - Vue Router - For handling routing within the single-page application (SPA), allowing navigation between pages without refreshing the page
      - Vuex - State management library for Vue.js, useful for handling complex state in larger applications.
      - Axios for HTTP requests - A promise-based HTTP client used to interact with the backend APIs (sending requests to the Python backend)
      - Vuetify for UI components -Component libraries for Vue.js that provide pre-built UI components, speeding up development and ensuring responsive design
### Backend
  - FastAPI - Python framework that is easy to use, and the performance is excellent, especially for APIs. FastAPI is a good alternative to frameworks like Flask if you need better performance and built-in async support.
    - MongoDB - If your data structure is more flexible or involves a lot of unstructured data
    - OR PostgreSQL (database) - Popular relational databases to store structured data
    - Redis (optional, for caching) - An in-memory data store often used for caching, real-time processing, or managing sessions.
    - PyJWT (authentication) - For secure, stateless authentication between the frontend and backend. Libraries like PyJWT can be used in Flask to generate and verify tokens.
### Cloud/DevOps
- AWS - Hosting platform where you can deploy your Dockerized app. AWS S3/CloudFront can be used to serve Vue.js static files
  - Docker - Containerize your Vue.js frontend and Python backend applications to ensure consistency across different environments (development, staging, production)
  - NGINX - Often used as a reverse proxy server to handle requests between the frontend and backend. It can serve your static Vue.js files and route API requests to the Python backend
  - Uvicorn - Uvicorn is a lightning-fast ASGI server used with FastAPI
