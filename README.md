# SOC Events - Landing Page

A modern, GDPR-compliant landing page for SOC Events featuring dual navigation to professional event planning services and local Sound of Centuries events.

## 🌟 Features

### Core Features
- **Minimalist Design** - Clean, professional aesthetic with animated particle background
- **Dual Navigation** - Choose between event planning services or local SOC events
- **Responsive Design** - Optimized for desktop, tablet, and mobile devices
- **Dark/Light Mode Toggle** - User-controlled theme switching
- **GDPR Compliance** - Full cookie consent system with granular controls

### Technical Features
- **Google Analytics 4 Integration** - Conditional loading based on user consent
- **Traffic Tracking** - Comprehensive visitor and click tracking
- **SEO Optimized** - Meta tags, OpenGraph, and semantic HTML
- **Performance Optimized** - Minimal dependencies and fast loading

## 🚀 Quick Start

### Option 1: Direct HTML Hosting (Recommended)
The easiest way to deploy this landing page:

1. **Use the main file**: `final-landing-page.html`
2. **Upload to any web hosting service**
3. **Configure Google Analytics** (see setup below)

### Option 2: Development Environment
For local development or customization:

```bash
# Clone the repository
git clone https://github.com/TheManager94/soc-events.git
cd soc-events

# Install dependencies
bun install

# Start development server
bun run dev
```

## 📊 Google Analytics Setup

1. **Create Google Analytics Account**
   - Go to [Google Analytics](https://analytics.google.com)
   - Create a new property for your website
   - Get your Measurement ID (format: `G-XXXXXXXXXX`)

2. **Update the Landing Page**
   - Open `final-landing-page.html`
   - Find line 38 and 42: `G-XXXXXXXXXX`
   - Replace with your actual Measurement ID

3. **What You'll Track**
   - Page visits and unique visitors
   - Click events on both destination buttons
   - Geographic and device information
   - User behavior and engagement metrics

## 🔒 GDPR Compliance

The landing page includes a comprehensive cookie consent system that:

- **Appears automatically** for first-time visitors
- **Provides granular control** over cookie categories
- **Respects user choices** throughout their session
- **Blocks analytics** until explicit consent is given
- **Offers detailed explanations** of data usage

### Cookie Categories
- **Necessary Cookies**: Always active (basic functionality)
- **Analytics Cookies**: Optional (Google Analytics tracking)

## 📁 Project Structure

```
soc-events/
├── final-landing-page.html    # 🎯 Main production file
├── public/
│   └── index.html            # Alternative version
├── docs/
│   ├── analytics-guide.md    # Google Analytics setup guide
│   ├── gdpr-compliance-guide.md # GDPR compliance documentation
│   └── todos.md             # Project progress tracking
├── netlify.toml             # Netlify deployment configuration
├── package.json             # Development dependencies
└── README.md               # This file
```

## 🌐 Deployment Options

### Netlify (Recommended)
1. Connect this GitHub repository to Netlify
2. Set build command: `echo "Static site"`
3. Set publish directory: `/`
4. Deploy automatically on push

### Vercel
1. Import this repository to Vercel
2. Configure as static site
3. Deploy

### Traditional Web Hosting
1. Upload `final-landing-page.html` to your web server
2. Rename to `index.html` if needed
3. Ensure proper MIME types are configured

## 🎨 Customization

### Colors & Branding
- CSS custom properties are defined in the `<style>` section
- Modify the color scheme by updating CSS variables
- Replace the emoji favicon with a custom logo

### Content Updates
- Update destination URLs in the button click handlers
- Modify text content in the HTML structure
- Adjust meta tags for SEO optimization

### Analytics & Tracking
- See `docs/analytics-guide.md` for detailed tracking setup
- Configure additional tracking tools as needed
- Monitor GDPR compliance with consent tracking

## 📱 Browser Support

- **Modern Browsers**: Chrome, Firefox, Safari, Edge (latest versions)
- **Mobile Browsers**: iOS Safari, Chrome Mobile
- **Progressive Enhancement**: Core functionality works without JavaScript

## 🛠️ Development

### Available Scripts
```bash
bun run dev      # Start development server
bun run build    # Build for production
bun run lint     # Run linting
bun run format   # Format code
```

### Tech Stack
- **HTML5** with semantic markup
- **CSS3** with custom properties
- **Vanilla JavaScript** for interactions
- **Vite** for development tooling (optional)

## 📄 License

This project is private and proprietary to SOC Events.

## 🆘 Support

For technical support or questions about this landing page:
- Check the documentation in the `docs/` folder
- Review the analytics and GDPR compliance guides
- Contact the development team for customizations

---

**Ready to launch!** 🚀 Upload `final-landing-page.html` to your hosting provider and configure your Google Analytics ID.