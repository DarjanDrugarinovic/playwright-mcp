<!-- Use this file to provide workspace-specific custom instructions to Copilot. For more details, visit https://code.visualstudio.com/docs/copilot/copilot-customization#_use-a-githubcopilotinstructionsmd-file -->

# Playwright MCP Project Instructions

This is a Playwright test automation project for the IOT website. The project focuses on testing user interactions.

## Project Structure

- `/tests/` - Contains all test files
- `playwright.config.ts` - Playwright configuration
- `tsconfig.json` - TypeScript configuration

## Key Guidelines

1. All tests should use TypeScript
2. Follow Page Object Model pattern for complex scenarios
3. Use data-test-id attributes when possible for reliable selectors
4. Include proper wait strategies (waitForLoadState, waitForSelector)
5. Add meaningful assertions and error messages
6. Take screenshots for debugging purposes

## Test Patterns

- Use descriptive test names
- Group related tests using test.describe()
- Include both positive and negative test cases
- Test hover effects and interactive elements
- Verify visual changes and state transitions

## Selectors Priority

1. data-test-id attributes (preferred)
2. Text content for user-visible elements
3. CSS selectors as last resort
4. Avoid XPath unless absolutely necessary

## Common Commands

- `npm run test` - Run all tests
- `npm run test:headed` - Run tests with browser UI
- `npm run test:debug` - Debug tests interactively
- `npm run test:ui` - Run tests with Playwright UI
