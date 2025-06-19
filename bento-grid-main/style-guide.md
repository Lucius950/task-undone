<!-- # Front-end Style Guide

## Layout

The designs were created to the following widths:

- Mobile: 375px
- Desktop: 1440px

> 💡 These are just the design sizes. Ensure content is responsive and meets WCAG requirements by testing the full range of screen sizes from 320px to large screens.

## Colors

- Purple 100: hsl(254, 88%, 90%)
- Purple 500: #7650dc

- Yellow 100: hsl(31, 66%, 93%)
- Yellow 500: hsl(39, 100%, 71%)

- White: hsl(0, 0%, 100%)
- Black: hsl(0, 0%, 7%)

## Typography

### Body Copy

- Font size (paragraph): 18px

### Font

- Family: [DM Sans](https://fonts.google.com/specimen/DM+Sans)
- Weights: 400, 500

> 💎 [Upgrade to Pro](https://www.frontendmentor.io/pro?ref=style-guide) for design file access to see all design details and get hands-on experience using a professional workflow with tools like Figma. The design file for this challenge also includes a design system and tablet layout to help you build a more accurate solution faster. -->



/* Reset & base */
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  font-family: sans-serif;
  background: #f9fafb;
  color: #333;
  padding: 20px;
}

/* Grid layout */
.grid-container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
   grid-auto-rows: min-content;
  gap: 20px;
}

/* Hero spans all columns */
.hero {
  grid-column: 1 / -1;
  background: #3b82f6;
  color: #fff;
  padding: 30px;
  border-radius: 12px;
  text-align: center;
}
.hero .highlight {
  color: #fbbf24;
}
.hero .stars {
  font-size: 1.2em;
  margin: 10px 0;
}
.hero .sub {
  opacity: 0.8;
}

/* Cards */
.card {
  background: #fff;
  padding: 20px;
  border-radius: 12px;
  position: relative;
}
.card.yellow { background: #fbbf24; color: #333; }
.card.blue   { background: #3b82f6; color: #fff; }
.card.purple { background: #c4b5fd; color: #333; }

.card.small { font-size: 0.9em; }
.card.chat { display: flex; flex-direction: column; }

.card h2, .card h3 {
  margin-bottom: 10px;
}

/* Buttons */
.btn {
  background: #fff;
  color: inherit;
  border: none;
  padding: 10px 20px;
  border-radius: 6px;
  cursor: pointer;
  font-weight: bold;
}

/* Bar charts */
.bar-chart {
  display: flex;
  align-items: flex-end;
  gap: 8px;
  height: 80px;
  margin: 10px 0;
}
.bar-chart.small { height: 50px; }
.bar {
  flex: 1;
  background: currentColor;
  opacity: 0.7;
  border-radius: 4px 4px 0 0;
}

/* Chat box */
.chat-box {
  background: rgba(255,255,255,0.8);
  padding: 10px;
  border-radius: 8px;
  font-size: 0.85em;
  line-height: 1.4;
}

/* Calendar */
.calendar {
  background: rgba(255,255,255,0.8);
  padding: 10px;
  border-radius: 8px;
  font-size: 0.85em;
}
.weekdays {
  display: flex;
  justify-content: space-between;
  margin-top: 5px;
}
.weekdays div {
  width: 20%;
  text-align: center;
}

/* Stats & avatars */
.stat {
  text-align: center;
}
.stat h1 {
  font-size: 2.5em;
}
.avatars {
  display: flex;
  justify-content: center;
  gap: 5px;
  margin-top: 10px;
}
.avatar {
  font-size: 1.5em;
}

/* Followers growth card */
.stats {
  display: flex;
  justify-content: space-between;
  align-items: flex-end;
}
.stats h3 {
  margin: 0;
}
.stats p {
  font-size: 0.85em;
  opacity: 0.8;
}