# Playwright MCP Test Automation

This project contains automated tests for the spremiispit.com website using Playwright.

## Features

- ✅ TypeScript support
- ✅ Cross-browser testing (Chromium, Firefox, WebKit)
- ✅ HTML test reports
- ✅ Screenshots and traces on failure
- ✅ Test for clicking "Elektronski fakultet" button
- ✅ Test for hover effects

## Installation

1. Clone this repository
2. Install dependencies:
   ```bash
   npm install
   ```
3. Install Playwright browsers (if not already installed):
   ```bash
   npx playwright install
   ```

## Running Tests

### Basic Commands

```bash
# Run all tests
npm run test

# Run tests with browser UI (headed mode)
npm run test:headed

# Debug tests interactively
npm run test:debug

# Run tests with Playwright UI
npm run test:ui

# View test report
npm run test:report

# Generate test code by recording interactions
npm run test:codegen
```

### Test Files

- `tests/elektronski-fakultet.spec.ts` - Tests for the "Elektronski fakultet" button functionality

## Test Scenarios

### 1. Click on Elektronski Fakultet Button

- Navigates to spremiispit.com
- Locates the "Elektronski fakultet" button
- Verifies it's visible
- Clicks on the button
- Takes screenshots before and after clicking

### 2. Hover Effect Verification

- Tests the hover effect on the "Elektronski fakultet" button
- Verifies that the box-shadow changes when hovering
- Ensures visual feedback is working correctly

## Configuration

The project is configured with:

- Base URL: `https://spremiispit.com`
- Screenshots on failure
- Traces on first retry
- Parallel test execution
- HTML reporting

## Project Structure

```
playwright-mcp/
├── tests/
│   └── elektronski-fakultet.spec.ts
├── .github/
│   └── copilot-instructions.md
├── playwright.config.ts
├── tsconfig.json
├── package.json
└── README.md
```

## Browser Support

Tests run on:

- ✅ Chromium (Desktop Chrome)
- ✅ Firefox (Desktop Firefox)
- ✅ WebKit (Desktop Safari)

## Screenshots and Reports

- Screenshots are automatically taken on test failures
- HTML reports are generated after test runs
- Test artifacts are stored in `test-results/` and `playwright-report/` directories

## Development

To add new tests:

1. Create new `.spec.ts` files in the `tests/` directory
2. Use the existing test structure as a template
3. Follow the project's coding guidelines in `.github/copilot-instructions.md`
