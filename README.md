# React Router DOM: Inconsistent Route Rendering or Errors on Nonexistent Paths

This repository demonstrates an uncommon bug in React Router DOM v6 related to how it handles navigation to routes that don't exist.  The issue manifests inconsistently, sometimes causing unexpected rendering behavior and other times throwing errors.  The provided solution addresses this by implementing a catch-all route and a custom error component.

## Bug Description
The bug is characterized by the inconsistent behavior of the React Router when navigating to a nonexistent route. It may not always throw an error, and sometimes, parts of the application may render incorrectly or fail to update the UI as expected. 

## Solution
The solution involves adding a catch-all route (`/*`) to the `Routes` component and creating a custom `Error` component to handle navigation errors gracefully.  The catch-all route will be the last route declared and will redirect to an error page.