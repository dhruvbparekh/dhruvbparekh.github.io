# Dhruv Bhavesh Parekh - Portfolio Website

A modern, responsive portfolio website showcasing education, work experience, projects, and skills.

## Features

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Modern UI**: Clean and professional design with smooth animations
- **Easy Navigation**: Fixed header with smooth scrolling to sections
- **SEO Friendly**: Proper HTML structure and meta tags
- **Fast Loading**: Minimal dependencies, optimized performance

## File Structure

```
dhruv_website/
├── index.html          # Main HTML file
├── styles.css          # CSS styles
├── script.js           # JavaScript for interactivity
└── README.md           # This file
```

## Deployment to GitHub Pages

### Method 1: Using GitHub Web Interface

1. **Create a new repository on GitHub**
   - Go to [GitHub](https://github.com) and sign in
   - Click the "+" icon in the top right and select "New repository"
   - Name it `username.github.io` (replace `username` with your GitHub username)
   - Make it public
   - Don't initialize with README, .gitignore, or license
   - Click "Create repository"

2. **Upload your files**
   - On the repository page, click "uploading an existing file"
   - Drag and drop all files (`index.html`, `styles.css`, `script.js`, `README.md`)
   - Click "Commit changes"

3. **Enable GitHub Pages**
   - Go to repository Settings
   - Scroll down to "Pages" section
   - Under "Source", select "main" branch
   - Click "Save"
   - Your site will be live at `https://username.github.io`

### Method 2: Using Git Command Line

1. **Initialize Git repository**
   ```bash
   cd /nas/etc/dhruv_website
   git init
   git add .
   git commit -m "Initial commit: Portfolio website"
   ```

2. **Create a repository on GitHub**
   - Go to GitHub and create a new repository named `username.github.io`
   - Don't initialize with any files

3. **Push to GitHub**
   ```bash
   git remote add origin https://github.com/username/username.github.io.git
   git branch -M main
   git push -u origin main
   ```

4. **Enable GitHub Pages**
   - Go to repository Settings → Pages
   - Select "main" branch as source
   - Save and wait a few minutes

### Method 3: Using GitHub CLI

```bash
cd /nas/etc/dhruv_website
git init
git add .
git commit -m "Initial commit: Portfolio website"
gh repo create username.github.io --public --source=. --remote=origin --push
```

Then enable GitHub Pages in repository settings.

## Customization

### Update Content

Edit `index.html` to modify:
- Personal information
- Education details
- Work experience
- Projects
- Skills
- Contact information

### Change Colors

Edit `styles.css` and modify the CSS variables in the `:root` section:

```css
:root {
    --primary-color: #2c3e50;
    --secondary-color: #3498db;
    --accent-color: #e74c3c;
    /* Add your preferred colors */
}
```

### Add Sections

1. Add new section in `index.html`:
```html
<section id="newsection">
    <div class="container">
        <h2>New Section Title</h2>
        <!-- Your content here -->
    </div>
</section>
```

2. Add navigation link:
```html
<li><a href="#newsection">New Section</a></li>
```

3. Style it in `styles.css` as needed

## Local Development

To view the website locally:

1. **Using Python's HTTP server:**
   ```bash
   python3 -m http.server 8000
   ```
   Then open `http://localhost:8000` in your browser

2. **Using Node.js http-server:**
   ```bash
   npx http-server
   ```

3. **Direct file opening:**
   Simply open `index.html` in your web browser

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## Dependencies

- Font Awesome 6.4.0 (loaded via CDN for icons)

## License

Feel free to use this template for your own portfolio!

## Contact

- Email: dhruvparekh@my.utexas.edu
- LinkedIn: [dhruv-b-parekh](https://linkedin.com/in/dhruv-b-parekh)

---

Built with HTML, CSS, and JavaScript. No frameworks required!
