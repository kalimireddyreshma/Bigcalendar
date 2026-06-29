# Contributing to React Big Calendar

Thank you for your interest in contributing to this project! We appreciate all contributions, big and small.

## 🎯 Code of Conduct

Please be respectful and constructive in all interactions. We're committed to providing a welcoming and inclusive environment.

## 🚀 Getting Started

### 1. Fork and Clone

```bash
# Fork the repository on GitHub
# Clone your fork
git clone https://github.com/YOUR_USERNAME/Bigcalendar.git
cd Bigcalendar

# Add upstream remote
git remote add upstream https://github.com/kalimireddyreshma/Bigcalendar.git
```

### 2. Set Up Development Environment

```bash
# Install dependencies
npm install

# Create a new branch for your feature
git checkout -b feature/your-feature-name
```

### 3. Make Your Changes

```bash
# Start development server
npm start

# In another terminal, run tests
npm test

# Lint your code
npm run lint

# Format code
npm run format
```

## 📋 Contribution Guidelines

### Before You Start

- Check [existing issues](https://github.com/kalimireddyreshma/Bigcalendar/issues) to avoid duplicates
- Open an issue first for significant changes
- Discuss major features in an issue before coding

### Commit Messages

Follow these conventions:

```bash
# Feature
git commit -m "feat: add event filtering by category"

# Bug fix
git commit -m "fix: resolve calendar date navigation issue"

# Documentation
git commit -m "docs: update installation guide"

# Style
git commit -m "style: format code with prettier"

# Test
git commit -m "test: add unit tests for Calendar component"

# Refactor
git commit -m "refactor: simplify event validation logic"
```

### Code Quality

```bash
# Ensure linting passes
npm run lint:fix

# Format code
npm run format

# Run tests
npm test

# Check test coverage
npm test -- --coverage
```

## 🧪 Testing

### Writing Tests

- Write tests for new features
- Update tests when changing existing code
- Maintain ≥80% code coverage

```bash
# Run all tests
npm test

# Run tests in watch mode
npm test -- --watch

# Run tests with coverage report
npm test -- --coverage
```

## 📤 Submitting a Pull Request

1. **Push your branch**

   ```bash
   git push origin feature/your-feature-name
   ```

2. **Create a Pull Request**

   - Use a clear, descriptive title
   - Reference related issues: "Closes #123"
   - Describe what your PR does
   - Include screenshots for UI changes

3. **PR Template**

   ```markdown
   ## Description
   Brief description of changes

   ## Related Issue
   Closes #issue-number

   ## Type of Change
   - [ ] Bug fix
   - [ ] New feature
   - [ ] Breaking change
   - [ ] Documentation update

   ## Changes Made
   - Change 1
   - Change 2

   ## How to Test
   Steps to verify the changes

   ## Screenshots (if applicable)
   Add images here

   ## Checklist
   - [ ] My code follows the style guidelines
   - [ ] I have performed a self-review
   - [ ] I have updated the documentation
   - [ ] My changes generate no new warnings
   - [ ] I have added tests
   ```

4. **Review Process**

   - Maintainers will review your PR
   - Address feedback and comments
   - Update your PR with changes
   - Once approved, your PR will be merged!

## 🐛 Reporting Bugs

### Before Reporting

- Check if the issue already exists
- Try to reproduce with latest code
- Gather relevant information

### Issue Template

```markdown
## Description
Clear description of the bug

## Steps to Reproduce
1. Step 1
2. Step 2
3. Step 3

## Expected Behavior
What should happen

## Actual Behavior
What actually happens

## Environment
- OS: (e.g., Windows 10)
- Node version: (e.g., 18.0.0)
- npm version: (e.g., 8.0.0)

## Screenshots
Add screenshots if applicable

## Additional Context
Any other relevant information
```

## 💡 Feature Requests

Use the [feature request template](https://github.com/kalimireddyreshma/Bigcalendar/issues/new?template=feature-request.md)

```markdown
## Description
What feature would you like?

## Use Case
Why do you need this feature?

## Proposed Solution
How should it work?

## Alternatives
Any alternatives you've considered?
```

## 📚 Documentation

### Update Documentation When

- Adding new features
- Changing API or behavior
- Fixing unclear explanations
- Adding examples

### Documentation Style

- Use clear, simple language
- Include code examples
- Add comments to complex code
- Update README, CONTRIBUTING, or relevant docs

## 🎨 Code Style

### JavaScript/React Standards

```javascript
// ✅ Good
const MyComponent = ({ title, onClick }) => {
  return (
    <div className="my-component">
      <h1>{title}</h1>
      <button onClick={onClick}>Click me</button>
    </div>
  );
};

// ❌ Avoid
var MyComponent = function(props) {
  return (
    <div>
      <h1>{props.title}</h1>
      <button onClick={props.onClick}>Click me</button>
    </div>
  );
};
```

### Naming Conventions

- Components: `PascalCase` (e.g., `CalendarView.jsx`)
- Files: `kebab-case` (e.g., `calendar-view.jsx`)
- Variables/Functions: `camelCase` (e.g., `handleDateChange`)
- Constants: `UPPER_SNAKE_CASE` (e.g., `MAX_EVENTS`)

### Comments

```javascript
// ❌ Avoid obvious comments
const x = 5; // Set x to 5

// ✅ Use meaningful comments
// Calculate total event duration in minutes
const totalDuration = events.reduce((sum, event) => sum + event.duration, 0);
```

## 🔧 Common Tasks

### Running Storybook

```bash
npm run storybook
# Open http://localhost:6006
```

### Build for Production

```bash
npm run build
```

### Clean Install

```bash
rm -rf node_modules package-lock.json
npm install
```

## 📞 Need Help?

- 💬 Ask in [GitHub Discussions](https://github.com/kalimireddyreshma/Bigcalendar/discussions)
- 🐛 Open an [issue](https://github.com/kalimireddyreshma/Bigcalendar/issues)
- 📧 Contact the maintainer

## 🙏 Thank You!

Your contributions make this project better. We appreciate your time and effort!

---

Happy coding! 🚀
