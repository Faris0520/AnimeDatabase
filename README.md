# Anime Database with MyAnimeList Integration

A React web application for searching and exploring anime using the Jikan API (unofficial MyAnimeList API).

## Features

- **Anime Search**: Search anime by title
- **Top Anime**: Display list of most popular anime
- **Anime Details**: View complete information including:
  - Rating, broadcast schedule, and anime type
  - Duration, rank, and popularity
  - Season and release year
  - Trailer (if available)
- **Detail Popup**: Click anime cards to view full details in a popup
- **Responsive Design**: Optimal viewing experience across different screen sizes

## Demo

[https://project-8-wphj.vercel.app/](https://project-8-wphj.vercel.app/)

## Screenshot

![Anime Database Screenshot](https://i.imgur.com/lngnweQ.png)

## Technologies Used

- **React** - JavaScript library for building UI
- **Jikan API** - Unofficial API for MyAnimeList
- **SCSS/CSS** - Styling
- **React Hooks** - State management (useState, useEffect)

## Project Structure

```
AnimeDatabase/
├── public/
│   ├── index.html
│   ├── manifest.json
│   └── robots.txt
├── src/
│   ├── App.js
│   ├── index.js
│   ├── assets/
│   │   ├── css/
│   │   │   └── main.css
│   │   └── scss/
│   │       └── main.scss
│   └── components/
│       ├── AnimeCard.js
│       ├── AnimePopup.js
│       ├── Header.js
│       ├── MainContent.js
│       └── Sidebar.js
├── package.json
└── README.md
```

## Installation

1. Clone repository:
```bash
git clone https://github.com/Faris0520/AnimeDatabase.git
cd AnimeDatabase
```

2. Install dependencies:
```bash
npm install
```

3. Run the application:
```bash
npm start
```

4. Open browser and access:
```
http://localhost:3000
```

## Components

### `src/App.js`
Main component that manages state and API calls.

### `src/components/Header.js`
Displays the application title.

### `src/components/Sidebar.js`
Displays a list of top 5 popular anime with links to MyAnimeList.

### `src/components/MainContent.js`
Manages search box, search results list, and detail popup.

### `src/components/AnimeCard.js`
Displays individual anime cards with image and title.

### `src/components/AnimePopup.js`
Modal popup that displays complete anime details including trailer.

## API

This application uses [Jikan API v4](https://docs.api.jikan.moe/):
- **Top Anime**: `https://api.jikan.moe/v4/top/anime?filter=bypopularity`
- **Search Anime**: `https://api.jikan.moe/v4/anime?q={query}&order_by=title&sort=asc&limit=10`

## Styling

- Uses SCSS compiled to CSS
- Font: 'Fira Sans'
- Main colors: #313131, #AAA, #EEE
- Hover effects and transition animations
- Responsive design with flexbox

## Responsive Design

This application is optimized for various screen sizes:
- Desktop: Layout with sidebar and 3-column grid
- Mobile: Stack layout with responsive grid

## Contributing

Contributions are always welcome! Please:
1. Fork the repository
2. Create a new branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Create a Pull Request

## License

This project is open source and available for free use.

## Author

**Faris0520**

## Acknowledgments

- [MyAnimeList](https://myanimelist.net/) for anime data
- [Jikan API](https://jikan.moe/) for providing the REST API
- Create React App for project template
