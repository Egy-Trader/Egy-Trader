# GitHub Copilot Instructions – Static Stock Trading Education Website (Arabic – Egyptian Dialect)

## Repository Purpose

This repository contains a **static educational website** hosted on **GitHub Pages**.
The website explains **stock market trading concepts** in **Egyptian Arabic dialect**, targeting beginners and intermediate learners.

The site focuses on:
- Trading tools and how to use them
- Well-known chart patterns (e.g. Double Top)
- Key economic and financial indicators (e.g. M2, P/E)
- Explaining concepts using **simple language**, **card-based UI**, and **RTL layout**

The content is educational only and does not provide financial advice.

---

## High-Level Project Information

- **Project Type:** Static Website
- **Hosting:** GitHub Pages
- **Languages:**  
  - HTML (structure)  
  - CSS (custom styling, RTL, cards)  
  - JavaScript (optional, light enhancements only)

- **Frameworks:** None (plain HTML/CSS/JS only)
- **Target Audience:** Arabic-speaking users (Egyptian dialect)
- **Text Direction:** Right-To-Left (RTL)

No backend, build system, or package manager is used.

---

## Global Content & Style Rules (CRITICAL)

Copilot **must strictly follow** these rules when generating or editing any file:

1. **Language**
   - All text must be written in **Arabic Egyptian dialect**
   - Avoid MSA/formal Arabic
   - Tone should be friendly, educational, and simple

2. **RTL Layout**
   - Every HTML page must use RTL:
     ```html
     <html lang="ar" dir="rtl">
     ```
   - CSS must include:
     ```css
     body {
       direction: rtl;
       text-align: right;
     }
     ```

3. **Card-Based Design**
   - All content sections must be inside cards
   - No long continuous text blocks
   - Each concept = one card

4. **No Frameworks**
   - Do NOT use Bootstrap, Tailwind, React, Vue, etc.
   - Use **custom CSS only**

5. **Static Only**
   - No APIs, no backend, no build steps
   - Pure static content compatible with GitHub Pages

---

## Website Structure (Expected Pages)

### 1. Home Page (`index.html`)
Purpose:
- Introduce stock market trading
- Explain what the site offers

Must include cards explaining:
- What is stock trading (simple Egyptian Arabic)
- Who this site is for
- Navigation cards linking to other pages:
  - Tools
  - Chart Patterns
  - Indicators

---

### 2. Tools Page (`tools.html`)
Purpose:
Explain common trading tools.

Each tool must be in **one card** with:
- Tool name
- Simple usage explanation
- Practical benefit

Must include (at minimum):
- Trading platforms
- Stock screeners
- Charting tools
- News & economic calendars

Language example style:
> "الأداة دي بتخليك تشوف الأسهم اللي بتنطبق عليها شروط معينة بدل ما تدور يدوي"

---

### 3. Chart Types Page (`charts.html`)
Purpose:
Explain famous chart patterns **from a liquidity & order-flow perspective**.

Each chart pattern must:
- Be in its own card
- Explain:
  - Shape of the pattern
  - What happens to liquidity
  - Buy vs sell order behavior
  - Why price reverses or continues

Must include at least:
- Double Top
- Double Bottom
- Head and Shoulders

Example explanation focus:
- Where sellers appear
- Where buyers fail
- Why smart money exits

---

### 4. Indicators Page (`indicators.html`)
Purpose:
Explain well-known economic & financial indicators.

Each indicator card must include:
- What the indicator measures
- Why it matters to stock markets
- Simple real-world explanation
- At least **one external reference link**

Must include at least:
- M2 Money Supply
- P/E Ratio
- Interest Rates

External links must be reputable (e.g. Investopedia, central banks).

---

## CSS Architecture

Expected files:
/assets/css/styles.css

CSS must include:
- RTL handling
- Card styling
- Clean readable layout
- Neutral colors (white cards, light background)

Example card class:
```css
.card {
  background: #ffffff;
  border-radius: 8px;
  padding: 16px;
  margin-bottom: 16px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.1);
}
```
## JavaScript Usage
- JavaScript Usage (If Any)
-- Optional only
-- Allowed uses:
--- Menu toggles

Simple interactivity
- Forbidden:
--- Frameworks
--- Complex logic
--- API calls

## Repository Layout (Expected)

├─ index.html
├─ tools.html
├─ charts.html
├─ indicators.html
├─ assets/
│  ├─ css/
│  │  └─ styles.css
│  └─ js/
│     └─ main.js (optional)
└─ .github/
   └─ copilot-instructions.md