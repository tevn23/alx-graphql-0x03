# ALX Rick and Morty App

## Project Overview

This is a React-based web application that leverages the Rick and Morty API using GraphQL. The app provides an interactive interface to explore characters, episodes, and locations from the Rick and Morty universe.

## Main Features

- **ErrorBoundary**: A robust error handling component that catches JavaScript errors anywhere in the component tree, logs them, and displays a fallback UI instead of crashing the entire application.

- **ErrorProneComponent**: A demonstration component used for testing error boundary functionality and handling edge cases.

- **GraphQL Integration**: Efficient data fetching using GraphQL queries to interact with the Rick and Morty API.

- **Responsive Design**: Mobile-friendly interface that works seamlessly across different device sizes.

- **Component-Based Architecture**: Modular structure with reusable React components for maintainability and scalability.

## Usage

1. Browse through the application to discover characters, episodes, and locations from Rick and Morty
2. Use the search and filter features to find specific content
3. Click on items to view detailed information
4. The ErrorBoundary component will gracefully handle any runtime errors that occur

## Quick Setup

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn package manager

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/tevn23/alx-graphql-0x03.git
   cd alx-graphql-0x03/alx-rick-and-morty-app
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

### Build for Production

```bash
npm run build
# or
yarn build
```

## Project Structure

- `/components` - Reusable React components including ErrorBoundary and ErrorProneComponent
- `/pages` - Application pages and routing logic

## Technologies Used

- React
- GraphQL
- Rick and Morty API
- Next.js (or your framework of choice)

## Contributing

Feel free to submit issues and enhancement requests!

## License

This project is part of the ALX GraphQL learning curriculum.
