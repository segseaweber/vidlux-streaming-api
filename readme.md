# VidLux - Premium Video Streaming API

<div align="center">

**Lightning-fast, ad-free video streaming API for movies and TV shows**

[![Next.js](https://img.shields.io/badge/Next.js-14.2.16-black?logo=next.js)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue?logo=typescript)](https://www.typescriptlang.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![API Status](https://img.shields.io/badge/API-Live-success)](https://vidlux.site)

[Website](https://vidlux.site) • [Documentation](https://vidlux.site/docs) • [Dashboard](https://vidlux.site/dashboard) • [API Demo](https://vidlux.site/embed/movie/603692)

</div>

---

## 🚀 What is VidLux?

VidLux is a powerful, embeddable video streaming API designed for developers who want to integrate high-quality movie and TV show streaming into their applications. Built with Next.js and TypeScript, VidLux offers a seamless, ad-free experience for premium users while supporting multiple extraction sources for maximum reliability.

### ✨ Key Features

- 🎬 **Extensive Library** - Access to thousands of movies and TV shows via TMDB integration
- 🔒 **Secure API** - AES-256 encryption, domain whitelisting, and rate limiting
- 🎨 **Customizable Player** - Brand with your logo, colors, and custom UI
- 📊 **Usage Analytics** - Track views, bandwidth, and API consumption
- 💰 **Flexible Pricing** - Free tier available, pay for what you use
- ⚡ **Multiple Servers** - 5+ extraction sources with automatic failover
- 📱 **Responsive Design** - Works seamlessly on desktop, tablet, and mobile
- 🌍 **Multi-Language Subtitles** - Support for 15+ languages
- 🎯 **Quality Selection** - Auto-adaptive HLS and manual MP4 quality switching
- 🔄 **Resume Playback** - Automatic progress tracking and resume functionality

---

## 🎯 Use Cases

- **Movie Streaming Websites** - Embed VidLux player directly into your site
- **Mobile Apps** - Integrate via API for iOS/Android applications
- **Smart TV Apps** - Build streaming apps for Smart TVs and streaming devices
- **Educational Platforms** - Host video content with custom branding
- **Media Aggregators** - Combine multiple content sources
- **Discord/Telegram Bots** - Provide streaming links via bot commands

---

## 🎥 Live Demo

Try VidLux in action with our interactive embed examples:

**Movie Example:**
```html
<iframe 
  src="https://vidlux.site/embed/movie/603692?key=YOUR_API_KEY&color=3b82f6&logo=YOUR_LOGO_URL" 
  width="100%" 
  height="500" 
  frameborder="0" 
  allowfullscreen>
</iframe>
```

**TV Show Example:**
```html
<iframe 
  src="https://vidlux.site/embed/tv/1399/1/1?key=YOUR_API_KEY" 
  width="100%" 
  height="500" 
  frameborder="0" 
  allowfullscreen>
</iframe>
```

---

## 🔧 Quick Start

### 1. Get Your API Key

Visit [vidlux.site/register](https://vidlux.site/register) to create a free account and generate your API key.

### 2. Whitelist Your Domain

Add your domain to the whitelist in your [dashboard](https://vidlux.site/dashboard/domains) to authorize API requests.



---

## 📚 API Documentation

### Embed URLs

#### Movie Embed
```
https://vidlux.site/embed/movie/{TMDB_ID}?key={API_KEY}
```

#### TV Show Embed
```
https://vidlux.site/embed/tv/{TMDB_ID}/{SEASON}/{EPISODE}?key={API_KEY}
```

### URL Parameters

| Parameter | Type | Required | Description |
|-----------|------|----------|-------------|
| `key` | string | Yes | Your API key |
| `color` | hex | No | Primary color (e.g., `ff0000`) |
| `autoplay` | boolean | No | Auto-play video (default: `true`) |
| `server` | boolean | No | Show server selector (default: `true`) |

### API Endpoints



**Available Servers:**
- `ALpha` - Alpha Server (HLS)
- `Nova` - Nova Server (HLS)
- `astra` - Astra Server (HLS)
- `flix` - Flix Server (HLS)
- `Delta` - Delta Server (MP4)
- `Omega` - Omega Server (HLS)

#### Get Subtitles
```http
GET /api/subtitles?id={TMDB_ID}&type=movie
```

#### Get TMDB Metadata
```http
GET /api/tmdb?id={TMDB_ID}&type=movie
```

---

## 🛡️ Security Features

- **AES-256 Encryption** - All API responses are encrypted
- **Domain Whitelisting** - Restrict API usage to authorized domains
- **Rate Limiting** - Prevent abuse with configurable rate limits
- **IP Tracking** - Monitor and block suspicious activity
- **CORS Protection** - Secure cross-origin requests
- **Anti-Scraping** - Built-in protection against automated scraping

---

## 💎 Pricing Plans

### Free Tier
- ✅ 1,000 views/month
- ✅ Single domain
- ✅ Community support
- ❌ Custom branding
- ❌ Ad-free experience

### Premium ($19/month)
- ✅ 50,000 views/month
- ✅ 5 domains
- ✅ Custom logo & colors
- ✅ Ad-free player
- ✅ Priority support
- ✅ Usage analytics

### Enterprise (Custom)
- ✅ Unlimited views
- ✅ Unlimited domains
- ✅ Dedicated servers
- ✅ SLA guarantee
- ✅ 24/7 support
- ✅ Custom features

[View Pricing Details →](https://vidlux.site/dashboard/payment)

---

## 🏗️ Technology Stack

- **Framework:** Next.js 14 (App Router)
- **Language:** TypeScript
- **Styling:** Tailwind CSS + shadcn/ui
- **Video Player:** HLS.js + Custom React Player
- **Database:** Supabase (PostgreSQL)
- **Authentication:** Supabase Auth
- **Analytics:** Custom Analytics Engine
- **API Security:** AES-256 Encryption
- **Hosting:** Vercel / Self-hosted VPS

---

## 🔥 Features in Detail

### Smart Failover System
VidLux automatically switches between 5+ extraction servers if one fails, ensuring 99.9% uptime.

### Adaptive Streaming
- HLS for automatic quality adjustment based on bandwidth
- MP4 with manual quality selection (360p - 1080p)
- Bandwidth-aware buffering

### Custom Branding
- Upload your logo
- Choose primary color
- Hide VidLux watermark (premium)

### Resume Playback
- Automatic progress tracking
- Cross-device synchronization
- Watch history management

### Multi-Language Support
- 15+ subtitle languages
- Automatic language detection
- Custom subtitle styling

---

## 📊 Use Cases & Success Stories

### 🎬 StreamFlix (Movie Streaming Site)
> "VidLux helped us launch our streaming platform in just 2 weeks. The API is incredibly reliable and the custom branding made it feel like our own player." - John D.

### 📱 CinemaBot (Discord Bot)
> "We serve 50,000+ users daily with VidLux. The automatic failover means our bot never goes down." - Sarah M.

### 🌍 GlobalWatch (International Platform)
> "Multi-language subtitle support was crucial for our international audience. VidLux delivered perfectly." - Ahmed K.

---

## 🚦 Getting Started Guide

### Step 1: Sign Up
1. Visit [vidlux.site/register](https://vidlux.site/register)
2. Create your account with email verification
3. Complete your profile

### Step 2: Generate API Key
1. Go to [Dashboard](https://vidlux.site/dashboard/settings)
2. Click "Generate New Key"
3. Copy your API key (keep it secure!)

### Step 3: Configure Domains
1. Navigate to [Domains](https://vidlux.site/dashboard/domains)
2. Add your website domain
3. Wait for verification (instant)

### Step 4: Test Integration
1. Use our [Embed Examples](https://vidlux.site/docs)
2. Customize parameters (color, logo, etc.)
3. Test on your website

### Step 5: Go Live
1. Monitor usage in [Analytics](https://vidlux.site/dashboard/usage)
2. Upgrade plan if needed
3. Contact support for assistance

---

## 🤝 Community & Support

- **Documentation:** [vidlux.site/docs](https://vidlux.site/docs)
- **Support Tickets:** [vidlux.site/dashboard/support](https://vidlux.site/dashboard/support)
- **GitHub Issues:** [github.com/vidlux/issues](https://github.com/segseaweber/vidlux/issues)
- **Email:** support@vidlux.site

---

## 📈 Roadmap

- [x] Multi-server extraction
- [x] Custom branding
- [x] Analytics dashboard
- [x] Resume playback
- [x] MP4 quality selection
- [ ] Download API
- [ ] Chromecast support
- [ ] Offline viewing
- [ ] Playlist management
- [ ] Live TV streams

---

## 🔐 API Rate Limits

| Plan | Requests/Hour | Concurrent Streams |
|------|---------------|-------------------|
| Free | 100 | 1 |
| Premium | 1,000 | 10 |
| Enterprise | Unlimited | Unlimited |

---

## 🌟 Why Choose VidLux?

✅ **Reliable** - 99.9% uptime with automatic failover  
✅ **Fast** - Global CDN with <100ms latency  
✅ **Secure** - Enterprise-grade encryption and protection  
✅ **Affordable** - Competitive pricing with free tier  
✅ **Developer-Friendly** - Clean API, extensive documentation  
✅ **Customizable** - Full white-label capabilities  
✅ **Scalable** - From hobby projects to enterprise platforms  

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## ⚠️ Disclaimer

VidLux is a streaming API aggregator. We do not host or store any video content. All streams are sourced from third-party providers. Users are responsible for complying with copyright laws in their jurisdiction.

---

## 🙏 Acknowledgments

- [TMDB](https://www.themoviedb.org/) for movie/TV metadata
- [HLS.js](https://github.com/video-dev/hls.js/) for HLS playback
- [shadcn/ui](https://ui.shadcn.com/) for beautiful components
- [Supabase](https://supabase.com/) for backend infrastructure

---

<div align="center">

**Made with ❤️ by the VidLux Team**

[Website](https://vidlux.site) • [Docs](https://vidlux.site/docs) • [Dashboard](https://vidlux.site/dashboard) • [Support](https://vidlux.site/dashboard/support)

</div>
