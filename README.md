# BTD 5 Game Project

## Overview

This is a web-based Bloons Tower Defense 5 (BTD 5) game implementation using Flash/ActionScript content rendered through the Ruffle Flash emulator. The project serves as a browser-based gaming platform that allows users to play BTD 5 directly in modern web browsers without requiring Flash Player. The application includes domain-specific customization features to appear as different types of sites based on the hosting domain.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Static HTML Structure**: Single-page application with minimal HTML markup focused on game container
- **Flash Emulation**: Utilizes Ruffle-rs library to emulate Flash content in modern browsers without Flash Player dependency
- **Responsive Design**: Full-screen game layout that adapts to browser viewport dimensions
- **Domain-Based Customization**: Dynamic title and favicon switching based on hosting domain for stealth/educational purposes

### Client-Side Rendering
- **JavaScript-Driven**: DOM manipulation for dynamic content updates based on environment
- **CSS Styling**: Minimal styling focused on full-screen game presentation with black background
- **Asset Management**: Dynamic favicon loading based on domain detection

### Security and Access Considerations
- **Stealth Features**: Includes domain detection logic to disguise the game as educational content on specific domains
- **Analytics Integration**: Google Analytics tracking for user engagement monitoring

## External Dependencies

### Third-Party Libraries
- **Ruffle Flash Emulator**: Core dependency for Flash content rendering (`@ruffle-rs/ruffle` via unpkg CDN)
- **Google Analytics**: User tracking and engagement analytics (`gtag.js`)

### Hosting Platforms
- **Vercel**: Primary hosting platform with support for multiple domain configurations
- **CDN Services**: unpkg.com for JavaScript library delivery

### Asset Dependencies
- **Game Assets**: Flash-based BTD 5 game files (implied but not visible in current file structure)
- **Static Images**: Favicon and stealth mode images (`bitbot.png`, `coolthing.png`)

### Browser Compatibility
- **Modern Browser Support**: Relies on Ruffle's WebAssembly implementation for cross-browser Flash emulation
- **JavaScript ES6+**: Uses modern JavaScript features like `addEventListener` and `const`/`let` declarations
