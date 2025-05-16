# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This project is a single-page web application called "PyWheel Manager" that helps users manage Python wheel dependencies. The application allows users to:

1. Analyze dependencies for Python packages
2. Download wheel files for offline installation
3. Generate installation commands for offline package installation

The project consists of a single HTML file with embedded CSS and JavaScript.

## Key Components

- **User Interface**: HTML/CSS-based interface with forms for package configuration
- **PyPI Integration**: JavaScript functions to fetch package information from PyPI
- **Dependency Analysis**: Logic to recursively analyze package dependencies
- **Wheel Selection**: Algorithm to select the most appropriate wheel file based on Python version, platform, and architecture
- **Download Management**: Functions to download wheel files individually or in bulk

## Development Notes

### Testing

To test the application, simply open `wheels.html` in a web browser. The application runs entirely in the browser and uses fetch API to communicate with PyPI.

### Browser Compatibility

The application uses modern JavaScript features and the File System Access API for bulk downloads. This feature is currently only supported in Chromium-based browsers.

### Future Enhancements

Potential areas for improvement:
- Enhanced error handling for network issues
- Better wheel file matching for platforms
- Support for version constraints in dependencies
- Offline mode using cached PyPI data