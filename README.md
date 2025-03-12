# Coffee Roasters Directory

A nationwide directory of coffee roasters in the USA, built with simple HTML, CSS, and JavaScript.

## Project Overview

This project creates a static website for a coffee roaster directory with the following features:

- Homepage optimized for "Coffee Roasters Near Me"
- State pages listing coffee roasters by state
- City pages listing coffee roasters in specific cities
- SEO-friendly URL structure: domain.com/state/city/
- Weighted rating system that considers both star ratings and number of reviews
- Responsive design for all device sizes
- Proper image association with each business

## Directory Structure

```
site/                   # Main site directory
├── index.html          # Homepage
├── static/             # Static assets
│   ├── css/            # CSS files
│   ├── js/             # JavaScript files
│   └── img/            # Images
│       ├── roasters/   # Coffee roaster images
│       └── coffee-roaster-hero-image.jpeg
├── [state]/            # State directories
│   ├── index.html      # State page
│   └── [city]/         # City directories
│       └── index.html  # City page
```

## Technical Details

- **Data Source**: Excel spreadsheet with 5000+ coffee roasters
- **Images**: Local copies of images from Google, properly associated with each business
- **SEO**: Each page has appropriate meta titles and descriptions
- **Header/Footer**: Standalone components for easy site-wide updates

## Deployment

The site can be deployed to GitHub Pages and then to Vercel by following these steps:

1. Push the `site` directory to a GitHub repository
2. Connect the repository to Vercel
3. Configure Vercel to deploy from the `site` directory

## Local Development

To run the site locally:

1. Navigate to the `site` directory
2. Start a local server (e.g., `python -m http.server`)
3. Open `http://localhost:8000` in your browser

## Scripts

- `build_site.py`: Generates the entire site from the Excel data
- `download_images.py`: Downloads and processes images from Google URLs

## License

This project is licensed under the MIT License - see the LICENSE file for details. 