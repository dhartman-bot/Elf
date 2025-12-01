# 25 Days of Elf Magic

An interactive guide to help parents plan Elf on the Shelf scenes for the Christmas season.

## Features

- **25 Days of Scene Ideas** - One for each day from December 1-25
- **Difficulty Ratings** - Easy (5 min), Medium (10-15 min) scenes
- **Alternative Scenes** - Don't have the props? Click for alternatives using common household items
- **Props Checklist** - Interactive checklist to prepare for the month
- **Claude AI Integration** - One-click copy to use with Claude AI for custom letters and more scene ideas

## View the Guide

**Live Site:** [https://dhartman-bot.github.io/Elf/](https://dhartman-bot.github.io/Elf/)

## Using Claude AI

Click the "Copy Instructions for Claude AI" button, then paste into [claude.ai](https://claude.ai) to:
- Generate custom arrival, daily, and goodbye letters
- Get personalized scene ideas based on your available props
- Create nice reports and gentle reminders
- Plan special missions for your kids

## Claude Code Skill

For developers using Claude Code, this repo includes a skill for generating printable PDF letters:

```bash
# Install the skill
cp -r . ~/.claude/commands/elf-on-shelf/

# Then in Claude Code, say:
"Create an elf arrival letter for my kids"
```

## Files

- `index.html` - Main interactive guide (deploy to GitHub Pages)
- `SKILL.md` - Claude Code skill instructions
- `assets/` - Letter template and additional resources
- `references/` - Scene ideas in markdown format

---

Happy Elf Season! 🎄
