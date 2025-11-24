# CLAUDE.md - AI Assistant Guide for Avengers Repository

This document provides comprehensive guidance for AI assistants working with this repository.

## Repository Overview

**Purpose**: Educational repository for learning Git and GitHub workflows, themed around Marvel's Avengers.

**Language**: Spanish (all content, commit messages, and documentation are in Spanish)

**Source Attribution**: All information is sourced from Wikipedia and Marvel.com

## Repository Structure

```
/home/user/avengers/
├── README.md           # Main repository description
├── miembros.md         # List of Avengers team members
├── villanos.md         # List of villains/antagonists
├── misiones.md         # List of missions/objectives
└── CLAUDE.md          # This file - AI assistant guidance
```

### File Descriptions

- **README.md**: Entry point explaining the repository's purpose as a Git/GitHub learning environment
- **miembros.md**: Maintains the roster of Avengers members (currently 19 members including Iron Man, Captain America, Thor, etc.)
- **villanos.md**: Tracks villains and antagonists (currently Dr. Doom and Red Skull)
- **misiones.md**: Lists active missions and objectives for the team

## Development Workflows

### Git Workflow

The repository follows a **feature branch workflow** with pull requests:

1. **Branch Naming Conventions**:
   - Feature branches: descriptive names in Spanish (e.g., `rama-misiones`)
   - AI assistant branches: Must follow format `claude/claude-md-*` with session ID
   - All development happens on feature branches, never directly on main

2. **Commit Message Conventions**:
   - Written in Spanish
   - Clear, descriptive messages explaining the change
   - Reference issues when applicable using `fixes #<issue-number>` or similar
   - Examples from history:
     - "Agregamos a Nick fixes #4"
     - "Actualizacion de misiones - Red Skull"
     - "El capi se volvio loco y ahora es malo"

3. **Pull Request Workflow**:
   - Feature branches are merged via pull requests
   - PRs should be reviewed before merging
   - Merge commits preserve branch history
   - Example: PR #2 merged `rama-misiones` branch

### Branch Strategy

- **Main/Master Branch**: Protected, stable version
- **Feature Branches**: Short-lived branches for specific features or updates
- **Claude Branches**: Session-specific branches for AI assistant work (format: `claude/claude-md-*`)

## Content Conventions

### Language and Style

- **Primary Language**: Spanish
- **Tone**: Informal and educational
- **Format**: Markdown with simple formatting
- **Lists**: Use bullets (`*`) for unordered lists, numbers for ordered lists

### File Modification Guidelines

#### miembros.md
- Add new members to the bulleted list
- Keep alphabetical order not required (chronological addition is acceptable)
- One member per line with bullet point
- Use proper character names from Marvel canon

#### villanos.md
- Use numbered list format
- One villain per line
- Keep it simple - just the villain name

#### misiones.md
- Use bulleted list with asterisks
- Each mission should be action-oriented
- Keep descriptions brief and clear
- Missions can reference villains or team objectives

### Content Integrity

- All characters and information should be Marvel canon
- Reference Wikipedia or Marvel.com for accuracy
- Maintain the Avengers theme consistently
- Don't add non-Marvel characters or break theme

## Key Conventions for AI Assistants

### When Modifying Content

1. **Always Read First**: Read the relevant file before making changes to understand current content
2. **Respect Language**: All additions/modifications must be in Spanish
3. **Maintain Format**: Preserve existing markdown formatting and list styles
4. **Stay On Theme**: Only add Marvel-related content that fits the repository purpose
5. **Commit Properly**: Write clear commit messages in Spanish that explain what was changed

### When Adding Members (miembros.md)

- Verify the character is an Avenger in Marvel canon
- Add to the end of the list unless specifically asked to reorder
- Use the character's Spanish or commonly known name
- Format: `* Character Name`

### When Adding Villains (villanos.md)

- Verify the villain has faced the Avengers in Marvel canon
- Add to the end of the numbered list
- Format: `N. Villain Name` (where N is the next number)

### When Adding Missions (misiones.md)

- Make missions relevant to existing villains or Avengers storylines
- Use action verbs in Spanish (Investigar, Capturar, Detener, etc.)
- Format: `* Mission description`
- Keep missions concise

### Git Operations for AI Assistants

1. **Always work on the assigned claude/* branch**
2. **Never push to main/master directly**
3. **Create clear commits** after each logical change
4. **Push when work is complete** using: `git push -u origin <branch-name>`
5. **Branch names must match** the session ID pattern for successful push

### Common Operations

**Adding a new member:**
```bash
# 1. Read miembros.md first
# 2. Add the member in proper format
# 3. Commit: "Agregamos a [Character Name]"
# 4. Push to claude/* branch
```

**Adding a villain:**
```bash
# 1. Read villanos.md first
# 2. Add with next number in sequence
# 3. Commit: "Agregamos villano [Villain Name]"
# 4. Push to claude/* branch
```

**Adding a mission:**
```bash
# 1. Read misiones.md first
# 2. Add mission with bullet point
# 3. Commit: "Nueva mision: [brief description]"
# 4. Push to claude/* branch
```

## Testing and Validation

Since this is a documentation-focused repository:

1. **Syntax Check**: Ensure markdown is properly formatted
2. **Content Validation**: Verify character names are spelled correctly
3. **Canon Check**: Confirm additions align with Marvel universe
4. **Language Check**: Ensure all content is in Spanish

## Issue References

- Issues are tracked in GitHub
- Reference issues in commit messages using `fixes #N` or `closes #N`
- Example from history: "Agregamos a Nick fixes #4"

## Historical Context

The repository has evolved through:
- Initial setup with basic structure
- Addition of villains and members
- Creation of missions system
- Multiple feature branch merges via PRs
- Bug fixes and content updates

Key patterns from history:
- Content additions are incremental
- Each feature gets its own branch
- Team uses Spanish throughout
- Simple, clear commit messages
- Pull request workflow is standard

## Best Practices for AI Assistants

1. **Read Before Modify**: Always read files before editing
2. **Small Commits**: Make focused commits for each logical change
3. **Spanish First**: All content and commits in Spanish
4. **Theme Consistency**: Maintain Avengers/Marvel theme
5. **Format Preservation**: Keep existing markdown styles
6. **Branch Discipline**: Work only on assigned branches
7. **Clear Communication**: Commit messages should explain what and why
8. **Canon Compliance**: Verify information against Marvel sources

## Error Prevention

- **Don't** add non-Marvel characters
- **Don't** mix languages (English/Spanish)
- **Don't** break markdown formatting
- **Don't** commit to wrong branch
- **Don't** make assumptions about character details - verify first
- **Don't** create new file types unless specifically requested
- **Don't** over-engineer - keep it simple like existing content

## Current State (as of latest commit)

- **Current Branch**: `claude/claude-md-midoa9xju4v58rmy-01AmW2tbHn6WyhdsZW1dTemZ`
- **Members**: 19 Avengers listed
- **Villains**: 2 villains (Dr. Doom, Red Skull)
- **Missions**: 2 active missions
- **Last Update**: Nick Fury added (fixes #4)
- **Status**: Clean working directory

## Quick Reference Commands

```bash
# View current status
git status

# View file structure
ls -la

# Read a file
cat miembros.md

# View recent commits
git log --oneline -10

# View all branches
git branch -a

# Push changes (use correct branch name)
git push -u origin claude/claude-md-*
```

## Questions to Ask Before Making Changes

1. Is this content Marvel/Avengers related?
2. Should this be in Spanish?
3. Have I read the target file first?
4. Am I on the correct branch?
5. Does this follow the existing format?
6. Is my commit message clear and in Spanish?
7. Have I verified this information is canon?

## Summary

This is a simple, educational repository with clear conventions:
- **Spanish language** for all content
- **Marvel Avengers theme** strictly maintained
- **Feature branch workflow** with pull requests
- **Simple markdown files** for easy editing
- **Clear, descriptive commits** in Spanish
- **Issue tracking** through GitHub

Keep modifications simple, on-theme, and properly formatted. When in doubt, maintain consistency with existing content patterns.
