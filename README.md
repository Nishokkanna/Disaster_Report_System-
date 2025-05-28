# Disaster Response AI

A frontend-based AI-powered web application that aids in disaster response by analyzing uploaded images, detecting damage severity using the Google Cloud Vision API, and visualizing affected zones on an interactive Google Map.

## Features

- 🗺️ Interactive Google Map showing disaster location of user report.
- 🔔 Real-time browser push alerts using Notification API
- 💾 Local storage for saving disaster reports
- 📱 Responsive design for mobile and desktop

## Setup

1. Clone this repository
2. Get your API keys:
   - Google Maps JavaScript API key (with Places API enabled)
   - Google Cloud Vision API key
3. Serve the application using a local web server (e.g., Live Server in VS Code)

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

### Browser Requirements
- Modern browser with JavaScript enabled
- LocalStorage support

### Data Storage
The application uses browser's LocalStorage to save disaster reports. No backend server is required.

## License

MIT License - Feel free to use this project for any purpose.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request 
