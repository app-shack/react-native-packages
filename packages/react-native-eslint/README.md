# @martinagnalv/react-native-eslint

A comprehensive ESLint configuration for React Native projects with TypeScript support. This package provides a well-tested, opinionated set of ESLint rules specifically tailored for React Native development.

## Features

- 🚀 React Native optimized rules
- 📱 TypeScript support with strict type checking
- ⚡ ESLint 9 flat config format
- 🎯 Jest testing rules included
- 🎨 Stylistic rules for consistent code formatting
- 🔧 Promise-based async/await best practices
- 🛡️ Security-focused React rules

## Installation

```bash
npm install --save-dev @martinagnalv/react-native-eslint
```

Or with yarn:

```bash
yarn add --dev @martinagnalv/react-native-eslint
```

## Usage

Create an `eslint.config.mjs` file in your project root:

```javascript
import reactNativeConfig from '@martinagnalv/react-native-eslint'

export default reactNativeConfig
```

Or extend it with additional configuration:

```javascript
import reactNativeConfig from '@martinagnalv/react-native-eslint'

export default [
  ...reactNativeConfig,
  {
    // Your custom rules here
    rules: {
      // Override or add rules
      'no-console': 'warn'
    }
  }
]
```

## What's Included

This configuration includes rules for:

- **JavaScript/TypeScript**: Core language rules and TypeScript-specific linting
- **React**: React best practices and hooks rules  
- **React Native**: Platform-specific rules for React Native development
- **Jest**: Testing rules and best practices
- **Promises**: Async/await and Promise handling
- **Stylistic**: Code formatting and style consistency

## Scripts

Add these scripts to your `package.json`:

```json
{
  "scripts": {
    "lint": "eslint .",
    "lint:fix": "eslint . --fix"
  }
}
```

## Requirements

- Node.js >= 18.0.0
- ESLint >= 9.0.0
- TypeScript project

## License

MIT © [App Shack](https://github.com/app-shack)

## Contributing

Issues and pull requests are welcome! Please check the [issues page](https://github.com/app-shack/react-native-eslint/issues) before contributing.

---

## Publishing Notes

To publish this package, you need to set up an NPM auth token:

```sh
echo 'export NPM_AUTH_TOKEN=<YOUR_TOKEN>' >> ~/.zshrc
source ~/.zshrc

# or for bash
echo 'export NPM_AUTH_TOKEN=<YOUR_TOKEN>' >> ~/.bashrc
source ~/.bashrc
```