# Next.js 15 Navigation Issue

This repository demonstrates a navigation problem in a Next.js 15 application.

## Problem Description

The application consists of three pages: Home, About, and Contact. Navigation from Home to About works correctly using `next/link`. However, navigation from About to Contact using `next/router` does not work as expected.  The Contact page does not render.

## Reproduction Steps

1. Clone this repository.
2. Run `npm install` to install the necessary dependencies.
3. Run `npm run dev` to start the development server.
4. Navigate to the About page.
5. Click the "Go to Contact Page" button. The Contact page should appear, but it doesn't.

## Solution

The issue was due to a missing export in the Contact page component.  The solution includes the correct export to allow Next.js to properly route to the Contact page.
