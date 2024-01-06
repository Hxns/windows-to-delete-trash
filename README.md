# Freeing Up Space on Windows

This repository provides instructions and useful commands to free up disk space on Windows operating systems. Follow the steps below to optimize storage on your machine.

## Steps

### 1. Delete Temporary Files

Press `Win + R` to open the Run window and type `%temp%`. This will open the temporary files folder. Delete all files and folders present in this location.

### 2. Clean the Prefetch Folder

1. Again, open the Run window with `Win + R`.
2. Enter `C:\Windows\Prefetch` and press Enter.
3. Delete all files present in this folder.

### 3. Use Event Viewer

1. Open Event Viewer by typing `eventvwr` in the Run window.
2. Navigate to `Windows Logs -> System`.
3. Look for events with Event ID `517` (disk cleanup) and check for any events related to disk cleanup.
4. If you find disk cleanup events, you can be assured that periodic cleanups are taking place.

## Notes

- Perform these steps with caution to avoid deleting important files. Make sure to review files before deletion.
- Cleaning temporary files and the Prefetch folder is generally safe, but be aware that some programs may store important files in these locations.
