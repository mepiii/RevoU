# Expense & Budget Visualizer

A mobile-friendly web application for tracking daily spending with visual analytics.

## Features

- **Total Balance Indicator** - Real-time balance display with color-coded feedback
- **Transaction Management** - Add, view, and delete transactions with ease
- **Category System** - Pre-built categories (Food, Transport, Fun) with custom category support
- **Visual Analytics** - Interactive donut chart showing spending distribution by category
- **Monthly Summary** - Track income, expenses, and net balance by month
- **Dark/Light Mode** - Toggle between themes with persistent preference

## Tech Stack

- **HTML5** - Semantic structure
- **CSS3** - Custom properties, Grid, Flexbox, animations
- **Vanilla JavaScript** - No frameworks, pure DOM manipulation
- **Chart.js** - Pie/donut chart visualization (via CDN)
- **Inter Font** - Modern sans-serif typography (via Google Fonts)
- **Local Storage** - Client-side data persistence

## Project Structure

```
RevoU/
├── index.html          # Main HTML file
├── css/
│   └── styles.css      # All styles (single file)
├── js/
│   └── app.js          # Application logic (single file)
├── docs/
│   └── superpowers/
│       └── specs/      # Design specifications
└── README.md           # This file
```

## Getting Started

### Prerequisites

- Modern web browser (Chrome, Firefox, Edge, Safari)
- No installation or build process required

### Running Locally

1. Clone or download this repository
2. Open `index.html` in your web browser
3. Start adding transactions!

Alternatively, use a local server:

```bash
# Using Python
python -m http.server 8000

# Using Node.js (npx)
npx serve

# Using PHP
php -S localhost:8000
```

Then visit `http://localhost:8000`

## Usage

### Adding a Transaction

1. Enter the item name (e.g., "Coffee", "Bus ticket")
2. Enter the amount (positive for income, negative for expenses)
3. Select a category from the dropdown
4. Click "Add Transaction"

### Custom Categories

1. Click "+ Add Custom Category"
2. Enter your category name
3. Click the plus button to add
4. New category appears in the dropdown

### Deleting a Transaction

- Click the trash icon next to any transaction
- Click "Undo" in the toast notification to restore

### Viewing Analytics

- The donut chart shows spending by category
- Hover over segments to see amounts and percentages
- Use month arrows to navigate monthly summaries

### Theme Toggle

- Click the sun/moon icon in the header
- Theme preference is saved automatically

## Data Storage

All data is stored in your browser's Local Storage:

```json
{
  "transactions": [
    {
      "id": "unique-id",
      "name": "Item name",
      "amount": 10.00,
      "category": "Food",
      "date": "2026-04-17T20:00:00.000Z"
    }
  ],
  "categories": ["Food", "Transport", "Fun", "Custom"],
  "theme": "light"
}
```

## Browser Support

- Chrome 80+
- Firefox 75+
- Safari 13+
- Edge 80+

## Accessibility

- Keyboard navigation support
- Focus states on all interactive elements
- ARIA labels on icon buttons
- Color contrast meets WCAG AA standards
- Screen reader friendly

## License

MIT License - feel free to use for personal or educational purposes.
