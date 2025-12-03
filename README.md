# Suply Echo - Static Site

AI-Powered Cold Chain Monitoring Platform

## Deployment on Vercel

This is a static site that can be deployed directly to Vercel.

### Quick Deploy

1. Connect your GitHub repository to Vercel
2. Vercel will automatically detect the configuration from `vercel.json`
3. The site will be deployed with all routes working correctly

### Configuration

- **Output Directory**: `public_html` (configured in `vercel.json`)
- **Build Command**: None required (static site)
- **Routes**: All HTML files and static assets are automatically served

### Available Pages

- `/` - Main landing page (index.html)
- `/asd.html` - Echo device connection page
- `/scany.html` - Bluetooth scanning page
- `/demo.html` - Demo page
- `/demo_report.html` - Demo report page
- `/demoreport.html` - Alternative demo report
- `/playbook_cc_ai.html` - Playbook page

### Static Assets

All static assets in `public_html/` are served with proper caching headers:
- CSS files
- JavaScript files
- Images
- Fonts
- Other static files

### Custom Domain

After deployment, you can configure a custom domain in Vercel settings.

