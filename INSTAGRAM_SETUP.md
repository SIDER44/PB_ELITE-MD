# 📸 Instagram Commands Setup Guide

## Quick Start - Android

### Option 1: Auto-Setup (Easiest)

1. In WhatsApp with your bot, send:
   ```
   .getiscookie
   ```

2. You'll see 3 options. Pick **Option 1** and visit the link shown in your browser

3. Login to Instagram on that page, it auto-shows your cookies

4. Copy the cookie string and send back to the bot:
   ```
   .setiscookie <paste-cookie-here>
   ```

5. Bot restarts automatically, you're done! ✅

---

### Option 2: Manual Extract (If Option 1 doesn't work)

**From Chrome/Kiwi Browser:**
1. Open `instagram.com` and log in
2. Press `F12` → Console tab
3. Paste this and press Enter:
   ```javascript
   copy(document.cookie)
   ```
4. Send to bot:
   ```
   .setiscookie <paste-here>
   ```

---

## Commands

### `.getiscookie`
Shows detailed guide with 3 extraction methods

### `.setiscookie <cookie-string>`
Saves your cookies (owner only)
- Automatically reloads the bot
- Cookie badge 🔐 appears in `.ig` responses once active

### `.ig <instagram-link>`
Download Instagram reel/photo with full metadata
- Works on public posts without cookies
- Works on private posts you follow WITH cookies

---

## What Cookies Do

✅ **With cookies:**
- Download private posts you follow
- Download your own videos
- See accurate like/view/comment counts
- Access carousel photos
- Better reliability overall

❌ **Without cookies:**
- Public posts only
- Some stats show "N/A"
- May hit rate limits faster

---

## Security Notes

🔒 Your cookies are:
- Stored **locally in your `.env` file** (not cloud)
- Only used by **your own bot**
- Never sent anywhere except Instagram
- Session-based (expire after ~90 days, auto-extend with use)

⚠️ Never share your cookie string with anyone!

---

## Troubleshooting

**"No cookies found"**
→ Make sure you're logged into Instagram on that browser/page

**"Post may be private"**
→ Add your cookies and try again. If still fails, the post is truly private.

**"Error: .env file not found"**
→ The bot folder doesn't have an `.env` file. Create one with:
```
PAIRING_NUMBER=
PREFIX=.
BOT_NAME=ELITE-MD
IG_COOKIES=
```

---

Happy downloading! 🎬
