# Next international checkout: email-first POC

Interactive prototype with ten first-screen optimisation concepts using the Next Fabric theme, fonts and icons. Static HTML and JavaScript: no installation, build command, API keys or dependencies required.

## Upload to GitHub and publish

1. Extract the ZIP on your computer.
2. Create a new GitHub repository, e.g. `next-login-poc`, or open the repository you want to use.
3. Choose **Add file → Upload files** and upload the extracted files. Upload `index.html` and `icons.svg` directly to the repository root, alongside this README. Do not upload the ZIP itself or put the files inside another folder.
4. Commit the files to `main`.
5. In the repository, open **Settings → Pages**.
6. Under **Build and deployment**, choose **Deploy from a branch**, then select **main** and **/ (root)**. Save.
7. Open the website URL shown by GitHub Pages after deployment completes. It usually looks like `https://YOUR-USERNAME.github.io/next-login-poc/`.

GitHub Pages availability and repository visibility depend on your account and organisation settings. Check these before publishing company material.

## Try the prototype

- Switch between concepts 1–10; concepts 6–10 are labelled New.
- Select Existing customer or New customer in the demo control, enter any valid dummy email, and continue.
- Existing customer leads to a password screen; New customer leads to guest checkout.
- Use the mobile-width preview or resize the browser.
- Concept 8 has expandable help; concept 10 has expandable alternative checkout actions.

No account lookup, authentication, email or payment service is connected. No credentials are transmitted or stored by the prototype. All outcomes are simulated. Use dummy details only.

## Files and editing

- `index.html`: complete interface, embedded Fabric theme/fonts, CSS and interaction logic.
- `icons.svg`: local Next icon sprite; keep beside index.html.
- `.nojekyll`: prevents Jekyll processing where included.
- `.gitignore`: ignores operating-system metadata.

Edit the `concepts` array and the `first()` function in index.html to change explanatory text and concept screens.

## Avoid a blank page

This POC loads directly from index.html: there is no React build or Vite base-path configuration to manage. Assets use relative paths and work under a GitHub repository URL. If the site is missing, check that index.html is at the top level and Pages points to main / (root). If icons are missing, confirm icons.svg is alongside index.html. When replacing an existing POC, refresh the page after deployment completes.

## Branding

Includes the Fabric theme, fonts and Next icons supplied for this prototype. This package does not grant redistribution rights to those brand assets.
