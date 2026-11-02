# Healthy Recipe Generator

A web page for GitHub Pages. It uses only HTML, CSS and JavaScript, with no server or Streamlit.

- Matches ingredients and utensils to 52 built-in healthy recipes, including local-style dishes
- Asks about allergens from a list, with a box for anything else, and removes recipes that match
- Shows estimated calories and nutrition, plus healthy add-on suggestions
- Suggests alternatives from a built-in list, with a search link for cookbook advice
- Downloads each recipe as an A4 PDF with credited photos when available
- Optional: visitors can add their own Gemini key to create new recipes and search online for cookbook alternatives

## Publish on GitHub Pages

1. Create a **public** repository on GitHub.
2. Upload every file in this folder, including `.nojekyll`, to the top level of the repository.
3. Open **Settings > Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**, the branch to **main** and the folder to **/ (root)**, then select **Save**.
5. Wait a minute or two, then open the address GitHub shows on that page.

Don't put a Gemini key in any file here. Anyone can read a GitHub Pages site's files, including keys, even when they're stored as GitHub secrets and added during publishing.

## Change the recipes

Recipes, foods and alternatives are in `data.js`.

## Good to know

- **Allergens:** the check looks for known food words and some likely hidden allergens, so it can't catch everything. Always read product labels and check for cross-contamination.
- **Nutrition:** figures are estimates, not lab values or medical advice.
- **Recipes:** recipes haven't been kitchen-tested. Built-in recipes and alternatives were written for this page and aren't taken from any cookbook.
- **Halal:** built-in recipes use no pork or alcohol. Choose halal-certified meat and products.
- **Images:** photos come from Wikimedia Commons under free licences and are credited. They show a similar dish, and some recipes may have no photo.
- **PDF text:** PDFs use a standard font for Western European characters. Other characters in AI text appear as `?`.
