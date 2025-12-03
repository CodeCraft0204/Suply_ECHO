# Vercel Deployment Guide

## Configuration Settings

When importing the repository to Vercel, use these settings:

### Framework Preset
- **Select: "Other"** or **"Other"** from the dropdown
- Do NOT select React, Next.js, Vue, etc.

### Root Directory
- **Leave empty** (use project root) OR set to `.` (current directory)
- The `vercel.json` file should be in the root directory

### Build Command
- **Leave empty** (no build needed for static site)
- Or set to: `echo "No build needed"`

### Output Directory
- **Set to: `public_html`**
- This tells Vercel where your static files are located

### Install Command
- **Leave empty** (no dependencies to install)

## Alternative: Manual Configuration

If the UI doesn't work, you can also:

1. **Import repository** without changing any settings
2. Go to **Settings** → **General**
3. Under **Build & Development Settings**:
   - Framework Preset: **Other**
   - Root Directory: **Leave empty** (or `.`)
   - Build Command: **Leave empty**
   - Output Directory: **`public_html`**
   - Install Command: **Leave empty**

## Verification

After deployment, verify these URLs work:
- `https://your-domain.vercel.app/` → Should show index.html
- `https://your-domain.vercel.app/asd.html` → Should show asd.html
- `https://your-domain.vercel.app/scany.html` → Should show scany.html
- `https://your-domain.vercel.app/nc_assets123/css/style.css` → Should load CSS

## Troubleshooting

If you still get 404 errors:

1. Check that `vercel.json` is in the root directory
2. Verify `outputDirectory` is set to `public_html`
3. Make sure Framework Preset is set to "Other"
4. Check Vercel deployment logs for any errors

