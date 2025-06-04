# SOC Events Landing Page - Analytics & Tracking Guide

## 📊 **How the Traffic Tracking Works**

Your landing page now has **comprehensive traffic tracking** that monitors:
- **Page visits** (how many people visit)
- **Click tracking** (which links they click)
- **Visitor details** (where they come from, device info)

## 🔧 **Multiple Tracking Solutions Implemented**

### 1. **Google Analytics 4 (GA4) - Professional Solution**
- **Most Popular & Comprehensive**
- Tracks everything automatically
- Provides detailed reports and insights
- Free to use

**Setup Required:**
1. Go to [Google Analytics](https://analytics.google.com)
2. Create a free account
3. Get your Measurement ID (looks like `G-XXXXXXXXXX`)
4. Replace `G-XXXXXXXXXX` in the HTML file with your actual ID

**What You'll See:**
- Total visitors per day/week/month
- Which countries visitors come from
- What devices they use (mobile/desktop)
- How long they stay on your page
- Click events for both destination links

### 2. **Built-in Local Tracking (Already Working)**
- **No setup required** - works immediately
- Stores data in browser's local storage
- Basic but effective for testing

**To View Current Data:**
1. Open your landing page
2. Press `F12` (open browser developer tools)
3. Go to `Console` tab
4. Type: `localStorage.getItem('landing_page_analytics')`
5. You'll see all tracked visits and clicks

### 3. **Alternative: Plausible Analytics (Privacy-Focused)**
- **GDPR-friendly** alternative to Google Analytics
- No cookies required
- Simple setup and beautiful dashboard
- $9/month for up to 10k page views

**Setup:**
1. Go to [Plausible.io](https://plausible.io)
2. Add your domain
3. Get the tracking script
4. Replace the Google Analytics section with Plausible script

## 🎯 **What Gets Tracked Automatically**

### Page Visits
- **Timestamp** of each visit
- **Page URL** visited
- **Referrer** (where visitor came from)
- **User Agent** (browser/device info)

### Click Events
- **Button clicked** ("Event Planning" or "Local Events")
- **Click timestamp**
- **User session** (to track user journey)

### Traffic Sources
- **Direct traffic** (typed URL directly)
- **Social media** (Facebook, Instagram, etc.)
- **Search engines** (Google, Bing, etc.)
- **Referral sites** (other websites linking to you)

## 📈 **Reading Your Analytics Data**

### Google Analytics Dashboard
Once set up, you'll see:
- **Real-time visitors** currently on your site
- **Daily/weekly/monthly** visitor trends
- **Top traffic sources** bringing you visitors
- **Device breakdown** (mobile vs desktop)
- **Geographic data** (which countries/cities)

### Key Metrics to Watch
1. **Unique Visitors** - how many different people visited
2. **Page Views** - total number of page loads
3. **Bounce Rate** - % of people who left immediately
4. **Click-through Rate** - % who clicked your buttons
5. **Traffic Sources** - where your visitors come from

## 🔧 **Advanced Setup Options**

### Custom Event Tracking
The page already tracks button clicks, but you can add more:
```javascript
// Track custom events
gtag('event', 'custom_action', {
  'event_category': 'engagement',
  'event_label': 'specific_action'
});
```

### Enhanced E-commerce (Future)
If you add booking/payment functionality later:
```javascript
// Track conversions
gtag('event', 'purchase', {
  'transaction_id': '12345',
  'value': 1.00,
  'currency': 'EUR'
});
```

## 📊 **Quick Analytics Checklist**

- ✅ **Google Analytics account created**
- ✅ **Measurement ID added to HTML file**
- ✅ **GDPR consent system active**
- ✅ **Click tracking working**
- ✅ **Real-time data flowing**

## 🛠️ **Troubleshooting**

### "No data showing in Google Analytics"
1. **Check your Measurement ID** - make sure it's correct
2. **Wait 24-48 hours** - data can take time to appear
3. **Test in incognito mode** - to avoid your own visits
4. **Check GDPR consent** - analytics only loads after consent

### "Tracking seems slow"
1. **Real-time reports** show data immediately
2. **Standard reports** update every 24 hours
3. **Use real-time tab** in Google Analytics for immediate feedback

## 🎯 **Pro Tips**

1. **Exclude your own visits** - set up internal traffic filters
2. **Set up goals** - track when people click your buttons as conversions
3. **Weekly reports** - check your analytics every Monday
4. **Mobile-first** - most traffic will likely be mobile
5. **Privacy compliance** - your GDPR system handles this automatically

---

**Your landing page is now fully tracked and ready to provide valuable insights about your visitors!** 📈