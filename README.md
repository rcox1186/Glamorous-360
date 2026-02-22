# Glamorous 360 - Venue Booking Platform

A modern, elegant venue booking application featuring 360-degree panoramic venue previews and seamless reservation management.

## Features

✨ **360-Degree Panoramic Viewer** - Explore venues with immersive panoramic images
📅 **Smart Date Selection** - Prevents past date bookings automatically
⏰ **Time Selection** - Easy time slot picking for your event
✅ **Real-time Validation** - Instant feedback on your booking details
📱 **Fully Responsive** - Works beautifully on desktop, tablet, and mobile devices
🎨 **Modern UI** - Glassmorphism design with smooth animations and transitions
♿ **Accessible** - Built with accessibility standards (WCAG) in mind

## Tech Stack

- **React 18** - UI framework
- **Pannellum** - 360-degree panoramic viewer library
- **CSS3** - Modern styling with gradients and animations
- **JavaScript ES6+** - Modern JavaScript features

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/rcox1186/Glamorous-360.git
cd Glamorous-360
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm start
```

The application will open at `http://localhost:3000`

## Project Structure

```
Glamorous-360/
├── public/
│   └── index.html
├── src/
│   ├── components/
│   │   ├── BookingPage.jsx
│   │   └── BookingPage.css
│   ├── index.js
│   ├── index.css
│   └── App.js
├── package.json
└── README.md
```

## Usage

1. **View the Venue** - Use the 360 panoramic viewer to explore the venue from all angles
2. **Select a Date** - Choose your preferred booking date (minimum tomorrow)
3. **Select a Time** - Pick the time for your event
4. **Confirm Reservation** - Submit your booking request
5. **Receive Confirmation** - Get instant feedback on your booking

## Customization

### Change the Panoramic Image

Edit `src/components/BookingPage.jsx` line 23:
```javascript
panorama: "YOUR_360_IMAGE_URL_HERE",
```

### Update Venue Title

Edit the title in the same file (line 24):
```javascript
title: "Your Venue Name",
```

### Customize Colors

Modify the CSS in `src/components/BookingPage.css` to match your branding

## Backend Integration

To connect to your backend API, update the `handleBooking` function in `BookingPage.jsx`:

```javascript
const response = await fetch('YOUR_API_ENDPOINT', {
  method: 'POST',
  headers: { 'Content-Type': 'application/json' },
  body: JSON.stringify({ 
    date: bookingDate, 
    time: bookingTime 
  })
});
```

## Available Scripts

### `npm start`
Runs the app in development mode at `http://localhost:3000`

### `npm build`
Builds the app for production to the `build` folder

### `npm test`
Launches the test runner in interactive watch mode

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the MIT License.

## Support

For support, please open an issue on the GitHub repository.

---

**Built with ❤️ for glamorous events**