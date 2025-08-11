# Hrudu Shibu - Portfolio Website

A modern, responsive portfolio website built with HTML5, CSS3, JavaScript, and Bootstrap 5.

## 🚀 Live Demo

[View Portfolio](https://hrudu.me/)

## 📋 Features

- **Responsive Design**: Optimized for all devices (desktop, tablet, mobile)
- **Modern UI/UX**: Clean, professional design with smooth animations
- **Bootstrap 5**: Utilizes the latest Bootstrap framework
- **Font Awesome Icons**: Professional iconography
- **Smooth Scrolling**: Enhanced navigation experience
- **Interactive Elements**: Hover effects and animations
- **SEO Optimized**: Semantic HTML structure
- **Fast Loading**: Optimized assets and code

## 🛠️ Technologies Used

- HTML5
- CSS3 (Custom properties, Flexbox, Grid)
- JavaScript (ES6+)
- Bootstrap 5.3.2
- Font Awesome 6.4.0

## 📁 Project Structure

```
my-portfolio/
├── index.html              # Main HTML file
├── css/
│   └── style.css           # Custom CSS styles
├── js/
│   └── main.js            # JavaScript functionality
├── assets/
│   ├── profile.jpg        # Profile image (add your photo here)
│   └── Hrudu_Shibu_Resume.pdf  # Resume PDF (add your resume here)
└── README.md              # Project documentation
```

## 🚀 Getting Started

### Prerequisites

- A modern web browser
- Git (for version control)
- A code editor (VS Code recommended)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/my-portfolio.git
   cd my-portfolio
   ```

2. **Add your content**
   - Replace `assets/profile.jpg` with your professional photo
   - Add your resume as `assets/Hrudu_Shibu_Resume.pdf`
   - Update any personal information in `index.html`

3. **Test locally**
   - Open `index.html` in your browser
   - Or use a local server (recommended):
     ```bash
     # Using Python 3
     python -m http.server 8000
     
     # Using Node.js (if you have http-server installed)
     npx http-server
     ```

## 🌐 Deployment to GitHub Pages with Custom Domain

1. **Create a new repository on GitHub**
   - Repository name: `your-username.github.io` (recommended) or `my-portfolio`
   - Make it public

2. **Push your code**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/your-username/my-portfolio.git
   git push -u origin main
   ```

3. **Configure your custom domain DNS**
   
   **For apex domain (hrudu.me):**
   Add these A records in your DNS provider:
   ```
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```
   
   **For www subdomain (optional):**
   Add a CNAME record:
   ```
   www.hrudu.me → your-username.github.io
   ```

4. **Enable GitHub Pages**
   - Go to repository Settings
   - Scroll down to "Pages" section
   - Source: Deploy from a branch
   - Branch: main / (root)
   - Custom domain: `hrudu.me`
   - Check "Enforce HTTPS" (wait for SSL certificate)
   - Save

5. **Verify your domain**
   - GitHub will automatically verify your domain
   - It may take 24-48 hours for DNS changes to propagate

6. **Access your site**
   - Your site will be available at: `https://hrudu.me`
   - GitHub will automatically redirect www.hrudu.me to hrudu.me

## 🎨 Customization

### Colors
Update the CSS custom properties in `css/style.css`:
```css
:root {
    --primary-color: #0d6efd;        /* Main theme color */
    --secondary-color: #6c757d;      /* Secondary color */
    --dark-color: #212529;           /* Dark text color */
    --light-color: #f8f9fa;          /* Light background */
}
```

### Content
- Update personal information in `index.html`
- Modify sections as needed
- Add or remove skills, experience, etc.

### Images
- Profile image: `assets/profile.jpg` (recommended: 500x500px, square aspect ratio)
- Resume: `assets/Hrudu_Shibu_Resume.pdf`

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## 🔧 Performance Optimizations

- Minified CSS and JavaScript (for production)
- Optimized images
- CDN-hosted libraries
- Efficient animations

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📞 Contact

Hrudu Shibu - [hrudu.shibu@outlook.com](mailto:hrudu.shibu@outlook.com)

Project Link: [https://github.com/your-username/my-portfolio](https://github.com/your-username/my-portfolio)

## 🙏 Acknowledgments

- [Bootstrap](https://getbootstrap.com/) for the responsive framework
- [Font Awesome](https://fontawesome.com/) for the icons
- [GitHub Pages](https://pages.github.com/) for hosting

---

⭐ **Star this repository if you found it helpful!**
