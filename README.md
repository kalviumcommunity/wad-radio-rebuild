# City Radio - responsive rebuild starter

A deliberately broken, fixed-width page for the LU45 (Media Queries) code sandbox.

- `index.html` - City Radio markup (do not edit).
- `style.css` - broken, fixed `900px` / always-3-columns stylesheet. Students rebuild this mobile-first with at least two media queries.
- `package.json` - runs a Vite dev server so StackBlitz shows a live Preview. StackBlitz imports a GitHub repo as a WebContainer and only renders a preview if a start script exists; without this file the preview stays stuck on "Booting WebContainer". Do not delete it.

## Publishing this so the StackBlitz embed works

StackBlitz's generic blank "web-platform" starter no longer ships files (it opens a bolt.new AI page with an empty file tree), so the lesson embeds a **GitHub repo** instead, exactly like the `nextbites` reference lesson.

1. Create a public GitHub repo (suggested name: `wad-radio-rebuild`) under the course org.
2. Push these two files (`index.html`, `style.css`) to its default branch.
3. The lesson embed points at:
   `https://stackblitz.com/github/<org>/wad-radio-rebuild?embed=1&file=style.css&hideNavigation=1&view=default`
   Update `<org>` in `lesson.mdx` to the real org/user if it differs.

Once the repo is public **and contains `package.json`**, StackBlitz boots the WebContainer, runs `npm install` then `vite`, and the Preview shows the live page. Students just edit `style.css` - no pasting. If the preview ever stays on "Booting WebContainer", confirm `package.json` is present on the default branch.
