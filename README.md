# TikTok Downloader - Download TikTok Videos & Images Without Watermark

A fast, responsive, and easy-to-use TikTok downloader web application that allows you to download TikTok videos without watermark, images, and audio in high quality.

## 🌟 Features

- **Download Videos Without Watermark** - Get TikTok videos in HD and standard quality without watermark
- **Download TikTok Images** - Download all images from TikTok photo posts in a gallery view
- **Extract Audio** - Download MP3 audio from any TikTok video
- **Video with Watermark** - Option to download original video with TikTok watermark
- **User Information Display** - Shows author profile, username, and statistics (views, likes, comments, shares)
- **Fully Responsive** - Optimized for desktop, tablet, and mobile devices
- **Dark Theme UI** - Beautiful dark mode interface with smooth animations
- **No Registration Required** - Completely free to use without any signup

## 🚀 Demo
Visit the live demo: [TikTok Downloader](https://tiktok.botzaku.eu.org)

## 📸 Screenshots
![Screenshot](https://cdn.botzaku.eu.org/119dj5yes1-Zu4-Jg7yeBe8Q0-GM334PC)

### Desktop View
- Clean and modern interface
- Easy-to-use download options
- Video/Image preview with metadata

### Mobile View
- Responsive design
- Touch-friendly buttons
- Hamburger menu navigation

## 🛠️ Technologies Used

- **HTML5** - Semantic markup
- **CSS3** - Modern styling with flexbox and grid
- **JavaScript (ES6+)** - Async/await, fetch API
- **Bootstrap Icons** - Icon library
- **SweetAlert2** - Beautiful alert notifications
- **BotzApi** - Backend API for TikTok content fetching

## 📋 API Integration

This application uses the BotzApi TikTok downloader endpoint:

```javascript
GET https://host.optikl.ink/download/tiktok?url={TIKTOK_URL}
```

### API Response Structure

#### Video Response
```json
{
  "creator": "@PaxSenix",
  "ok": true,
  "message": "Hope you guys love my hard work :3",
  "detail": {
    "type": "video",
    "author": "username",
    "authorProfile": "https://.. .",
    "authorUsername": "username",
    "authorProfileLink": "https://...",
    "description": "Video description",
    "cover": "https://...",
    "view": 787287,
    "like": 60943,
    "comment": 1189,
    "share": 7871
  },
  "downloadUrls": {
    "music": "https://...",
    "images": [],
    "video": "https://...",
    "video_standard": "https://...",
    "video_wm": "https://..."
  }
}
```

#### Image Response
```json
{
  "creator": "@PaxSenix",
  "ok": true,
  "message": "Hope you guys love my hard work :3",
  "detail": {
    "type": "image",
    "author": "username",
    "authorProfile": "https://...",
    "authorUsername": "username",
    "authorProfileLink": "https://.. .",
    "description": "Image description",
    "cover": "https://...",
    "view": 2625773,
    "like": 217371,
    "comment": 15394,
    "share": 43917
  },
  "downloadUrls": {
    "music": "https://...",
    "images": [
      "https://image1.jpg",
      "https://image2.jpg",
      "https://image3.jpg"
    ],
    "video": null,
    "video_standard": null,
    "video_wm": null
  }
}
```

## 🎯 How to Use

1. **Copy TikTok URL**
   - Open TikTok app or website
   - Find the video or image post you want to download
   - Copy the share link

2. **Paste URL**
   - Paste the TikTok URL into the input field
   - Click the "Download" button

3. **Choose Download Option**
   - For videos: Choose between HD, Standard, or With Watermark
   - For images: Click download button on each image in the gallery
   - For audio: Click "Download Audio" button

4. **Download Complete**
   - Files will be automatically downloaded to your device
   - Use "Download Another" button to download more content

## 💻 Installation

### Local Development

1. Clone the repository:
```bash
git clone https://github. com/BotzIky/TikBotz-TikTok-Downloader-Website.git
cd TikBotz-TikTok-Downloader-Website
```

2.  Open `index.html` in your browser:
```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx http-server

# Or simply open the file
open index.html
```

3. Navigate to `http://localhost:8000` in your browser

### Deploy to GitHub Pages

1. Push your code to GitHub repository
2. Go to repository Settings > Pages
3. Select branch `main` and folder `/ (root)`
4. Click Save
5. Your site will be live at `https://yourusername.github.io/TikBotz-TikTok-Downloader-Website`

### Deploy to Vercel

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel
```

### Deploy to Netlify

1.  Drag and drop your project folder to Netlify
2. Or connect your GitHub repository
3. Deploy automatically

## 🔧 Configuration

### Change API Endpoint

Edit the API URL in the JavaScript section:

```javascript
const apiUrl = 'https://host.optikl.ink/download/tiktok?url=' + encodeURIComponent(url);
```

### Customize Colors

Edit the CSS variables:

```css
/* Primary color - green */
--primary-color: #98ff98;

/* Secondary color - dark green */
--secondary-color: #7ae87a;

/* Background color */
--bg-color: #000;

/* Text color */
--text-color: #f1fdf1;
```

## 📱 Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Opera (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile, Samsung Internet)

## ⚠️ Legal Disclaimer

This tool is provided for **personal use only**. Please ensure you have the rights to download and use any content.  Respect copyright laws and TikTok's terms of service.  

- Do not use downloaded content for commercial purposes without permission
- Always credit the original creator
- Respect intellectual property rights

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 🐛 Bug Reports

If you find any bugs, please create an issue on GitHub with:
- Description of the bug
- Steps to reproduce
- Expected behavior
- Screenshots (if applicable)
- Browser and OS information

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. 

## 👨‍💻 Author

**BotzAku (Riski Yanda)**
- Website: <https://botzaku.eu.org>
- Instagram: [@botzaku](https://instagram.com/botzaku)
- TikTok: [@botzaku](https://tiktok.com/@botzaku)
- Twitter: [@botz_aku](https://twitter.com/botz_aku)
- Telegram: [BotzAku](https://t.me/BotzAku)
- WhatsApp: [Channel](https://whatsapp.com/channel/0029VbBjxQl8qIzmg51J5W3x)
- Discord: [Server](https://discord.gg/Ehr7DrsU)

## 🙏 Acknowledgments

- [Paxsenix0](https://github.com/Paxsenix0) for providing the TikTok download API
- [Bootstrap Icons](https://icons.getbootstrap.com/) for beautiful icons
- [SweetAlert2](https://sweetalert2.github.io/) for elegant alerts
- All contributors and users of this project

## ⭐ Star History

If you find this project useful, please consider giving it a star on GitHub! 

---

Made with ❤️ by [BotzAku](https://botzaku.eu.org)

**Disclaimer**: This is an unofficial tool and is not affiliated with TikTok or ByteDance. 
