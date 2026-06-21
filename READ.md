# Instagram-style Profile Page (Express + EJS Practice)

A small practice project built while learning the basics of backend development with **Express.js** and **EJS templating**. This was my first hands-on project after completing Express and EJS lectures, focused on understanding how a server receives requests, processes data, and returns rendered HTML.

## What this project does

Renders a simple Instagram-style profile page (e.g. `/ig/cats`) that displays:
- Profile info — username, followers, following
- A list of posts with an image, like count, and comment count

All data is read from a local `data.json` file and injected into an EJS template using interpolation.

## What I learned

- Setting up a basic Express server and listening on a port
- Creating routes with `app.get()` and handling different paths (e.g. `/home`, `/search`)
- Working with **route/query parameters** and how Express parses them
- Organizing routes into a separate `routes/` folder and requiring them in `index.js`
- Using **EJS** to render dynamic HTML — interpolation syntax (`<%= %>`), looping over data with `<% %>`
- Reading and passing local JSON data (`data.json`) into views via `res.render()`
- How a request/response cycle actually works under the hood
- Testing API endpoints manually with **Hoppscotch** (checking status codes, response time, response body)

## Tech stack

- Node.js
- Express.js
- EJS (Embedded JavaScript templates)

## Project structure

```
.
├── index.js          # Entry point — sets up the Express app and routes
├── data.json          # Static data used to populate the EJS views
├── routes/             # Route handlers
├── views/
│   └── instagram.ejs  # EJS template for the profile page
├── package.json
└── README.md
```

## Getting started

1. Clone the repo
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```

2. Install dependencies
   ```bash
   npm install
   ```

3. Run the server
   ```bash
   node index.js
   ```

4. Visit the app in your browser, e.g.
   ```
   http://localhost:3000/ig/cats
   ```
   (adjust the port/route based on your actual `index.js` setup)

## Notes

This is an early learning project — the focus was on understanding Express routing and EJS templating fundamentals, not on building a production-ready app. Next steps for me: connecting a real database instead of a static JSON file, and adding form handling / POST routes.

## Author

**Zarqa**
Software Engineering student | Learning full-stack web development