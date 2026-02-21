# Skeleton Coin - Meme Coin Landing Page

A modern, responsive landing page for a meme coin cryptocurrency, featuring a skeleton warrior theme.

## Setup Instructions

1. **Add the Skeleton Warrior Image**
   - Place your skeleton warrior image file in: `assets/images/skeleton-warrior.png`
   - The image should be a PNG file with a transparent or dark background
   - Recommended size: 800x800px or larger for best quality

2. **Open the Website**
   - Simply open `index.html` in your web browser
   - Or use a local server for best results:
     ```bash
     # Using Python
     python -m http.server 8000
     
     # Using Node.js (http-server)
     npx http-server
     ```
   - Then navigate to `http://localhost:8000`

## Features

- ✅ Modern, responsive design
- ✅ Smooth scrolling navigation
- ✅ Animated hero section with skeleton warrior
- ✅ Tokenomics section with progress bars
- ✅ Roadmap timeline
- ✅ Buy section with contract address
- ✅ Social media links
- ✅ Mobile-friendly layout

## Customization

### Colors
Edit the CSS variables in `assets/css/style.css`:
```css
:root {
    --primary-color: #8b5cf6;
    --secondary-color: #ec4899;
    --dark-bg: #0a0a0f;
    /* ... */
}
```

### Content
- Update text content in `index.html`
- Modify contract address in the buy section
- Update social media links in the footer

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Technologies Used

- Bootstrap 5.3.0
- Font Awesome 6.4.0
- Vanilla JavaScript
- CSS3 with animations
