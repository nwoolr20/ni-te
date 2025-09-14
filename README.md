# @NiTE

A modern mobile application built with Ionic Framework and Vue 3, featuring a responsive sidebar navigation and folder-based organization system.

## Overview

`@NiTE` showcases how to build a cross-platform mobile application with Ionic and Vue 3. It provides a mailbox-style layout with folder-based navigation and simple label management, demonstrating how familiar email workflows can be implemented with modern web technologies.

## Features

- 📱 Cross-platform mobile app (iOS, Android, and PWA)
- 🎨 Modern UI with Ionic components
- 📂 Folder-based navigation (Inbox, Outbox, Favorites, Archived, Trash, Spam)
- 🏷️ Label management system
- 📱 Responsive design with native mobile feel
- ⚡ Built with Vue 3 and TypeScript for performance and type safety

## Technologies Used

- **Framework**: [Ionic Framework](https://ionicframework.com/) v5.4+
- **Frontend**: [Vue 3](https://vuejs.org/) with TypeScript
- **Mobile Runtime**: [Capacitor](https://capacitorjs.com/) v3.1+
- **Routing**: Vue Router v4
- **Build Tool**: Vue CLI
- **Testing**: Jest (unit tests) + Cypress (e2e tests)
- **Linting**: ESLint with Vue and TypeScript support

## Prerequisites

Before you begin, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (version 14 or higher)
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)
- [Ionic CLI](https://ionicframework.com/docs/cli) (optional but recommended)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/nwoolr20/ni-te.git
cd ni-te
```

2. Install dependencies:
```bash
npm install
```

> **Note**: This project uses older dependencies that may show warnings on newer Node.js versions (18+). The application should still function correctly despite these warnings.

3. Start the development server:
```bash
npm run serve
```

The application will be available at `http://localhost:8080`.

## Available Scripts

### Development
- `npm run serve` - Start development server with hot reload
- `npm run build` - Build the project for production
- `npm run lint` - Run ESLint to check code quality

> **Note**: Some npm scripts may require dependency updates to work with newer Node.js versions. The core functionality remains intact.

### Testing
- `npm run test:unit` - Run unit tests with Jest
- `npm run test:e2e` - Run end-to-end tests with Cypress

## Project Structure

```
ni-te/
├── public/                 # Public assets
│   ├── index.html         # Main HTML file
│   └── assets/            # Static assets
├── src/
│   ├── components/        # Reusable Vue components
│   ├── router/            # Vue Router configuration
│   │   └── index.ts       # Route definitions
│   ├── theme/             # CSS theme variables
│   │   └── variables.css  # Ionic CSS custom properties
│   ├── views/             # Page components
│   │   └── Folder.vue     # Folder view component
│   ├── App.vue            # Root Vue component
│   └── main.ts            # Application entry point
├── tests/
│   ├── e2e/               # End-to-end tests
│   └── unit/              # Unit tests
├── capacitor.config.json  # Capacitor configuration
├── ionic.config.json      # Ionic CLI configuration
└── package.json           # Project dependencies and scripts
```

## Mobile Development

This app is built with Capacitor for native mobile deployment.

### Building for Mobile

1. Build the web assets:
```bash
npm run build
```

2. Add your target platform:
```bash
npx cap add ios
npx cap add android
```

3. Sync the web code with native projects:
```bash
npx cap sync
```

4. Open in native IDE:
```bash
npx cap open ios     # Opens in Xcode
npx cap open android # Opens in Android Studio
```

## Navigation Structure

The app features a sidebar navigation with the following sections:

### Main Folders
- **Inbox** - Main message area
- **Outbox** - Sent items
- **Favorites** - Starred content
- **Archived** - Stored items
- **Trash** - Deleted items
- **Spam** - Filtered content

### Labels
- Family
- Friends
- Notes
- Work
- Travel
- Reminders

## Configuration

### Capacitor
Configure native app settings in `capacitor.config.json`:
- App ID: `io.ionic.starter`
- App Name: `@NiTE`
- Web Directory: `dist`

### Ionic
Ionic configuration is managed in `ionic.config.json`:
- Project Type: Vue
- Capacitor integration enabled

## Development Guidelines

### Code Style
- Use TypeScript for type safety
- Follow Vue 3 Composition API patterns
- Maintain consistent ESLint configuration
- Use Ionic components for UI consistency

### Testing
- Write unit tests for business logic
- Add e2e tests for user workflows
- Maintain test coverage for critical paths

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Run tests and linting
5. Submit a pull request

## License

This project is private and all rights are reserved.

## Support

For questions or issues, please contact the development team or create an issue in the repository.
