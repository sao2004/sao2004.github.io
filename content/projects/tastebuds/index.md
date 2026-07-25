---
title: "TasteBuds"
date: 2026-07-25
summary: "App for voting restaurants in the area - great when you and your friends can't decide where to eat."
---

TasteBuds is a web application that helps groups find restaurants nearby and match on where to eat, using a swipe interface.

{{< github repo="sao2004/TasteBuds" showThumbnail=false >}}

## Screenshots

{{< carousel images="{login_screen.png,home_screen.png,swipe_screen.png}" captions="{login_screen.png:Login screen - sign in with Google or as a guest,home_screen.png:Home screen - create or join a room,swipe_screen.png:Swipe screen - vote on restaurants in real time}" >}}

## Features

- **Google & Guest Authentication** - sign in with Google or jump in as a guest
- **Room Creation** - create a virtual room using GPS to pull nearby restaurants
- **Join via Code** - others join with a unique 5-character room code
- **Swiping Mechanism** - vote "Yes" or "No" on restaurant cards
- **Real-time Matching** - instant notification when the whole group likes the same place
- **Winner Selection** - if there are multiple matches, the app randomly picks a final winner
- **Google Maps Redirection** - jump straight to directions for the chosen restaurant
- **History Tracking** - view past favorite restaurants (for Google-authenticated users)

## Design Patterns

- **Factory Pattern** - standardizes how `Room` objects are created, centralizing ID generation and data structure setup
- **Facade Pattern** - a dedicated `HistoryService` simplifies Firebase collection interactions behind clean, high-level methods

## Tech Stack

| Component | Technology | Role |
|---|---|---|
| Frontend | React.js | UI and state management |
| Styling | Tailwind CSS | Responsive design |
| Backend | Python (Flask) | API proxy for Google Places |
| Database | Firebase Firestore | NoSQL storage and real-time sync |
| Authentication | Firebase Auth | Google Sign-In |
| External API | Google Places API | Restaurant data and geolocation |
