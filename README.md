# React Router v6 Catch-all Route Issue

This repository demonstrates a common issue encountered when using catch-all routes ('*') in React Router v6.  The catch-all route, intended to handle invalid routes, is not working correctly.

## Problem

The provided code uses React Router v6 to define routes.  A catch-all route is added to handle any invalid route. However, it does not display when an invalid URL is entered.

## Solution

The solution involves ensuring that the catch-all route is placed last in the `Routes` component.  This guarantees that it's only triggered if no other route matches.  Also, it's crucial to use the `Routes` component instead of `Switch`, as `Switch` is deprecated in React Router v6.