# Wanderlust Travel Presentation

This is a dynamic travel presentation built with React, Framer Motion, and React Globe GL.

## How to Add/Edit Destinations

To add or edit destinations, modify the file:
`client/src/lib/destinations.ts`

### Data Structure
Each destination has the following format:
```typescript
{
  id: 'unique-id',
  name: 'City Name',
  country: 'Country Name',
  subtitle: 'Short tagline',
  description: 'Full description text...',
  image: 'Imported image object',
  lat: 48.8566, // Latitude
  lng: 2.3522,  // Longitude
  stats: {
    visitors: '17.4M/yr',
    temp: '12.8°C',
    bestTime: 'Apr-Jun'
  }
}
```

### Adding Images
1. Place new images in `attached_assets/stock_images/` (or any folder).
2. Import the image at the top of `destinations.ts`:
   `import newCityImg from '@assets/stock_images/new-city.jpg';`
3. Use `newCityImg` in the destination object.

## Features
- Interactive 3D Globe with zoom and spin.
- Smooth transitions between Globe and Slide views.
- Swipe gestures for mobile navigation.
- Responsive design.
