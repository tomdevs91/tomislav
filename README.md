# Tomislav TypeScript App

A basic TypeScript application with Express.js server and automatic AWS deployment.

## Features

- **TypeScript**: Strict TypeScript configuration for type safety
- **Express.js**: Web server with REST API endpoints
- **Auto-deployment**: GitHub Actions automatically deploys to AWS EC2
- **Health checks**: Built-in health monitoring endpoint
- **Error handling**: Comprehensive error handling middleware

## API Endpoints

- `GET /` - Welcome message with timestamp
- `GET /health` - Health check with system info
- `GET /api/hello/:name?` - Personalized greeting endpoint

## Development

```bash
# Install dependencies
npm install

# Development mode (with hot reload)
npm run dev

# Build TypeScript
npm run build

# Start production server
npm start

# Watch mode for development
npm run watch
```

## Deployment

This project automatically deploys to AWS EC2 when pushed to the main branch via GitHub Actions.

**Deployment Details:**
- **Server**: AWS EC2 (63.178.163.229)
- **Location**: `/root/CLAUDE/tomislav`
- **Trigger**: Push to main branch
- **Duration**: 2-3 minutes

## Project Structure

```
tomislav/
├── src/
│   └── index.ts          # Main application file
├── dist/                 # Compiled JavaScript (generated)
├── .github/
│   └── workflows/
│       └── deploy.yml    # GitHub Actions deployment
├── package.json          # Dependencies and scripts
├── tsconfig.json         # TypeScript configuration
├── .gitignore           # Git ignore rules
└── README.md            # This file
```

## Technology Stack

- **Runtime**: Node.js
- **Language**: TypeScript
- **Framework**: Express.js
- **Deployment**: GitHub Actions + AWS EC2
- **Organization**: testingceres

## Getting Started

1. Clone the repository
2. Run `npm install`
3. Start development with `npm run dev`
4. Push to main branch for automatic deployment

The application will be automatically deployed to AWS within 2-3 minutes of pushing to GitHub.
