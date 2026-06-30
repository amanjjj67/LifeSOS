# LifeSOS - Tourist Safety Platform

LifeSOS is a comprehensive travel safety application designed to protect tourists from scams and provide emergency assistance. Built with Next.js and secured with Clerk authentication.

## Features

- **Real-Time Scam Alerts** - Get notified about scam-prone areas near your location
- **Emergency SOS** - Instant SOS button that alerts emergency services
- **Cab Fare Estimation** - Check accurate cab fares to avoid overcharging
- **Price Checker** - Verify product prices before purchasing
- **Community Reporting** - Report and view scams reported by other travelers
- **Tourist Chatroom** - Connect with fellow travelers via real-time chat

## Tech Stack

- **Frontend:** Next.js 14, TypeScript, Tailwind CSS
- **Authentication:** Clerk
- **Maps:** Leaflet, Mapbox
- **Real-time Chat:** Socket.io
- **Charts:** Chart.js

## Local Development

### Prerequisites

- Node.js 18+
- npm

### Setup

1. Clone the repository
2. Install dependencies:

```bash
# Install frontend dependencies
npm install

# Install server dependencies
cd server && npm install && cd ..
```

3. Create a `.env` file in the root with your Clerk keys:

```
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_publishable_key
CLERK_SECRET_KEY=your_secret_key
```

4. Start the development servers:

```bash
# Terminal 1 - Frontend (Next.js)
npm run dev

# Terminal 2 - Socket.io server
cd server && npm start
```

5. Open [http://localhost:3000](http://localhost:3000)

### Available Routes

| Route | Description |
|-------|-------------|
| `/` | Home page |
| `/features` | Features overview |
| `/impact` | Impact statistics |
| `/track` | Track scam areas |
| `/about` | About the project |
| `/cabfare` | Cab fare estimation |
| `/sos` | Emergency SOS |
| `/chatroom` | Tourist chatroom |
| `/report-scam` | Report a scam |
| `/contact` | Contact page |

