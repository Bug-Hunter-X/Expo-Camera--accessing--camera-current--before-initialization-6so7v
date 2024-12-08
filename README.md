# Expo Camera: accessing 'camera.current' before initialization

This repository demonstrates a common error when working with the Expo Camera API: attempting to access `camera.current` before the component has mounted or the camera has finished initializing.  The `bug.js` file showcases the problematic code, while `bugSolution.js` provides a corrected version.

## Problem

Accessing `camera.current` prematurely results in `null` values or unexpected behavior.  The solution involves ensuring the camera is ready before attempting to use its functionalities.  The primary cause is usually improper handling of asynchronous operations.

## Solution

The corrected code uses asynchronous operations correctly and checks if `camera.current` is available before using it.  This prevents errors and provides a more robust implementation.

## How to reproduce

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install`.
4. Run `expo start`.
5. Observe the behavior of both `bug.js` and `bugSolution.js`. 