# Cezerin Platform

Cezerin is a modern eCommerce platform built with React and Node.js, offering a robust and scalable solution for online shopping. The platform is divided into several components:

- **Cezerin API**: Backend services that handle eCommerce functionalities.
- **Cezerin Store**: Frontend React application for the shopping experience.
- **Cezerin Admin**: Dashboard for managing store data and configurations.
- **Cezerin Client**: JavaScript client for interacting with the Cezerin REST API.

## Built With

- **Node.js**
- **React.js**
- **Redux**
- **Express.js**

## Quick Start

1. **Run Setup Script**
   - Execute the `setup.sh` script to set up the environment.

2. **Set Up MongoDB Collections**
   - Run `yarn setup` from the command line in the project folder to configure the necessary MongoDB collections.


## Application Structure

├── config # Project and build configurations
├── dist # Distribution folder
├── locales # Text files
├── logs # Log files
├── public # Static public assets and uploads
│ ├── admin # Dashboard index.html
│ ├── admin-assets # Dashboard assets
│ └── content # Store root folder
|
├── scripts # Shell scripts for theme install/export
├── src # Application source code
│ ├── admin # Dashboard application
│ │ └── client # Client-side code
│ ├── api # REST API
│ │ └── server # Server-side code
│ ├── store # Store application
│ │ ├── client # Client-side code
│ │ ├── server # Server-side code
│ │ └── shared # Universal code
│ └── index.js # Server application start point
├── theme # Theme as a local package
└── process.json # PM2 process file

## NPM Scripts

| Command                   | Description                                       |
|---------------------------|---------------------------------------------------|
| `setup`                   | Run Cezerin MongoDB setup.                       |
| `compile`                 | Compiles the store to disk (`~/dist` by default).|
| `compile:watch`           | Compiles the store and theme to disk and watch. |
| `webpack:admin`           | Assemble admin bundles.                          |
| `webpack:store`           | Assemble store bundles.                          |
| `webpack:admin:watch`     | Assemble admin bundles and watch.                |
| `webpack:store:watch`     | Assemble store bundles and watch.                |
| `theme:install`           | Install theme from `/public/.zip`.               |
| `theme:export`            | Zip the current theme to `/public/.zip`.         |
| `theme:compile`           | Compile the theme after modification.           |
| `theme:build`             | Refresh the theme after modification.           |
| `build`                   | Compile and assemble bundles.                    |
| `build:watch`             | Compile and assemble bundles and watch.         |
| `lint`                    | Check project with ESLint.                       |
| `lint:fix`                | Check and fix project with ESLint.              |
| `format`                  | Format project with Prettier.                    |
| `start:api`               | Start the Node server.                           |
| `start:store`             | Start the store server.                          |
| `start`                   | Start the Cezerin platform.                      |
| `watch:api`               | Start the Node server and watch.                |

For more information or troubleshooting, please refer to the official [Cezerin documentation](https://github.com/Cezerin2/Cezerin2).
