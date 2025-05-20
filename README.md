Here's the complete content ready to paste directly into your **`README.md`** file:

````markdown
# SmartPopunder.js

A lightweight JavaScript library designed to create and manage popunder windows or tabs, allowing URLs to open discreetly in the background of the user's browser.

## 🚀 How It Works

`SmartPopunder.js` enables your website to open a URL behind the currently active browser window or tab (commonly known as a "popunder"). It's particularly useful for advertising and increasing user engagement without interrupting user activity.

## ⚙️ Installation

### Include Directly in HTML

Include the JavaScript file directly into your HTML page:

```html
<script src="smartpopunder.js"></script>
````

Alternatively, embed directly into your HTML page:

```html
<script>
  /* Paste smartpopunder.js content here */
</script>
```

## 🚩 Usage Example

Basic usage:

```javascript
// URL to open as popunder
var popunderURL = "https://example.com";

// Activate popunder with default settings
SmartPopunder.make(popunderURL);
```

Customizable options example:

```javascript
var popunderURL = "https://example.com"; // replace with your URL

// Custom options
var popunderOptions = {
    newTab: true,       // Open in new tab (true) or new window (false)
    blur: true,         // Keep popunder in background
    cookieExpires: 60,  // Prevent repeated popunder for user (in minutes)
    cookiePath: '/',    // Cookie path
    chromeDelay: 500,   // Delay in ms to prevent Chrome popunder blocking
    blurByAlert: false, // Optional: trigger alert to keep popunder hidden
    smart: false,       // Optional: enable advanced mouse tracking

    beforeOpen: function(){
        console.log('Popunder about to open.');
    },

    afterOpen: function(){
        console.log('Popunder successfully opened.');
    }
};

// Activate popunder with custom settings
SmartPopunder.make(popunderURL, popunderOptions);

// Or you can go with the Default Config values mentioned below!
SmartPopunder.make(popunderURL);
```

## 📌 Configuration Options

| Option          | Description                                                                    | Default Value  |
| --------------- | ------------------------------------------------------------------------------ | -------------- |
| `newTab`        | Open popunder in new tab or new window.                                        | `true`         |
| `blur`          | Ensure popunder opens behind the active tab/window.                            | `true`         |
| `cookieExpires` | Minutes to wait before allowing another popunder.                              | `60*12`           |
| `cookiePath`    | Path for the cookie used to track popunder execution.                          | `'/'`          |
| `chromeDelay`   | Chrome-specific delay (ms) to avoid popunder blocks.                           | `500`          |
| `blurByAlert`   | Optionally use alert dialog to force popunder to background (rarely required). | `false`        |
| `smart`         | Enable dynamic mouse tracking for advanced popunder triggering.                | `false`        |
| `beforeOpen`    | Callback before popunder opens.                                                | empty function |
| `afterOpen`     | Callback after popunder opens.                                                 | empty function |

## ✅ Browser Compatibility

* ✅ Chrome
* ✅ Firefox
* ✅ Safari
* ✅ Edge
* ✅ IE (Limited support)

*Note:* Popunders may be blocked by browsers or extensions with strict security settings or popup blockers.

## 📢 Disclaimer

Ensure compliance with web standards, advertising policies, and privacy regulations. Use this responsibly to maintain a positive user experience.

## 📄 License

This project is licensed under the MIT License.

```

You can directly copy and paste the above markdown content into your **`README.md`** file on GitHub.
```
