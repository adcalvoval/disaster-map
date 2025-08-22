# Movie Wishlist with Supabase Integration

A modern web application for managing your movie and TV show wishlist with cross-device synchronization.

## ✨ Features

### 🎬 Movie & TV Show Management
- Search movies and TV shows using The Movie Database (TMDB) API
- Smart search by title, actor, or director
- Separate wishlists for movies and TV shows
- Detailed information including posters, cast, director, and genres

### 🔄 Cross-Device Sync
- **Supabase Integration**: Your data syncs across all devices
- **Offline Support**: Works without internet, syncs when back online
- **Data Migration**: Existing localStorage data automatically migrated
- **Real-time Status**: Visual indicators show sync status

### 🎨 User Experience
- Responsive design for desktop and mobile
- Genre filtering and multiple sorting options
- CSV export/import functionality
- Clean, modern interface with smooth animations

## 🚀 Quick Start

### 1. Set Up Supabase (Optional)
1. Create account at [supabase.com](https://supabase.com)
2. Create new project
3. Go to **SQL Editor** and run the schema from `../supabase-schema.sql`
4. Get your Project URL and anon key from **Settings → API**
5. Update credentials in `supabase.js`

### 2. Run the App
1. Open `index.html` in your browser
2. Start searching for movies and TV shows!
3. Sign in to enable cross-device sync

## 🔧 Configuration

### Without Supabase
The app works perfectly with just localStorage - your data stays on your device.

### With Supabase
Update these values in `supabase.js`:
```javascript
const SUPABASE_URL = 'your-project-url'
const SUPABASE_ANON_KEY = 'your-anon-key'
```

## 📱 How It Works

### Local Mode (Default)
- Data stored in browser localStorage
- Works offline
- Device-specific storage

### Cloud Mode (With Supabase)
- Sign up/in with email and password
- Data synced to Supabase database
- Access from any device
- Offline support with sync when online

## 🎯 Usage

1. **Search**: Use the search bar to find movies or TV shows
2. **Add to Wishlist**: Click the "+" button on search results
3. **Manage Lists**: View your wishlists in the main interface
4. **Filter & Sort**: Use genre filters and sorting options
5. **Export Data**: Download your wishlist as CSV
6. **Sign In**: Enable cloud sync for cross-device access

## 🛠️ Technical Details

### Stack
- **Frontend**: Vanilla HTML, CSS, JavaScript
- **Database**: Supabase (PostgreSQL)
- **API**: The Movie Database (TMDB)
- **Authentication**: Supabase Auth

### Architecture
- Hybrid storage (localStorage + Supabase)
- Offline-first design
- Progressive enhancement
- Mobile-responsive

### Security
- Row Level Security (RLS) in Supabase
- User-specific data access
- Safe API key usage

## 📂 File Structure

```
movie-library/
├── index.html          # Main application
├── script.js           # Core functionality
├── styles.css          # Styling
├── supabase.js         # Supabase integration
├── test-import.csv     # Sample CSV data
└── README.md           # This file
```

## 🎨 Features Overview

- **Smart Search**: Find content by title, actor, or director
- **Genre Filtering**: Filter by movie/TV genres
- **Multiple Sorting**: Sort by title, year, or genre
- **CSV Export/Import**: Backup and restore your data
- **Responsive Design**: Works on all screen sizes
- **Real-time Sync**: Changes appear instantly across devices
- **Offline Support**: Use without internet connection

## 🔮 Future Enhancements

- Social features (sharing wishlists)
- Streaming service integration
- Personalized recommendations
- Mobile app versions
- Advanced filtering options

## 🤝 Contributing

This is a personal project, but suggestions and improvements are welcome!

## 📄 License

Open source - feel free to use and modify for your own projects.

---

**Enjoy building your perfect movie watchlist!** 🍿🎬