## Setup

Open a terminal and navigate to the root of this repo. Run

```
npm install
```

Open VSCode and installed the recommended extensions. You might need to restart VSCode in order for extensions to take in effect. Restart by running `CMD+Shift+P` and search for "Reload Window", hit `Enter`.

## Run Dev Environment

```
npm run dev
```

Navigate to http://localhost:5173/

## Deploy to GH-Pages

**It is important that you follow these steps in the correct order:**

1. Add `"homepage": "https://hes-e39.github.io/<repo>/"` to `package.json`. Where `<repo>`, is the name of this repo.
2. Push to GH
3. Wait until action finishes, this will create a new branch `gh-pages`
4. In your GH repo: Settings -> Pages -> Build and deployment -> Branch -> gh-pages
5. Once all GH actions have completed, you can navigate to `https://hes-e39.github.io/<repo>/` and you should see your app.

You might have to hard refresh the browser page when pushing multiple updates to GH in order to reflect the most recent changes.
