# Project-Based Learning Skill

The **Ultimate CS Tutor** skill for you AI agent. This skill transforms your AI agent into an expert Computer Science tutor that helps you learn programming concepts directly from completed or "vibe-coded" projects in your IDE.

## Features

This skill uses the **Progressive Disclosure** pattern, acting as a dispatcher that dynamically loads one of 5 specialized sub-skills based on your learning goals:

- 🏗️ **Architecture Tutor**: Teaches system design, data flows, tradeoffs, and diagramming.
- 🔬 **Code Review Tutor**: Analyzes code line-by-line using Socratic questioning.
- 🐛 **Bug Hunt Tutor**: The "break it and fix it" mode with difficulty levels (Easy, Medium, Hard).
- 🧹 **Refactoring Tutor**: Challenges you to apply SOLID principles and clean up code smells.
- 📚 **Theory Tutor**: Connects practical, written code to academic CS theory (Big-O analysis, Design Patterns).

## Installation

1. Copy this entire folder (`project-based-learning/`) into your global skills directory at:
   `~/.gemini/config/skills/`
2. You can also place it in a specific project's `.agents/skills/` directory if you only want it available locally.

## Usage

Open any project directory in your IDE and use natural language to trigger the skill. 

**Examples:**
- *"I want to learn programming using this project."*
- *"Help me understand the system architecture of this app."*
- *"I want to do a hard difficulty bug hunt in this project."*
- *"Let's do some Socratic code review on the authentication system."*

The agent will automatically read the main `SKILL.md` dispatcher, figure out your intent, load the appropriate sub-skill from `references/`, and begin your interactive tutoring session!

## Safety First

All interactive coding challenges and bug hunts enforce a strict isolated environment (like a `scratch/` folder or duplicated files) to ensure your actual working project remains completely intact.
