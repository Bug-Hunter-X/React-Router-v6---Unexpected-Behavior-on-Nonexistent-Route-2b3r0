# React Router v6 - Unexpected Behavior on Nonexistent Route

This repository demonstrates a common issue encountered when using React Router v6: unexpected behavior when navigating to a route that does not exist.  The application may crash or display a blank screen instead of gracefully handling the 404 scenario.

## Problem

The provided `App.js` uses `Routes` and `Route` components to define routes.  However, navigating to a path not defined in the `Routes` results in an error, breaking the app.

## Solution

The solution involves adding a `Route` component with a `path="*"` (catch-all route) to handle any unmatched paths. This allows you to create a custom 404 page that gracefully handles non-existent routes.  The `bugSolution.js` file demonstrates this fix.