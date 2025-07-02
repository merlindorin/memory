# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a newly initialized project called "memory". This repository store various data I want to capture.

## Memory structure

Each memory is stored as a file at root level with an easy to find filename. In each memory, I have this structure:

- Metadata header (YAML front matter):
  - title: The title of the memory
  - date: Creation date in YYYY-MM-DD format
  - keywords: Comma-separated list of relevant keywords
- Quick quote using ">" that abstract quickly the memory (one line or two)
- Table of content (generated)
- Problem
- Solution
- Mitigation (if no solution)
- References

## Project Structure

- Memory files are stored at the root level with descriptive filenames (e.g., `synology-ups-network-connectivity.md`)
- Screenshots and other media assets should be stored in the `assets/` folder
- The main `README.md` should be updated with each new memory entry, organized by category
- When adding images to memory files, reference them as `assets/filename.png`

## Development Setup

Since this is a new project with no established codebase yet, you'll need to:

1. Determine the appropriate programming language and framework based on user requirements
2. Set up the corresponding package management system (npm, pip, cargo, go mod, etc.)
3. Create the initial project structure
4. Initialize any necessary configuration files

## Claude CLI Configuration

The project has Claude CLI configured with the following permissions:
- Allowed: `ls` and `find` bash commands
- Configuration location: `.claude/settings.local.json`

## Git Repository

- Main branch: `main`
- Repository is initialized and clean
- Initial commit already made
