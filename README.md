# Blog API with Express.js

![image](https://github.com/user-attachments/assets/41a655d3-444e-4e41-a4ec-2d66edbafa74)

This is a simple **Express.js** application that provides a RESTful API for managing blog posts. It allows users to create, retrieve, update, and delete posts using HTTP methods. The API is designed to be simple and efficient for building and testing blog-related functionalities.

## Features
- CRUD operations for blog posts: Create, Read, Update, Delete.
- In-memory data store (posts are lost when the server restarts).
- Allows retrieving all posts or specific posts by ID.
- Updates individual post fields like title, content, and author.

## Tech Stack
- **Backend**: Node.js, Express.js
- **Template Engine**: EJS (for potential future front-end integration)
- **Body Parser**: For parsing incoming request bodies
- **Data Storage**: In-memory array (data is not persistent)

## Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/blog-api.git
   cd blog-api
   npm i
   nodemon index.js
   nodemon server.js

## Usage

### Endpoints

#### `GET /posts`
- **Description**: Fetch all blog posts.
- **Response**:
   ```json
   [
     {
       "id": 1,
       "title": "The Rise of Decentralized Finance",
       "content": "Decentralized Finance (DeFi) is an emerging and rapidly evolving field...",
       "author": "Aya Issawy",
       "date": "2023-08-01T10:00:00Z"
     },
     ...
   ]
### Response
{
  "id": 1,
  "title": "The Rise of Decentralized Finance",
  "content": "Decentralized Finance (DeFi) is an emerging and rapidly evolving field...",
  "author": "Aya Issawy",
  "date": "2023-08-01T10:00:00Z"
}
### POST /posts
Description: Create a new post.
Request Body:
{
  "title": "New Post Title",
  "content": "Content of the new post",
  "author": "Author Name"
}
### File Structure
blog-api/
├── node_modules/      # Installed dependencies
├── views/             # EJS templates (if needed)
│   └── index.ejs      # Main template for displaying API responses
├── package.json       # Node.js package configuration
├── app.js             # Main server file
├── README.md          # Project documentation

## Dependencies
- **Express**: Web framework for Node.js.
- **Axios**: HTTP client for making API requests.
- **EJS**: Template engine for rendering dynamic HTML.
