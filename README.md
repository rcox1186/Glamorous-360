# Glamorous 360 - Venue Booking Page

A modern, interactive venue booking page featuring a 360-degree panoramic viewer and elegant booking form.

## Features

✨ **360-Degree Panoramic Viewer** - Explore the venue with Pannellum viewer
📅 **Easy Date & Time Selection** - Intuitive booking form with date/time inputs
🎨 **Modern Design** - Responsive, glamorous UI with smooth interactions
✅ **Form Validation** - Prevents past date bookings and ensures required fields
📱 **Mobile Responsive** - Works seamlessly on all screen sizes
🚀 **Production Ready** - Includes error handling, loading states, and success feedback

## Installation

```bash
# Install dependencies
npm install

# Start development server
npm start

# Build for production
npm build
```

## Usage

The BookingPage component is your main entry point. It displays:
- A 360-degree panoramic view of the venue on the left
- A booking form on the right for date/time selection

### Key Components

- **BookingPage.jsx** - Main component with form logic and 360 viewer
- **BookingPage.css** - Responsive styling with glassmorphism effects

## Technology Stack

- React 18.2.0
- Pannellum 2.5 (360 viewer)
- CSS3 with responsive design
- Modern JavaScript (ES6+)

## API Integration

The booking form is ready to connect to your backend. Update the fetch URL in `handleBooking()`:

```javascript
const response = await fetch('/api/bookings', {
  method: 'POST',
  headers: { 'Content-Type': 'application/json' },
  body: JSON.stringify({ date: bookingDate, time: bookingTime })
});
```

## Customization

### Change the Panorama Image

Edit the panorama URL in `BookingPage.jsx`:

```javascript
panorama: "https://your-image-url.jpg"
```

### Customize Colors

Modify the CSS variables in `BookingPage.css`:

```css
background: #007bff; /* Primary color */
```

## Browser Support

- Chrome/Edge 88+
- Firefox 85+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

## License

MIT

## Author

Created by rcox1186
