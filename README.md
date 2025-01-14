# React Router Dom Nested Routes Issue
This repository demonstrates a common issue encountered when working with nested routes in React Router Dom v6.  The problem involves a nested route failing to render when navigating directly to it via a URL with parameters.

The issue arises because the parent route ('/contact') matches the initial path, and the nested route is only accessed if you navigate through the parent route first.

## Bug Description:
The ContactDetails component, intended to display contact details when navigating to a specific contact using a URL like '/contact/1', does not render correctly.

## Solution:
The solution uses the `useParams` hook and modifies the route structure to resolve the issue.  See `bugSolution.js` for the corrected code.