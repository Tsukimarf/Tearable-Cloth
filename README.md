# 🎭 Random Joke Generator

A simple, elegant web application that fetches random jokes from popular joke APIs. Built with vanilla JavaScript, HTML, and CSS.

## ✨ Features

- **Dual API Support**: Choose between two popular joke APIs
  - [icanhazdadjoke](https://icanhazdadjoke.com/) - Dad jokes
  - [Official Joke API](https://official-joke-api.appspot.com/) - Setup/punchline jokes
- **Copy to Clipboard**: One-click copying of jokes
- **Auto-Fetch Mode**: Automatically fetch new jokes every 5 seconds
- **Keyboard Shortcut**: Press `Space` to fetch a new joke instantly
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **Modern UI**: Clean, gradient background with smooth animations

## 🚀 Getting Started

### Prerequisites

No dependencies or build tools required! Just a modern web browser.

### Installation

1. Clone or download this repository
2. Open `index.html` in your web browser
3. Start enjoying jokes!

```bash
# Clone the repository
git clone <repository-url>

# Navigate to the directory
cd random-joke-generator

# Open in browser (or use a local server)
open index.html
```

## 🎮 Usage

### Basic Usage

1. **Select an API** from the dropdown menu
2. **Click "Get Joke"** button or press `Space` on your keyboard
3. Enjoy the joke!

### Advanced Features

- **Copy Joke**: Click the 📋 Copy button to copy the joke to your clipboard
- **Auto Mode**: Click 🔄 Auto (5s) to automatically fetch new jokes every 5 seconds
  - Click again (⏹️ Stop Auto) to stop the automatic fetching
- **Keyboard Shortcut**: Press the `Space` bar anywhere on the page to fetch a new joke

## 🔧 Technical Details

### APIs Used

#### icanhazdadjoke API
- **Endpoint**: `https://icanhazdadjoke.com/`
- **Format**: Single-line dad jokes
- **Response**: `{ id, joke, status }`

#### Official Joke API
- **Endpoint**: `https://official-joke-api.appspot.com/random_joke`
- **Format**: Setup and punchline jokes
- **Response**: `{ id, type, setup, punchline }`

### Key Functions

```javascript
// Fetch joke from icanhazdadjoke
async function fetchIcanHazDadJoke()

// Fetch joke from Official Joke API
async function fetchOfficialJoke()

// Display joke in UI
function setJoke(primary, extra = '')

// Update status message
function showStatus(text, isError = false)

// Main function to fetch and display joke
async function getAndShowJoke()
```

### Browser Compatibility

- Chrome/Edge: ✅ Fully supported
- Firefox: ✅ Fully supported
- Safari: ✅ Fully supported
- Opera: ✅ Fully supported

**Requirements**: Modern browser with ES6+ support and Fetch API

## 📱 Responsive Design

The application is fully responsive and adapts to different screen sizes:

- **Desktop**: Full-width controls with side-by-side buttons
- **Mobile**: Stacked layout for better touch interaction
- **Tablet**: Optimized middle-ground layout

## 🎨 Customization

### Changing Colors

Edit the CSS variables in the `<style>` section:

```css
/* Primary gradient */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);

/* Accent color */
color: #667eea;
```

### Adjusting Auto-Fetch Interval

Change the interval in the event listener:

```javascript
autoInterval = setInterval(getAndShowJoke, 5000); // 5000ms = 5 seconds
```

## 🐛 Error Handling

The application includes comprehensive error handling:

- Network errors are caught and displayed
- Failed API requests show user-friendly error messages
- Clipboard operations handle permission issues gracefully

## 🤝 Contributing

Contributions are welcome! Here are some ways you can help:

- Report bugs
- Suggest new features
- Add support for additional joke APIs
- Improve UI/UX design
- Enhance accessibility

## 📄 License

This project is open source and available under the MIT License.

## 🙏 Acknowledgments

- [icanhazdadjoke](https://icanhazdadjoke.com/) for their excellent dad joke API
- [Official Joke API](https://github.com/15Dkatz/official_joke_api) for their setup/punchline joke API

## 📞 Support

If you encounter any issues or have questions:

1. Check the browser console for error messages
2. Ensure you have an active internet connection
3. Try refreshing the page
4. Test with a different browser

## 🔮 Future Enhancements

Potential features for future versions:

- [ ] Favorite jokes collection
- [ ] Share jokes on social media
- [ ] Dark mode toggle
- [ ] Custom joke categories
- [ ] Search functionality
- [ ] Joke rating system
- [ ] Multiple language support

---

**Enjoy the laughs! 😄**