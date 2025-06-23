# Interactive Calendar Widget

A modern, interactive calendar widget with drag & drop events, multiple views, and local storage. Perfect for websites and web applications that need a comprehensive event management system.

## ✨ Features

- **Multiple Views**: Month, Week, and Day views for different perspectives
- **Event Management**: Add, edit, and delete events with full CRUD operations
- **Color Coding**: Customize event colors for better organization
- **Local Storage**: Events persist between sessions
- **Responsive Design**: Works perfectly on all devices
- **Modern UI**: Clean, intuitive interface with smooth animations
- **Accessible**: Built with ARIA attributes and keyboard navigation
- **Lightweight**: Pure CSS and JavaScript, no dependencies

## 🚀 Live Demo

[View on CodePen](https://codepen.io/harmoncode/pen/your-pen-id)

## 📁 Files

- `index.html` - Main HTML structure
- `style.css` - All styling and animations
- `script.js` - JavaScript functionality

## 🛠️ Usage

### Basic Implementation

```html
<div class="container">
    <!-- Calendar Header -->
    <header class="calendar-header">
        <div class="header-controls">
            <button class="btn btn-icon" id="prevMonth">
                <i class="fas fa-chevron-left"></i>
            </button>
            <h1 class="current-month" id="currentMonth">December 2024</h1>
            <button class="btn btn-icon" id="nextMonth">
                <i class="fas fa-chevron-right"></i>
            </button>
        </div>
        
        <div class="view-controls">
            <button class="btn btn-view active" data-view="month">Month</button>
            <button class="btn btn-view" data-view="week">Week</button>
            <button class="btn btn-view" data-view="day">Day</button>
        </div>
    </header>

    <!-- Calendar Container -->
    <div class="calendar-container">
        <!-- Month View -->
        <div class="calendar-view month-view active" id="monthView">
            <div class="calendar-weekdays">
                <div class="weekday">Sun</div>
                <div class="weekday">Mon</div>
                <div class="weekday">Tue</div>
                <div class="weekday">Wed</div>
                <div class="weekday">Thu</div>
                <div class="weekday">Fri</div>
                <div class="weekday">Sat</div>
            </div>
            <div class="calendar-grid" id="monthGrid">
                <!-- Days will be populated by JavaScript -->
            </div>
        </div>
    </div>
</div>
```

### JavaScript Initialization

```javascript
// Initialize calendar
const calendar = new InteractiveCalendar();

// Add event programmatically
calendar.addEvent({
    title: 'Meeting',
    date: '2024-12-15',
    startTime: '10:00',
    endTime: '11:00',
    description: 'Team meeting',
    color: '#667eea'
});
```

## 🎨 Customization Options

- **Colors**: Customize calendar colors, event colors, and themes
- **Layout**: Modify calendar layout and spacing
- **Animations**: Adjust transition effects and timing
- **Typography**: Change fonts, sizes, and weights
- **Event Colors**: Add/remove color options for events

## ⚙️ Configuration

```javascript
const calendarConfig = {
    defaultView: 'month',        // Default view (month, week, day)
    startHour: 6,               // Start hour for day/week view
    endHour: 22,                // End hour for day/week view
    enableLocalStorage: true,   // Enable local storage
    eventColors: [              // Available event colors
        '#667eea', '#10b981', '#f59e0b', '#ef4444', '#8b5cf6'
    ]
};
```

## 📱 Browser Support

- Chrome ✅
- Firefox ✅
- Safari ✅
- Edge ✅
- IE11+ ✅

## 🔧 API Methods

### Event Management
- `addEvent(eventData)` - Add a new event
- `updateEvent(eventId, eventData)` - Update existing event
- `deleteEvent(eventId)` - Delete an event
- `getEventsForDate(date)` - Get events for specific date

### Navigation
- `navigateMonth(direction)` - Navigate months (+1 or -1)
- `switchView(view)` - Switch between month/week/day views
- `selectDate(date)` - Select a specific date

### Data Management
- `saveEvents()` - Save events to localStorage
- `loadEvents()` - Load events from localStorage

## 🎯 Use Cases

- **Event Management Systems**: Perfect for scheduling and organizing events
- **Booking Platforms**: Handle appointments and reservations
- **Project Management**: Track deadlines and milestones
- **Personal Calendars**: Individual scheduling and planning
- **Team Calendars**: Collaborative event planning

## 🚀 Advanced Features

- **Drag & Drop**: Move events between dates (coming soon)
- **Recurring Events**: Set up repeating events
- **Event Categories**: Organize events by type
- **Export/Import**: Share calendar data
- **Notifications**: Event reminders and alerts

## 📱 Responsive Design

The calendar is fully responsive and works on:
- Desktop computers
- Tablets
- Mobile phones
- Touch devices

## 🎨 Styling

The calendar uses modern CSS features:
- CSS Grid for layout
- Flexbox for alignment
- CSS Custom Properties for theming
- Smooth transitions and animations
- Modern color schemes

## 🤝 Contributing

Feel free to submit issues and enhancement requests!

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Created by

**Harmon Code** - [harmoncode.com](https://harmoncode.com)

---

⭐ If you find this useful, please give it a star! 