# Compass Lawn Care & Maintenance Website

A professional Jekyll website for Matt McLean's lawn care business serving the Fraser Valley from Chilliwack to Surrey.

## 🌿 Features

- **Modern, Responsive Design** - Looks great on all devices
- **SEO Optimized** - Built for search engines with local business schema
- **Contact Forms** - Powered by Formspree for easy lead generation
- **Service Areas** - Comprehensive coverage display
- **Click-to-Call** - Mobile-friendly phone number integration
- **Professional Layout** - Clean, trustworthy design

## 📱 Contact Information

- **Owner:** Matt McLean
- **Phone:** 604-768-8382
- **Email:** compasslawncare1@gmail.com

## 🚀 Quick Start

### Prerequisites

1. Install Ruby (version 2.7 or higher)
2. Install Jekyll and Bundler:
   ```bash
   gem install jekyll bundler
   ```

### Setup

1. Clone or download this repository
2. Navigate to the project directory:
   ```bash
   cd compasslawncare
   ```
3. Install dependencies:
   ```bash
   bundle install
   ```
4. Start the development server:
   ```bash
   bundle exec jekyll serve
   ```
5. Open your browser to `http://localhost:4000`

## 📁 Project Structure

```
compasslawncare/
├── _config.yml          # Site configuration
├── _data/               # Data files
│   ├── services.yml     # Service listings
│   ├── service-areas.yml # Coverage areas
│   └── owner.yml        # Business owner info
├── _includes/           # Reusable components
│   ├── header.html      # Navigation
│   ├── footer.html      # Site footer
│   ├── service-card.html # Service display cards
│   ├── contact-cta.html # Contact call-to-action
│   └── service-area-map.html # Service areas display
├── _layouts/            # Page templates
│   ├── default.html     # Base template
│   └── page.html        # Content page template
├── assets/              # Static files
│   ├── css/style.css    # Main stylesheet
│   ├── js/main.js       # JavaScript functionality
│   └── images/          # Images and logos
├── index.html           # Home page
├── services.html        # Services & pricing page
├── Gemfile             # Ruby dependencies
└── README.md           # This file
```

## ✏️ Customization

### Updating Business Information

Edit `_config.yml` to update:
- Business name and description
- Contact information
- Service areas

### Adding/Editing Services

Edit `_data/services.yml` to:
- Add new services
- Update descriptions
- Mark services as featured (shown on homepage)

### Updating Service Areas

Edit `_data/service-areas.yml` to:
- Add new coverage areas
- Update area descriptions
- Mark areas as featured

### Updating Owner Information

Edit `_data/owner.yml` to:
- Update bio and credentials
- Change specialties
- Add certifications

## 📧 Contact Form Setup

The website uses Formspree for contact forms. To set up your own:

1. Sign up at [formspree.io](https://formspree.io)
2. Create a new form
3. Replace the form action URL in:
   - `_includes/contact-cta.html`
   - `services.html`
4. Update the email address to: `compasslawncare1@gmail.com`

## 🎨 Styling

The website uses custom CSS with:
- Modern color scheme (green primary, professional grays)
- Responsive grid layouts
- Font Awesome icons
- Inter font family
- Mobile-first design approach

### Color Palette
- Primary Green: `#22c55e`
- Dark Green: `#16a34a`
- Blue Accent: `#3b82f6`
- Dark Gray: `#1f2937`
- Light Gray: `#f9fafb`

## 📱 Mobile Optimization

- Responsive navigation with hamburger menu
- Touch-friendly buttons and links
- Optimized forms for mobile input
- Click-to-call phone numbers
- Compressed images and optimized loading

## 🔍 SEO Features

- Local business schema markup
- Optimized meta descriptions
- Semantic HTML structure
- Clean URLs with Jekyll
- Sitemap generation
- Fast loading times

## 🚀 Deployment Options

### GitHub Pages (Free)
1. Push your code to a GitHub repository
2. Enable GitHub Pages in repository settings
3. Your site will be available at `username.github.io/repo-name`

### Netlify (Recommended)
1. Connect your GitHub repository to Netlify
2. Netlify will automatically build and deploy your site
3. Get a custom domain or use the provided netlify.app URL
4. Forms will work automatically with Netlify Forms

### Custom Hosting
1. Run `bundle exec jekyll build` to generate the `_site` folder
2. Upload the contents of `_site` to your web hosting provider

## 📊 Analytics Setup

To add Google Analytics:
1. Get your Google Analytics tracking ID
2. Add it to `_config.yml` under a new `google_analytics` section
3. The tracking code is already included in the default layout

## 🔧 Maintenance

### Regular Updates
- Review and update service listings quarterly
- Check contact information accuracy
- Update testimonials as you receive them
- Add new service areas as your business grows

### Content Updates
- Add seasonal service promotions
- Update pricing information
- Include before/after photo galleries
- Add blog posts about lawn care tips

## 📞 Support

For technical support or questions about this website:
- Contact information is in the site header
- Form submissions go to: compasslawncare1@gmail.com

## 📝 License

This website is custom-built for Compass Lawn Care & Maintenance. All content and design rights reserved.

---

**Built with ❤️ for professional lawn care services in the Fraser Valley** 