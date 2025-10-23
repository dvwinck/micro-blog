# Micro Blog

A simple micro-blogging platform with a frontend and backend service.

## Project Structure

```
micro-blog/
├── back/               # Backend service
│   ├── db.js           # Database configuration
│   ├── package.json    # Backend dependencies
│   └── server.js       # Backend server
├── front/              # Frontend service
│   ├── package.json    # Frontend dependencies
│   ├── postcss.config.cjs # PostCSS configuration
│   ├── tailwind.config.cjs # Tailwind CSS configuration
│   ├── scripts/        # Utility scripts
│   │   └── copy-html.js
│   └── src/            # Frontend source files
│       ├── index.html  # Main HTML file
│       └── styles.css  # CSS styles
├── .gitignore          # Git ignore rules
└── LICENSE             # Project license
```

## Prerequisites

- Node.js (for development)
- npm or yarn (for package management)

## Setup and Running

### For Development

1. Clone the repository:
   ```bash
   git clone https://github.com/dvwinck/micro-blog.git
   cd micro-blog
   ```

2. Install dependencies for both frontend and backend:
   ```bash
   cd back && npm install && cd ../front && npm install
   ```

3. Start the backend server:
   ```bash
   cd back && npm start
   ```

4. Build the frontend assets:
   ```bash
   cd front && npm run build
   ```

5. The backend API will be available at:
   - `http://localhost:3000`

6. To view the frontend, you'll need to serve the built files from the `front/dist` directory using a web server of your choice.
ex: npx serve dist -l 8080

## Development

### Backend

The backend service is a Node.js application. You can work on it directly in the `back/` directory.

### Frontend

The frontend service uses HTML, CSS, and JavaScript with Tailwind CSS for styling. You can find the source files in the `front/src/` directory.

## License

This project is licensed under the terms of the [LICENSE](LICENSE) file.
