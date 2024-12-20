# Expo Android Build Failure: Vague Resource Merging Error

This repository demonstrates a common, yet frustrating, issue when building Android APKs with the Expo CLI. The build process fails with an ambiguous error message related to resource merging, making it challenging to identify the root cause.

## Problem

The primary problem is the lack of specificity in the error message.  While the error message indicates a resource merging problem, it often doesn't directly point to the offending resource or configuration issue.  This makes debugging time-consuming.

## Solution

The solution involves a systematic approach to identify the problematic resource.  This includes:

1. **Cleaning the project:** This removes any cached build artifacts that might be causing the issue.
2. **Checking for invalid resource files:** Ensure all images, XML layouts, and other resources are valid and properly formatted.
3. **Reviewing resource names and IDs:** Look for any potential naming conflicts or inconsistencies.
4. **Inspecting dependencies:** Conflicts or issues with project dependencies can sometimes lead to this type of error.
5. **Gradle sync:**  A clean and fresh sync of the gradle files can also help.

This repo provides example code and steps to reproduce and resolve this issue.