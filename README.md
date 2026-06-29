# React Big Calendar Application

[![GitHub](https://img.shields.io/badge/GitHub-kalimireddyreshma/Bigcalendar-blue)](https://github.com/kalimireddyreshma/Bigcalendar)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Node Version](https://img.shields.io/badge/node-%3E%3D14.0.0-green)](https://nodejs.org/)

A responsive, feature-rich React.js calendar application built with the **React Big Calendar** library. This project demonstrates advanced React component usage, modern UI design, and real-world event scheduling system implementation.

## 📋 Features

- 📅 **Multiple Calendar Views**: Monthly, weekly, and daily views
- 🗓️ **Event Scheduling**: Create, edit, and delete events
- 🎨 **Responsive Design**: Works seamlessly on desktop, tablet, and mobile
- 🧭 **Easy Navigation**: Intuitive date navigation and quick access
- 🔄 **Real-time Updates**: Dynamic event management
- 📱 **Mobile-Friendly**: Touch-friendly interface
- ♿ **Accessible**: WCAG compliant

## 🛠️ Tech Stack

| Technology | Version | Purpose |
|-----------|---------|---------|
| **React** | ^18.2.0 | UI Framework |
| **React Big Calendar** | ^1.8.5 | Calendar Component Library |
| **Date-fns** | ^2.30.0 | Date Manipulation |
| **React Scripts** | 5.0.1 | Build Tools |

### Development Tools

- **ESLint** - Code quality & linting
- **Prettier** - Code formatting
- **Storybook** - Component documentation

## 📦 Installation

### Prerequisites

- **Node.js** ≥ 14.0.0
- **npm** ≥ 6.0.0

### Steps

1. **Clone the repository**

   ```bash
   git clone https://github.com/kalimireddyreshma/Bigcalendar.git
   cd Bigcalendar
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Start the development server**

   ```bash
   npm start
   ```

   The application will open at [http://localhost:3000](http://localhost:3000)

## 🚀 Usage

### Running the Application

```bash
# Development mode with hot reload
npm start

# Production build
npm run build

# Run tests
npm test
```

### Code Quality

```bash
# Lint code
npm run lint

# Fix linting issues
npm run lint:fix

# Format code with Prettier
npm run format
```

### Storybook (Component Documentation)

```bash
# Start Storybook dev server
npm run storybook

# Build Storybook static site
npm run build-storybook
```

## 📁 Project Structure

```
Bigcalendar/
├── src/
│   ├── components/
│   │   ├── Calendar.jsx
│   │   ├── EventForm.jsx
│   │   └── EventList.jsx
│   ├── pages/
│   │   └── Home.jsx
│   ├── styles/
│   │   └── index.css
│   ├── App.jsx
│   └── index.jsx
├── public/
│   ├── index.html
│   └── favicon.ico
├── stories/
│   └── Calendar.stories.jsx
├── .storybook/
│   ├── main.js
│   └── preview.js
├── package.json
├── .eslintrc.json
├── .prettierrc
├── .gitignore
└── README.md
```

## 🎯 Example Usage

### Basic Calendar Component

```jsx
import React, { useState } from 'react';
import { Calendar, momentLocalizer } from 'react-big-calendar';
import moment from 'moment';
import 'react-big-calendar/lib/css/react-big-calendar.css';

const localizer = momentLocalizer(moment);

export default function MyCalendar() {
  const [events, setEvents] = useState([
    {
      id: 1,
      title: 'Team Meeting',
      start: new Date(2024, 0, 15, 10, 0),
      end: new Date(2024, 0, 15, 11, 0),
    },
  ]);

  return (
    <Calendar
      localizer={localizer}
      events={events}
      startAccessor="start"
      endAccessor="end"
      style={{ height: 500 }}
    />
  );
}
```

## 🤝 Contributing

We welcome contributions! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

### Quick Start

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Commit changes: `git commit -m 'Add amazing feature'`
4. Push to branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

## 🙋 Support & Issues

- Found a bug? [Open an issue](https://github.com/kalimireddyreshma/Bigcalendar/issues)
- Have a question? [Start a discussion](https://github.com/kalimireddyreshma/Bigcalendar/discussions)

## 📧 Contact

**Author**: [@kalimireddyreshma](https://github.com/kalimireddyreshma)

## 🙏 Acknowledgments

- [React Big Calendar](https://jquense.github.io/react-big-calendar/)
- [React Documentation](https://react.dev/)
- [Date-fns](https://date-fns.org/)

---

<div align="center">
  <p>⭐ If helpful, consider giving this project a star! ⭐</p>
</div>
