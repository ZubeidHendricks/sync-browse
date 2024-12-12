# Sync Browse

A Chrome extension for synchronized browsing with chat and voice features.

## Features

- Real-time synchronized web browsing
- Text chat with other participants
- Voice chat using WebRTC
- Screen sharing capabilities
- User authentication
- Room-based collaboration

## Project Structure

```
sync-browse/
├── extension/         # Chrome extension files
│   ├── manifest.json
│   ├── popup.html
│   ├── styles.css
│   ├── popup.js
│   ├── background.js
│   └── connection-manager.js
└── server/           # Backend server files
    ├── package.json
    ├── server.js
    ├── config.js
    └── models/
        ├── User.js
        └── Room.js
```

## Setup Instructions

### Extension Setup

1. Clone this repository
2. Open Chrome and go to `chrome://extensions/`
3. Enable Developer Mode
4. Click "Load unpacked" and select the `extension` directory

### Server Setup

1. Navigate to the `server` directory
2. Create `.env` file with your configuration:
```env
PORT=3000
MONGODB_URI=your_mongodb_uri
JWT_SECRET=your_secret_key
TURN_SERVER_URL=your_turn_server
TURN_USERNAME=turn_username
TURN_PASSWORD=turn_password
```
3. Install dependencies: `npm install`
4. Start the server: `npm start`

## Development

Pull requests are welcome. For major changes, please open an issue first.