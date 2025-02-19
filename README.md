# Next.js Infinite Redirect Loop Bug

This repository demonstrates a common bug in Next.js applications: infinite redirect loops caused by attempting to navigate to a route that does not exist.  The `router.push()` method, when given an invalid route, can lead to unexpected behavior.

## Bug
The `bug.js` file contains a component that uses the `useRouter` hook to navigate to a nonexistent route. Clicking the button will trigger an infinite redirect loop in the browser.

## Solution
The `bugSolution.js` file provides a corrected version. It incorporates error handling and prevents the redirect if the route is invalid. The solution shows a fallback to prevent the infinite loop.