# Expo CLI Android Environment Setup Error

This repository demonstrates a common error encountered when setting up the Android environment for Expo CLI and provides a solution.

## Problem
The Expo CLI may fail to build Android projects due to issues with the Android SDK, build tools, or environment variables. This often manifests as vague error messages that don't directly pinpoint the problem.

## Solution
The solution involves verifying and configuring the Android SDK and environment variables correctly.

1. **Install Necessary Android SDK Components:** Ensure you have the necessary Android SDK platforms and build tools installed.  Refer to the Expo documentation on setting up Android for precise instructions.
2. **Verify ANDROID_HOME Environment Variable:** Confirm that the `ANDROID_HOME` environment variable is correctly set to your Android SDK directory.
3. **Check JAVA_HOME:** Make sure `JAVA_HOME` points to a valid JDK installation (not just JRE).
4. **Restart your system** after any changes to ensure your system picks up the changes to the environment variables.
5. **Clean and rebuild:** If still failing run `expo prebuild` and `expo run:android` again. 

## Reproducing the Error
The `bug.js` file shows a simplified scenario where missing SDK components can lead to the error.  This is not an actual expo application and is only to help the user grasp the potential causes for the error.

## Fixing the Error
The `bugSolution.js` file demonstrates how to properly set up the Android development environment.