# ClearMind AI

ClearMind AI helps students understand difficult text by turning it into:
- A plain-English explanation
- Key takeaways
- A short summary
- Important terms with simple definitions

## Files
- `index.html` — page structure
- `style.css` — responsive styling
- `script.js` — file upload, Gemini API request, and results

## Run in VS Code
1. Download and unzip the project.
2. Open the `clearmind-ai` folder in VS Code.
3. Open `index.html` in your browser, or use the VS Code Live Server extension.
4. Click **AI setup** in the top-right corner.
5. Paste a Gemini API key from https://aistudio.google.com/apikey and click **Use this key**.
6. Paste text or upload a `.txt` file, choose the explanation level, and click **Simplify my text**.

## Important API-key warning
This beginner version calls Gemini directly from the browser so it can run with only HTML, CSS, and JavaScript. The API key is kept in page memory and is not saved to local storage, but browser-based keys can still be inspected by the person using the page and may be exposed if the app is shared or deployed. **Do not publish a personal API key or deploy this version with your own key.** For a public hackathon demo, use a small backend/serverless function to keep the key in an environment variable.

## Current upload support
This version reads plain `.txt` files. For PDF/DOCX, copy the text into the text area for now; proper document parsing can be added later.

## Suggested next improvements
- Add a secure backend for AI requests
- Add PDF and DOCX text extraction
- Add “explain with an example” and “make quiz questions”
- Add loading, error, and empty states tests
