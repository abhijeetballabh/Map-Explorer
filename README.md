# Map Explorer

A React-based web application that replicates Google Maps functionality, allowing users to search for locations, view them on an interactive map, and discover nearby points of interest by category.

## Features

- **Interactive Map**: Built with React Leaflet and Leaflet for seamless map interactions
- **Geolocation Support**: Automatically detects and displays user's current location with location accuracy feedback
- **Location Search**: Autocomplete search functionality using OpenStreetMap's Nominatim API
- **Point of Interest Discovery**: Browse nearby places by categories:
  - Restaurants
  - Hospitals
  - Museums
  - Gas Stations
  - And more...
- **Real-time Place Fetching**: Uses OpenStreetMap's Overpass API to fetch nearby places based on selected category
- **Responsive UI**: Search panel and map controls for easy navigation

## Technologies Used

- **Frontend Framework**: React 18.3.1
- **Mapping Library**: 
  - React Leaflet 4.2.1
  - Leaflet 1.9.4
- **API Integration**:
  - Axios 1.7.9 (HTTP requests)
  - OpenStreetMap Nominatim (location search)
  - OpenStreetMap Overpass API (place data)
- **UI Components**:
  - React Autosuggest 10.1.0 (search suggestions)
- **Build Tool**: Create React App with React Scripts 5.0.1

## Project Structure

```
src/
├── App.js              # Main application component with map logic
├── App.css             # Main styling
├── Search.js           # Search component with autosuggest functionality
├── Search.css          # Search styling
├── index.js            # React entry point
├── index.css           # Global styles
└── setupTests.js       # Test configuration

public/
├── index.html          # HTML template
├── manifest.json       # PWA manifest
└── robots.txt          # SEO robots file
```

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/abhijeetballabh/React-Map-App.git
cd final-google-maps-clone
```

2. Install dependencies:
```bash
npm install
```

### Running the Application

Start the development server:
```bash
npm start
```

The application will open at [http://localhost:3000](http://localhost:3000)

### Building for Production

Create an optimized production build:
```bash
npm run build
```

This generates a `build/` folder with minified files ready for deployment.

### Running Tests

```bash
npm test
```

Launches the test runner in interactive watch mode.

## Usage

1. **Allow Location Access**: When prompted, grant location permission to display your current position on the map
2. **Search for Locations**: Use the search bar to find any location. The autocomplete will suggest matching locations
3. **Explore Places**: Click on category buttons (Restaurant, Hospital, Museum, etc.) to discover nearby places
4. **View Place Details**: Click on markers to see place information in popups
5. **Navigate Map**: Use standard map controls to zoom and pan around the map

## API References

- **Nominatim Search API**: `https://nominatim.openstreetmap.org/search`
  - Provides location search and autocomplete suggestions
  
- **Overpass API**: `https://overpass-api.de/api/interpreter`
  - Fetches nearby points of interest within a 2km radius of the selected location

## Browser Support

The application supports all modern browsers including:
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Known Limitations

- Location accuracy warning displays for accuracy readings over 100 meters
- Place searches are limited to a 2km radius around the selected location
- Some location categories may have limited data depending on OSM coverage in that region

## Future Enhancements

- Route planning and directions
- Street view integration
- Custom marker clustering for better performance
- Place reviews and ratings integration
- Offline map support
- User location history

## Author

- **Abhijeet Ballabh** - GitHub: [@abhijeetballabh](https://github.com/abhijeetballabh)
