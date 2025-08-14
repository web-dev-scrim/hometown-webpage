## Hometown Webpage

A simple webpage showcasing my hometown built with Vite and deployed to Netlify.

### Development

1. Install dependencies:
```bash
npm install
```

2. Start development server:
```bash
npm run dev
```

3. Build for production:
```bash
npm run build
```

4. Preview production build:
```bash
npm run preview
```

### Deployment

This project is automatically deployed to Netlify via GitHub Actions when changes are pushed to the main/master branch.

#### Setup Instructions:

1. **Create a Netlify account** and connect your GitHub repository
2. **Get your Netlify credentials:**
   - Go to Netlify Dashboard → User Settings → Applications → Personal Access Tokens
   - Create a new token and copy it
   - Go to your site settings and copy the Site ID

3. **Add GitHub Secrets:**
   - Go to your GitHub repository → Settings → Secrets and variables → Actions
   - Add these secrets:
     - `NETLIFY_AUTH_TOKEN`: Your personal access token
     - `NETLIFY_SITE_ID`: Your site ID from Netlify

4. **Push to main/master branch** and the GitHub Action will automatically build and deploy your site.

### Project Structure

```
hometown-webpage/
├── index.html          # Main HTML file
├── styles.css          # CSS styles
├── images/            # Image assets
├── package.json       # NPM dependencies
├── vite.config.js     # Vite configuration
└── .github/workflows/ # GitHub Actions
```
