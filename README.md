# Atlan-frontend-SQL-App

## Overview

This project introduces a user-friendly web app designed for executing and managing SQL queries. It caters to data analysts, providing a seamless interface to run queries, view results, and save frequently used queries. The tab-based layout facilitates easy query organization and management.

## Key Features

1. **Tab Interface:** Organizes queries with a user-friendly tab system.
2. **Query Editor:** Employs a feature-rich SQL editor with syntax highlighting and a "Reset Code" button.
3. **Fullscreen Mode:** Offers distraction-free query editing with a fullscreen option.
4. **Query Execution:** Allows running queries and viewing results, with demo queries for exploration.
5. **Split View:** Enhances user experience with adjustable editor and results panels.
6. **Table Schema:** Displays table schema for quick understanding of data structure.
7. **Saved Queries:** Enables saving queries for future use, including demo queries.
8. **Local Storage Integration:** Persists saved queries across sessions using local storage.
9. **Dark Mode Support:** Enhances readability with a dark mode toggle.
10. **Export to CSV:** Allows exporting query results data to a CSV file.
11. **Error Handling:** Provides informative error messages and alerts for better user feedback.

## Technology Stack

- React
- Zustand (State Management)
- react-codemirror (Code Editor)
- PapaParse (CSV Parsing)
- lodash.throttle and lodash.debounce (Function optimization)
- Tailwind CSS (Styling)
- react-split (Split layout component)

## Page Load Time Measurement

[Lighthouse Report](link-to-lighthouse-report-image)

## Optimizations for Performance

1. **Zustand State Management:**
   Zustand is chosen over Context API to prevent unnecessary rerenders. It uses shallow comparison, rendering only components dependent on updated state, improving performance and efficiency.

2. **Pagination for Query Results:**
   Implemented pagination for query results, displaying a limited number of rows at a time. Enhances page load and rendering performance by avoiding rendering a large number of rows at once.

3. **Debounced and Throttled Function Calls:**
   Utilized debouncing for actions like data export, preventing repeated calls within a specified time. Throttling is applied, for example, when adding tabs, ensuring a smoother user experience by limiting excessive tab creations.

4. **Memoization and useCallback Hooks:**
   Memoization caches expensive calculations, avoiding redundant computations. useCallback memoizes callback functions, preventing unnecessary re-renders of child components by returning the same function instance on subsequent renders.

5. **Local State Variables:**
   Local state variables within components minimize rerenders, optimizing rendering performance. Only affected components are updated when state changes, reducing the scope of changes that trigger rerenders.

## Usage

1. Clone the repository: `git clone https://github.com/your-username/your-repository.git`
2. Install dependencies: `npm install`
3. Run the app: `npm start`

## Contributing

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/new-feature`
3. Commit your changes: `git commit -m "Add new feature"`
4. Push to the branch: `git push origin feature/new-feature`
5. Open a pull request.



