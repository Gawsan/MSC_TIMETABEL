# MSC Timetable - Personal Class Schedule Manager

A beautiful, interactive timetable application for managing your MSC (Master of Science in Computer Science) class schedule. Features dark theme, reminder notifications, calendar integration, and Zoom meeting links.

## 🌟 Features

- **Interactive Schedule Display**: View all your classes in an elegant card-based layout
- **Smart Reminders**: Set custom notification alerts before each class
- **Calendar Integration**: One-click Google Calendar event creation
- **Zoom Integration**: Direct links to join online classes
- **Responsive Design**: Works perfectly on desktop, tablet, and mobile
- **Dark Theme**: Beautiful gradient background with smooth animations
- **Local Storage**: Remembers your reminder preferences
- **Semester Timeline**: Automatically tracks semester dates and class occurrences

## 🚀 How to Host This Page

### Option 1: GitHub Pages (Free & Recommended)

This repository is already configured for GitHub Pages deployment! Here's how to enable it:

1. **Enable GitHub Pages**:
   - Go to your repository on GitHub
   - Click on "Settings" tab
   - Scroll down to "Pages" section
   - Under "Source", select "GitHub Actions"
   - The workflow will automatically deploy your site

2. **Access Your Live Site**:
   - Your site will be available at: `https://yourusername.github.io/MSC_TIMETABEL`
   - It may take a few minutes for the first deployment

3. **Auto-Deployment**:
   - Every time you push changes to the `main` branch, your site will automatically update
   - Check the "Actions" tab to see deployment status

### Option 2: Netlify (Free with Custom Domain)

1. **Deploy to Netlify**:
   - Visit [netlify.com](https://netlify.com)
   - Click "Add new site" → "Import an existing project"
   - Connect your GitHub account and select this repository
   - Build settings: Leave default (no build required for static HTML)
   - Click "Deploy site"

2. **Custom Domain** (Optional):
   - In Netlify dashboard, go to "Domain settings"
   - Add your custom domain
   - Follow DNS configuration instructions

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/Gawsan/MSC_TIMETABEL)

### Option 3: Vercel (Free with Excellent Performance)

1. **Deploy to Vercel**:
   - Visit [vercel.com](https://vercel.com)
   - Click "New Project"
   - Import your GitHub repository
   - Click "Deploy"

2. **Custom Domain** (Optional):
   - In Vercel dashboard, go to project settings
   - Add your custom domain

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/Gawsan/MSC_TIMETABEL)

### Option 4: Local Development Server

For testing and development:

```bash
# Clone the repository
git clone https://github.com/Gawsan/MSC_TIMETABEL.git
cd MSC_TIMETABEL

# Serve locally using Python
python -m http.server 8000

# Or using Node.js
npx serve .

# Or using PHP
php -S localhost:8000
```

Then open `http://localhost:8000` in your browser.

## 📱 Browser Compatibility

- **Chrome/Edge**: Full support (recommended)
- **Firefox**: Full support
- **Safari**: Full support
- **Mobile browsers**: Responsive design optimized for all screen sizes

## ⚙️ Customization

### Updating Your Class Schedule

Edit the `classes` array in `index.html` (around line 446):

```javascript
const classes = [
  {
    id: "CS5213",
    day: "Saturday",
    start: "08:00",
    end: "10:30",
    code: "CS5213",
    title: "Enterprise Software Architecture",
    lecturer: "Prof. Indika Perera",
    zoom: null,
  },
  // Add your classes here...
];
```

### Updating Semester Dates

Modify the semester timeline (around line 442):

```javascript
const SEMESTER_START = new Date("2025-09-06T00:00:00");
const SEMESTER_END = new Date("2025-11-22T23:59:59");
```

### Customizing Appearance

The CSS variables at the top of the `<style>` section can be modified to change colors and spacing:

```css
:root {
  --bg: #0b1220;        /* Background color */
  --card: #0f172a;      /* Card background */
  --brand: #38bdf8;     /* Primary brand color */
  --brand-2: #818cf8;   /* Secondary brand color */
  /* ... more variables */
}
```

## 🔔 Notification Features

- **Browser Notifications**: Get desktop notifications before classes start
- **Audio Alerts**: Optional sound notification
- **Customizable Timing**: Set alerts 5-60 minutes before class
- **Persistent Settings**: Your preferences are saved locally

## 📊 Technical Features

- **Progressive Web App Ready**: Can be installed on mobile devices
- **Offline Capable**: Works without internet after first load
- **Performance Optimized**: Fast loading with minimal dependencies
- **SEO Friendly**: Proper meta tags and semantic HTML

## 🛠️ Troubleshooting

### GitHub Pages Not Working?

1. Check if GitHub Pages is enabled in repository Settings → Pages
2. Ensure the workflow file `.github/workflows/static.yml` exists
3. Check the "Actions" tab for any deployment errors
4. Make sure you're pushing to the `main` branch

### Notifications Not Working?

1. Allow notifications when prompted by your browser
2. Check browser notification settings
3. Ensure the page is served over HTTPS (required for notifications)

### Calendar Integration Issues?

- Google Calendar links work with any Google account
- Links open the Google Calendar event creation page
- Make sure popup blockers aren't preventing the calendar from opening

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Feel free to:
- Fork this repository
- Submit issues and feature requests
- Create pull requests for improvements
- Share with fellow students

## 📞 Contact

- GitHub: [@Gawsan](https://github.com/Gawsan)
- Repository: [MSC_TIMETABEL](https://github.com/Gawsan/MSC_TIMETABEL)

---

**Note**: This timetable is specifically designed for MSC Computer Science students. Feel free to adapt it for your own schedule and requirements!