# Project Setup Guide

## 📚 Complete Setup Instructions

### Prerequisites Checklist
- [ ] Node.js (≥14.0.0) installed
- [ ] npm (≥6.0.0) installed
- [ ] Git installed
- [ ] Text editor or IDE

### Step 1: Clone the Repository

```bash
git clone https://github.com/kalimireddyreshma/Bigcalendar.git
cd Bigcalendar
```

### Step 2: Extract Project Files from ZIP

The repository contains a `react-big-calendar-master.zip` file that needs to be extracted:

```bash
# Extract the ZIP file
unzip react-big-calendar-master.zip

# Move contents to the root directory (adjust based on ZIP structure)
# If the ZIP contains a folder like 'react-big-calendar-master':
mv react-big-calendar-master/* .
rmdir react-big-calendar-master

# Remove the ZIP file
rm react-big-calendar-master.zip
```

### Step 3: Install Dependencies

```bash
npm install
```

This will install all required packages listed in `package.json`:
- React & React DOM
- React Big Calendar
- Date-fns
- Development tools (ESLint, Prettier, etc.)

### Step 4: Start Development Server

```bash
npm start
```

The application will open automatically at `http://localhost:3000`

### Step 5: Verify Installation

- [ ] Calendar displays correctly
- [ ] Can navigate between months/weeks/days
- [ ] No console errors
- [ ] Responsive design works on different screen sizes

---

## 📦 Environment Setup

### Create Environment File

```bash
# Copy the example environment file
cp .env.example .env.local
```

Edit `.env.local` as needed for your setup.

---

## 🧪 Testing & Development

### Available Commands

| Command | Purpose |
|---------|---------|
| `npm start` | Start development server |
| `npm test` | Run test suite |
| `npm run build` | Create production build |
| `npm run lint` | Check code quality |
| `npm run lint:fix` | Auto-fix linting issues |
| `npm run format` | Format code with Prettier |
| `npm run storybook` | Start Storybook component library |

### Development Workflow

```bash
# 1. Start development server
npm start

# 2. In another terminal, start tests in watch mode
npm test

# 3. Before committing, format and lint
npm run format
npm run lint:fix
```

---

## 🐛 Troubleshooting

### Issue: `npm install` fails

**Solution:**
```bash
# Clear npm cache
npm cache clean --force

# Delete node_modules and lock file
rm -rf node_modules package-lock.json

# Reinstall
npm install
```

### Issue: Port 3000 already in use

**Solution:**
```bash
# On macOS/Linux
lsof -i :3000
kill -9 <PID>

# On Windows
netstat -ano | findstr :3000
taskkill /PID <PID> /F

# Or specify a different port
PORT=3001 npm start
```

### Issue: Module not found errors

**Solution:**
```bash
# Make sure you're in the correct directory
pwd  # verify current directory

# Ensure node_modules exists
npm install

# Clear cache
npm cache clean --force
```

---

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
├── .env.example
├── README.md
└── CONTRIBUTING.md
```

---

## 🚀 Next Steps

1. ✅ Complete the setup above
2. 📖 Read the [README.md](README.md)
3. 📝 Check [CONTRIBUTING.md](CONTRIBUTING.md) for contribution guidelines
4. 🧩 Explore components in Storybook (`npm run storybook`)
5. 💻 Start building!

---

## 📞 Need Help?

- 📖 Check the [README.md](README.md)
- 🤝 Review [CONTRIBUTING.md](CONTRIBUTING.md)
- 🐛 Open an [issue](https://github.com/kalimireddyreshma/Bigcalendar/issues)
- 💬 Use GitHub Discussions

Happy coding! 🎉
