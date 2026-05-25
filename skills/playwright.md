# Playwright Skill

## Overview
Expertise in Playwright for end-to-end testing of web applications.

## Core Concepts

### Browser Support
- Chromium (Chrome, Edge)
- Firefox
- WebKit (Safari)

### Key Features
- Auto-waiting for elements
- Cross-browser testing
- Mobile emulation
- Network interception
- Video recording

## Installation

```bash
npm install -D @playwright/test
npx playwright install
```

## Test Structure

### Basic Test
```javascript
import { test, expect } from '@playwright/test';

test('should display welcome message', async ({ page }) => {
  await page.goto('/'); 
  await expect(page.getByText('Welcome')).toBeVisible();
});
```

### Test Fixtures
- `page`: Browser page instance
- `context`: Browser context
- `browser`: Browser instance
- `browserName`: Current browser name

## Locators

### Built-in Locators
- `getByText()`: Text content
- `getByPlaceholder()`: Placeholder text
- `getByLabel()`: Label text
- `getByRole()`: ARIA roles
- `getByAltText()`: Alt text
- `getByTitle()`: Title attribute

### CSS Selectors
- `locator('css=selector')`
- `locator('xpath=//xpath')`

## Actions

### Navigation
- `page.goto(url, options)`
- `page.reload()`
- `page.goBack()`
- `page.goForward()`

### Input
- `locator.fill(value)`
- `locator.type(text, options)`
- `locator.clear()`

### Click
- `locator.click(options)`
- `locator.dblclick()`
- `locator.hover()`

### Assertions
- `expect(locator).toBeVisible()`
- `expect(locator).toBeEnabled()`
- `expect(locator).toHaveText()`
- `expect(locator).toHaveValue()`
- `expect(page).toHaveURL()`

## Advanced Features

### Network Interception
```javascript
await page.route('**/api/**', route => {
  route.continue({ 
    headers: { ...route.request().headers() } 
  });
});
```

### Mocking
```javascript
await page.route('**/api/users', route => {
  route.fulfill({
    status: 200,
    body: JSON.stringify(mockUsers)
  });
});
```

### Mobile Emulation
```javascript
const iPhone = playwright.devices['iPhone 13'];
const context = await browser.newContext({
  ...iPhone
});
```

### Video Recording
```javascript
const context = await browser.newContext({
  recordVideo: {
    dir: 'videos/'
  }
});
```

## Parallel Testing

### Test Parallelization
```bash
npx playwright test --workers=4
```

### Sharding
```bash
npx playwright test --shard=1/4
npx playwright test --shard=2/4
```

## Reporting

### HTML Reporter
```bash
npx playwright test --reporter=html
```

### JSON Reporter
```bash
npx playwright test --reporter=json
```

### Allure Reporter
```bash
npm install -D @allure/playwright
npx playwright test --reporter=allure-playwright
```

## CI/CD Integration

### GitHub Actions
```yaml
- name: Run Playwright tests
  run: npx playwright test

- name: Upload test results
  uses: actions/upload-artifact@v3
  if: always()
  with:
    name: playwright-report
    path: playwright-report/
```

### Docker
```dockerfile
FROM mcr.microsoft.com/playwright:v1.40.0-jammy
COPY . /app
WORKDIR /app
RUN npm ci
CMD ["npx", "playwright", "test"]
```

## Best Practices

1. Use auto-waiting instead of `setTimeout`
2. Prefer built-in locators over CSS selectors
3. Use test IDs for reliable element targeting
4. Implement page object model for large test suites
5. Run tests in headless mode for CI
6. Use test isolation (fresh context per test)
7. Capture screenshots on failure
8. Use trace viewer for debugging

## Debugging

### Debug Mode
```bash
npx playwright test --debug
```

### Trace Viewer
```bash
npx playwright show-trace trace.zip
```

### Console Logging
```javascript
page.on('console', msg => console.log(msg.text()));
```

## Performance Testing

### Metrics
- First Contentful Paint (FCP)
- Largest Contentful Paint (LCP)
- Time to Interactive (TTI)

### Custom Metrics
```javascript
const metrics = await page.evaluate(() => {
  const perf = performance.getEntriesByType('paint');
  return { paint: perf };
});
```
