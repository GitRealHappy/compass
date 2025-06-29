# Compass Lawn Care & Maintenance Website

A professional Jekyll website for Matt McLean's lawn care business serving the Fraser Valley from Chilliwack to Surrey.

## 🌐 Live Site
- **Production URL:** https://www.compasslawns.com
- **GitHub Repository:** https://github.com/GitRealHappy/compass
- **Local Development:** http://localhost:4000

## 🌿 Features

- **Modern, Responsive Design** - Looks great on all devices
- **SEO Optimized** - Built for search engines with local business schema
- **Contact Forms** - Powered by Formspree for easy lead generation
- **Service Areas** - Comprehensive coverage display with interactive elements
- **Click-to-Call** - Mobile-friendly phone number integration
- **Professional Layout** - Clean, trustworthy design
- **Custom Domain** - Professional domain with GitHub Pages hosting
- **SSL Certificate** - Secure HTTPS connection
- **Form Validation** - Client-side and server-side form validation

## 📱 Contact Information

- **Owner:** Matt McLean
- **Business:** Compass Lawn Care & Maintenance
- **Phone:** 604-768-8382
- **Email:** compasslawncare1@gmail.com
- **Service Area:** Fraser Valley (Chilliwack to Surrey)

## 🚀 Quick Start

### Prerequisites

1. Install Ruby (version 2.7 or higher)
2. Install Jekyll and Bundler:
   ```bash
   gem install jekyll bundler
   ```

### Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/GitRealHappy/compass.git
   cd compass
   ```
2. Install dependencies:
   ```bash
   bundle install
   ```
3. Start the development server with live reload:
   ```bash
   bundle exec jekyll serve --livereload
   ```
4. Open your browser to `http://localhost:4000`

### Development Commands

```bash
# Serve with drafts
bundle exec jekyll serve --drafts

# Build for production
bundle exec jekyll build

# Clean build artifacts
bundle exec jekyll clean

# Check for dependency updates
bundle update
```

## 🏗️ Technical Architecture

### Jekyll Configuration

- **Jekyll Version:** 4.3.4
- **Ruby Version:** 3.3.0
- **Build Tool:** Bundler
- **CSS Framework:** Custom CSS with Flexbox/Grid
- **JavaScript:** Vanilla JS (no frameworks)
- **Icons:** Font Awesome 6
- **Fonts:** Inter (Google Fonts)

### Build Process

1. **Liquid Templating** - Dynamic content generation
2. **Sass Compilation** - CSS preprocessing
3. **Asset Pipeline** - Image optimization and minification
4. **Static Site Generation** - Compiled to `_site/` directory
5. **GitHub Pages Deployment** - Automatic build and deploy

## 📁 Project Structure

```
compasslawncare/
├── _config.yml              # Site configuration
├── CNAME                    # Custom domain configuration
├── _data/                   # Data files (YAML)
│   ├── services.yml         # Service listings with icons
│   ├── service-areas.yml    # Coverage areas and descriptions
│   └── owner.yml            # Business owner information
├── _includes/               # Reusable components
│   ├── header.html          # Navigation with mobile menu
│   ├── footer.html          # Site footer with links
│   ├── service-card.html    # Service display cards with icons
│   ├── contact-cta.html     # Contact form (homepage)
│   └── service-area-map.html # Service areas display
├── _layouts/                # Page templates
│   ├── default.html         # Base template with meta tags
│   └── page.html            # Content page template
├── assets/                  # Static files
│   ├── css/style.css        # Main stylesheet (1,200+ lines)
│   ├── js/main.js           # JavaScript functionality
│   └── images/              # Optimized images
│       ├── hero.png         # Homepage hero image
│       ├── logo.png         # Company logo
│       ├── logo1.png        # Logo variant
│       └── matt.jpeg        # Owner photo
├── _site/                   # Generated site (ignore in git)
├── index.html               # Homepage template
├── services.html            # Services & pricing page
├── Gemfile                  # Ruby dependencies
├── Gemfile.lock            # Locked dependency versions
└── README.md               # This documentation
```

## 🎨 Design System

### Color Palette
```scss
:root {
  --primary-green: #22c55e;
  --dark-green: #16a34a;
  --blue-accent: #3b82f6;
  --dark-gray: #1f2937;
  --medium-gray: #6b7280;
  --light-gray: #f9fafb;
  --white: #ffffff;
}
```

### Typography
- **Primary Font:** Inter (400, 500, 600, 700 weights)
- **Headings:** Font weights 600-700
- **Body Text:** Font weight 400-500
- **Responsive Scale:** 14px mobile to 18px desktop base

### Component Library
- **Buttons:** Primary, secondary, outline variants
- **Cards:** Service cards, testimonial cards, pricing cards
- **Forms:** Multi-step forms with validation
- **Navigation:** Responsive with mobile hamburger menu
- **Grid System:** Custom CSS Grid for layouts

## 📧 Contact Form System

### FormSpree Integration
- **Service:** Formspree.io
- **Endpoint:** `https://formspree.io/f/xovwyzkg`
- **Forms:** 2 forms (homepage and services page)
- **Validation:** Required fields, email format, phone format
- **Notifications:** Email alerts to compasslawncare1@gmail.com

### Form Locations
1. **Homepage Contact Form** (`_includes/contact-cta.html`)
   - Quick contact form
   - Basic information collection
   
2. **Services Page Form** (`services.html`)
   - Detailed quote request form
   - Service-specific options
   - Timeline and property size selectors

### Form Testing
Monthly testing recommended:
1. Submit test form with obvious test data
2. Verify email notification received
3. Check FormSpree dashboard for submission
4. Test both forms (homepage and services page)

## 🌐 Deployment & Hosting

### GitHub Pages Configuration
- **Host:** GitHub Pages
- **Repository:** GitRealHappy/compass
- **Branch:** main
- **Custom Domain:** www.compasslawns.com
- **SSL:** Automatic (Let's Encrypt)
- **Build:** Automatic on push to main

### DNS Configuration
```
# A Records for apex domain (compasslawns.com)
@    A    185.199.108.153
@    A    185.199.109.153
@    A    185.199.110.153
@    A    185.199.111.153

# CNAME Record for www subdomain
www  CNAME  GitRealHappy.github.io
```

### Custom Domain Setup
1. **CNAME File:** Contains `www.compasslawns.com`
2. **DNS Records:** Configured as above
3. **GitHub Settings:** Custom domain configured in repository settings
4. **SSL Certificate:** Automatically provisioned by GitHub

## ✏️ Content Management

### Updating Business Information
Edit `_config.yml` to update:
```yaml
business:
  name: "Compass Lawn Care & Maintenance"
  phone: "604-768-8382"
  email: "compasslawncare1@gmail.com"
  address: "Fraser Valley, BC"
```

### Managing Services
Edit `_data/services.yml`:
```yaml
- category: "Core Lawn Services"
  services:
    - name: "Lawn Mowing"
      description: "Regular mowing to keep your lawn healthy"
      icon: "grass"          # Maps to FontAwesome icon
      featured: true         # Shows on homepage
```

### Service Icons
Icons are defined in `_includes/service-card.html`:
- `grass` → `fa-seedling` (Lawn Mowing)
- `seed` → `fa-dot-circle` (Grass Seeding)
- `trim` → `fa-cut` (Weed Eating)
- `cleanup` → `fa-broom` (Cleanup)
- `fertilizer` → `fa-flask` (Fertilizing)
- And more...

### Managing Service Areas
Edit `_data/service-areas.yml`:
```yaml
north_fraser:
  title: "North Fraser Valley"
  description: "Comprehensive coverage..."
  areas:
    - name: "Chilliwack"
      featured: true
```

## 📱 Mobile Optimization

### Responsive Design
- **Mobile-first approach** - Designed for mobile, enhanced for desktop
- **Breakpoints:** 
  - Mobile: < 768px
  - Tablet: 768px - 1024px
  - Desktop: > 1024px
- **Touch-friendly:** 44px minimum touch targets
- **Performance:** Optimized images, lazy loading

### Mobile Features
- **Click-to-call:** Phone numbers are clickable links
- **Touch navigation:** Easy-to-use mobile menu
- **Form optimization:** Large input fields, appropriate keyboards
- **Fast loading:** Compressed images, minimal JavaScript

## 🔍 SEO & Performance

### SEO Features
- **Meta tags:** Title, description, keywords for each page
- **Schema markup:** Local business structured data
- **Semantic HTML:** Proper heading hierarchy, alt tags
- **Clean URLs:** Jekyll generates SEO-friendly URLs
- **Sitemap:** Automatically generated
- **Robots.txt:** Search engine directives

### Performance Optimizations
- **Static site generation:** Fast loading, no database queries
- **Image optimization:** Compressed and appropriately sized images
- **CSS optimization:** Single stylesheet, minimal unused CSS
- **JavaScript minimal:** Only essential functionality
- **CDN delivery:** GitHub Pages global CDN

## 🔧 Maintenance & Updates

### Regular Maintenance Tasks
- **Monthly:** Test contact forms
- **Quarterly:** Review service listings and pricing
- **Bi-annually:** Update testimonials and photos
- **Annually:** Review and update business information

### Content Updates
To update content:
1. **Services:** Edit `_data/services.yml`
2. **Service Areas:** Edit `_data/service-areas.yml`
3. **Owner Info:** Edit `_data/owner.yml`
4. **Pages:** Edit `index.html` or `services.html`
5. **Styles:** Edit `assets/css/style.css`

### Deployment Process
```bash
# 1. Make changes locally
git add .
git commit -m "Update [description]"

# 2. Test locally
bundle exec jekyll serve

# 3. Deploy to production
git push origin main

# 4. Verify deployment
# Check https://www.compasslawns.com
```

## 🚨 Troubleshooting

### Common Issues

**Site not updating after push:**
- Check GitHub Actions for build errors
- Verify CNAME file is present
- Clear browser cache

**Forms not working:**
- Verify FormSpree endpoint URL
- Check spam folder for notifications
- Test with different email address

**Local development issues:**
- Run `bundle update` to update dependencies
- Check Ruby version compatibility
- Clear Jekyll cache: `bundle exec jekyll clean`

### Debugging Commands
```bash
# Check Jekyll version
bundle exec jekyll --version

# Validate site structure
bundle exec jekyll doctor

# Build with verbose output
bundle exec jekyll build --verbose

# Check for liquid errors
bundle exec jekyll serve --trace
```

## 📊 Analytics & Monitoring

### Performance Monitoring
- **Page Load Speed:** Target < 3 seconds
- **Mobile Usability:** Google Mobile-Friendly Test
- **SEO Scores:** Google PageSpeed Insights
- **Form Submissions:** Monitor via FormSpree dashboard

### Suggested Analytics Setup
1. **Google Analytics 4:** Track visitor behavior
2. **Google Search Console:** Monitor search performance
3. **FormSpree Analytics:** Track form conversion rates

## 🔐 Security

### Security Measures
- **HTTPS:** Enforced via GitHub Pages
- **Form Security:** FormSpree spam protection
- **No Database:** Static site reduces attack surface
- **Regular Updates:** Dependencies updated via Dependabot

### Best Practices
- **Strong Passwords:** For all associated accounts
- **Two-Factor Authentication:** GitHub, FormSpree accounts
- **Regular Backups:** Git repository serves as backup
- **Access Control:** Limited repository access

## 📝 License & Rights

This website is custom-built for Compass Lawn Care & Maintenance. All content and design rights reserved.

**Copyright © 2024 Compass Lawn Care & Maintenance**

---

**Built with ❤️ for professional lawn care services in the Fraser Valley**

**Last Updated:** June 28, 2025.