# Disaster Response AI

A frontend-based AI-powered web application that aids in disaster response by analyzing uploaded images, detecting damage severity using the Google Cloud Vision API, and visualizing affected zones on an interactive Google Map.

## Features

- 🎯 AI-based damage detection using Google Cloud Vision API
- 🗺️ Interactive Google Map showing live damage classification
- 🏥 Nearby emergency locations using Google Places API
- 🔔 Real-time browser push alerts using Notification API
- 💾 Local storage for saving disaster reports
- 📱 Responsive design for mobile and desktop

## Setup

1. Clone this repository
2. Get your API keys:
   - Google Maps JavaScript API key (with Places API enabled)
   - Google Cloud Vision API key
3. Create a `js/config.js` file with your API keys:
   ```javascript
   const CONFIG = {
       GOOGLE_MAPS_API_KEY: 'YOUR_GOOGLE_MAPS_API_KEY',
       GOOGLE_CLOUD_VISION_API_KEY: 'YOUR_GOOGLE_CLOUD_VISION_API_KEY'
   };
   ```
4. Replace the Google Maps API key in `index.html`:
   ```html
   <script src="https://maps.googleapis.com/maps/api/js?key=YOUR_GOOGLE_MAPS_API_KEY&libraries=places"></script>
   ```
5. Serve the application using a local web server (e.g., Live Server in VS Code)

## Usage

1. Allow location access when prompted to see nearby emergency services
2. Upload disaster images using the upload button or drag-and-drop
3. View AI analysis results and severity classification
4. Check the map for:
   - 🔴 Danger zones
   - 🟡 Moderate risk areas
   - 🟢 Safe zones
5. Enable notifications to receive alerts about new disaster reports
6. Click on emergency service markers to view details

## Technical Details

### APIs Used
- Google Cloud Vision API for image analysis
- Google Maps JavaScript API for mapping
- Google Places API for emergency services
- Web Notifications API for alerts

### Browser Requirements
- Modern browser with JavaScript enabled
- Geolocation support
- Notifications support
- LocalStorage support

### Data Storage
The application uses browser's LocalStorage to save disaster reports. No backend server is required.

## Privacy & Security

- No data is sent to any server except Google APIs
- Image analysis is performed client-side using the Vision API
- Location data is only used for mapping and is stored locally
- Reports are saved in your browser's local storage

## License

MIT License - Feel free to use this project for any purpose.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request 
