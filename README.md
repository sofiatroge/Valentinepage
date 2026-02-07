# 💕 Valentine's Day Interactive Page

A beautiful, animated Valentine's Day proposal page with Discord webhook integration to track responses in real-time!

## 🎯 Features

- **Beautiful Animations**: Floating hearts, smooth transitions, and a heartbeat effect
- **Interactive Buttons**: "Yes" and "Let me think..." options with fun interactions
- **Discord Notifications**: Get real-time notifications when someone opens the page or clicks a button
- **Confetti Celebration**: Animated confetti when they say yes!
- **Growing "Yes" Button**: The "Yes" button gets bigger each time they click "Let me think..."
- **Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **Custom Messages**: Personalized messages that change as they hesitate

## 🚀 Quick Start

### 1. Set Up Discord Webhook

1. Go to your Discord server
2. Navigate to **Server Settings** → **Integrations** → **Webhooks**
3. Click **New Webhook** or **Create Webhook**
4. Give it a name (e.g., "Valentine Tracker 💕")
5. Select the channel where you want notifications
6. Click **Copy Webhook URL**
7. Extract the webhook ID and token from the URL:
   ```
   https://discord.com/api/webhooks/WEBHOOK_ID/WEBHOOK_TOKEN
   ```

### 2. Update the Code

Open the HTML file and replace these values in the JavaScript section:

```javascript
const WEBHOOK_ID = 'YOUR_WEBHOOK_ID_HERE';
const WEBHOOK_TOKEN = 'YOUR_WEBHOOK_TOKEN_HERE';
```

### 3. Customize the Content

Update the message to make it personal:

```html
<h1>Hello bebe!</h1>
<p class="subtitle">I have something to ask you...👉👈</p>
<p class="message">
    You make every day brighter, every moment so sweet,
    My heart overflows every time that we meet.
    So this Valentine's Day, I'll ask you once more:
    Will you be my Valentine, for the fourth time in a row? 🥰
</p>
```

### 4. Deploy

Upload the HTML file to any web hosting service:
- **GitHub Pages** (free)
- **Netlify** (free)
- **Vercel** (free)
- **Your own web server**

## 📱 How It Works

### Discord Notifications

The page sends three types of notifications to your Discord channel:

1. **Page Opened**: When someone loads the page
   ```
   💕 Someone opened the Valentine page! (Feb 6, 9:20 PM)
   ```

2. **"Yes" Clicked**: When they accept
   ```
   🎉 HE SAID YES!!! 💕💕💕 (Feb 6, 9:21 PM) Time to celebrate! 🥳
   ```

3. **"Let me think..." Clicked**: When they hesitate
   ```
   💔 He clicked No button - Attempt 1 (Feb 6, 9:20 PM)
   ```

### Button Interactions

- **"Yes" button**: Triggers confetti animation and shows celebration message
- **"Let me think..." button**: 
  - Changes text with persuasive messages
  - Makes the "Yes" button grow larger with each click
  - Tracks the number of attempts

### Persuasive Messages

Each time they click "Let me think...", the button text changes:
1. "Are you sure? 🫣"
2. "Pretty please? 🥺"
3. "Think about all our good times! 💖"
4. "I promise to be the best valentine! 🥹"
5. "You know you want to say yes... 😉"
6. "Excuse me 😭"

After the 6th click, the button just shakes!

## 🎨 Customization

### Colors

The page uses CSS custom properties (variables) for easy color customization:

```css
:root {
    --primary: #ff6b9d;      /* Main pink color */
    --secondary: #c06c84;    /* Darker pink */
    --accent: #ffa8b8;       /* Light pink */
    --light: #fff0f3;        /* Very light pink */
    --white: #ffffff;        /* White */
}
```

### Fonts

The page uses Google Fonts:
- **Pacifico**: For headings (romantic, handwritten style)
- **Quicksand**: For body text (clean, modern)

To change fonts, update the Google Fonts link and CSS:

```html
<link href="https://fonts.googleapis.com/css2?family=YourFont&display=swap" rel="stylesheet">
```

### Animations

All animations can be adjusted:
- **Float animation**: Controls floating hearts (15 seconds by default)
- **Heartbeat**: Controls the main heart pulse (1.5 seconds)
- **Confetti**: Controls celebration confetti (3 seconds fall time)

## 🛠️ Technical Details

### Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Animations, gradients, flexbox
- **JavaScript (ES6+)**: Async/await, fetch API
- **Discord Webhook API**: Real-time notifications

### Browser Compatibility

Works on all modern browsers:
- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers

## 🐛 Troubleshooting

### Discord Webhook Not Working

1. **Check webhook is active**: Go to Discord → Server Settings → Integrations → Webhooks
2. **Verify ID and token**: Make sure you copied them correctly (they're case-sensitive)
3. **Check browser console**: Press F12 and look for error messages
4. **Look for 400 errors**: This usually means the webhook format is wrong
5. **Test with the debug tool**: Use the included debug HTML file


## 📝 Privacy & Security

⚠️ **Important Security Notes:**

1. **Webhook tokens are sensitive**: Anyone with your webhook URL can send messages to your Discord channel
2. **Don't share your webhook**: Keep the WEBHOOK_ID and WEBHOOK_TOKEN private
3. **Regenerate if exposed**: If you accidentally share your webhook, regenerate it in Discord settings
4. **Client-side only**: This page runs entirely in the browser - the webhook token is visible in the source code

### Best Practices

- Only share the page URL, not the source code
- If hosting publicly, consider using a backend proxy to hide the webhook
- Regularly check your Discord webhook settings
- Delete the webhook after Valentine's Day if you won't use it again

## 🙏 Credits

Created with love using:
- Google Fonts (Pacifico & Quicksand)
- Discord Webhook API
- Pure CSS animations
- Lots of hearts! ♥️


**Made with 💕 for someone special**

*P.S. - Good luck with your Valentine's proposal! 😊*
