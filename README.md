# alx-graphql-0x03

## Project Description

ReactGuard: Mastering Error Handling

A comprehensive React project demonstrating best practices for error handling in modern React applications. This project showcases the implementation of Error Boundaries and error-prone components to gracefully handle runtime errors and provide a better user experience.

## Features

- **ErrorBoundary**: A reusable Error Boundary component that catches JavaScript errors anywhere in the component tree, logs those errors, and displays a fallback UI instead of crashing the entire application.

- **ErrorProneComponent**: A demonstration component that intentionally triggers errors to showcase how Error Boundaries work in practice. This component helps developers understand error propagation and handling patterns.

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/tevn23/alx-graphql-0x03.git
   cd alx-graphql-0x03
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

3. Run the development server:
   ```bash
   npm run dev
   # or
   yarn dev
   ```

4. Open your browser and navigate to `http://localhost:3000`

## Usage of _app.tsx

The `_app.tsx` file serves as the root component wrapper for the entire application. It integrates the ErrorBoundary component at the highest level to catch errors throughout the application:

```typescript
import ErrorBoundary from '../components/ErrorBoundary';

function MyApp({ Component, pageProps }) {
  return (
    <ErrorBoundary>
      <Component {...pageProps} />
    </ErrorBoundary>
  );
}

export default MyApp;
```

This ensures that any errors thrown by child components are caught and handled gracefully.

## Testing Error Handling

Follow these steps to test the error handling functionality:

1. **Start the development server**: Run `npm run dev` or `yarn dev`

2. **Navigate to the error-prone component**: Access the page containing the ErrorProneComponent

3. **Trigger an error**: Click the button or perform the action that triggers an error in the ErrorProneComponent

4. **Observe the fallback UI**: The ErrorBoundary should catch the error and display a user-friendly error message instead of crashing the application

5. **Check the console**: Open browser DevTools to see detailed error logs and stack traces

6. **Test error recovery**: Use the "Try again" or reset functionality to recover from the error state

7. **Test different error scenarios**: Experiment with various error types (runtime errors, promise rejections, etc.) to ensure comprehensive error handling

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.
