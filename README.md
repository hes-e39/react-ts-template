## Dev Setup

**Prerequisite: you have `node` installed on the command line and can run `node --version`**

1. Open a terminal and navigate to the root of this repository
2. Run: `npm install`
3. Install [VSCode](https://code.visualstudio.com/?wt.mc_id=vscom_downloads)
4. Open VSCode. Install the recommended extensions that pop up in the bottom right. If you don't see this, then you can manually install the following two extensions: [BiomeJS](https://marketplace.visualstudio.com/items?itemName=biomejs.biome) and [TailwindCSS](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss).
5. You might need to restart VSCode in order for extensions to take in effect. Restart by running `CMD+Shift+P` and search for "Reload Window", hit `Enter`.
6. Verify that BiomeJS is working by adding some extra indents/spaces in `src/main.tsx`. It should format the file on save.
7. Start the dev server with `npm run dev` and navigate to http://localhost:5173/

## Deploy to GH-Pages

**It is important that you follow these steps in the correct order:**

1. Add `"homepage": "https://hes-e39.github.io/<repo>/"` to `package.json`. Where `<repo>`, is the name of this repo.
2. Push to GH
3. Wait until action finishes, this will create a new branch `gh-pages`
4. In your GH repo: Settings -> Pages -> Build and deployment -> Branch -> gh-pages
5. Once all GH actions have completed, you can navigate to `https://hes-e39.github.io/<repo>/` and you should see your app.

You might have to hard refresh the browser page when pushing multiple updates to GH in order to reflect the most recent changes.
