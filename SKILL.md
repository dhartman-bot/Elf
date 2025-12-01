---
name: elf-on-shelf
description: Create printable Elf on the Shelf letters, notes, and scene ideas for the Christmas season. This skill should be used when creating elf arrival letters, goodbye letters, daily notes from the elf, naughty/nice reports, or brainstorming creative elf scene setups. Generates festive, kid-friendly HTML letters that convert to one-page printable PDFs.
---

# Elf on the Shelf Letter & Scene Creator

Create magical, personalized letters and notes from your family's Elf on the Shelf, plus creative scene ideas for the Christmas season.

## Letter Types

1. **Arrival Letter** - Elf returns for the season, sets expectations
2. **Daily Note** - Short notes explaining what elf did overnight
3. **Nice Report** - Praise for good behavior
4. **Gentle Reminder** - Kind nudge about behavior
5. **Special Mission** - Elf assigns kids a fun task
6. **Goodbye Letter** - Christmas Eve farewell

## Creating a Letter

### Step 1: Gather Information
- Children's names
- Elf's name
- Letter type
- Special context (baby elf, behavior to address, etc.)

### Step 2: Generate HTML Letter
Use the template structure in `assets/letter_template.html`. Key elements:

**Fonts (Google Fonts):**
- Headers: `Mountains of Christmas` - whimsical, festive
- Body: `Caveat` - handwritten look

**Colors:**
- Christmas Red: `#c41e3a` (headers, signature)
- Forest Green: `#2d5a27` (body text)
- Dark Green: `#1a472a` (subheadings)
- Snowflake Blue: `#87ceeb`
- Background: `#fffef5` to `#fff8e7` gradient

**One-Page Print Sizing:**
- Body font: 17px, line-height: 1.4
- Tight margins: 0.25in padding
- Section margins: 10px
- Border: 6px double red

### Step 3: Convert to PDF
```bash
/Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome --headless --disable-gpu --print-to-pdf=/Users/dhartman/Desktop/[filename].pdf --no-margins /Users/dhartman/Desktop/[filename].html
```

Then open the PDF for review.

## Scene Ideas

See `references/scene_ideas.md` for 25 days of creative setups organized by:
- **Easy** - 5 minutes, minimal props
- **Medium** - 10-15 minutes, some props
- **Elaborate** - 20+ minutes, multiple props

Each scene includes setup instructions, props needed, and optional accompanying notes.

## Template Structure

```html
<div class="letter-container">
  <!-- Corner decorations -->
  <div class="header">
    <h1>Title with snowflakes</h1>
    <div class="from-north-pole">OFFICIAL ELF CORRESPONDENCE</div>
  </div>
  <div class="snowflakes">Row of snowflake emojis</div>
  <div class="greeting">Dear [NAMES],</div>
  <div class="letter-body">
    <p>Main content...</p>
    <div class="special-section">Highlighted box for missions/rules</div>
  </div>
  <div class="closing">
    <p>Signature line</p>
    <p class="signature">Elf Name</p>
  </div>
  <p class="ps">P.S. message</p>
  <div class="footer-decoration">Holiday emojis</div>
</div>
```

## Resources

- `assets/letter_template.html` - Complete HTML/CSS template
- `references/scene_ideas.md` - 25 days of scene setups with difficulty ratings
