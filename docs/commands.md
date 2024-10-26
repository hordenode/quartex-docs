# Quartex Command Documentation

This documentation provides an overview of the available `quartex` commands that can be used within the Electron application. Each command has a specific purpose related to window management and functionality.

## 1. `quartex.top()`

### Description
Sets the application window to be always on top of other windows.

### Usage
```javascript
quartex.top();
```

### Functionality
- Makes the current window stay above all other application windows.
- Useful for keeping the application visible while using other applications.

---

## 2. `quartex.minimize()`

### Description
Minimizes the application window.

### Usage
```javascript
quartex.minimize();
```

### Functionality
- Reduces the application window to the taskbar or dock.
- Helps in clearing the screen while keeping the application running in the background.

---

### Functionality
- Ensures that the application window is active and ready to receive input.
- Can be used when switching between multiple applications.

## 3. `quartex.togglefullscreen()`

### Description
Toggles the application window between full screen and windowed mode.

### Usage
```javascript
quartex.togglefullscreen();
```

### Functionality
- Switches the application to full screen if currently windowed, and vice versa.
- Enhances the user experience for applications that benefit from immersive displays.

## 4. `quartex.setwindowopacity({ value })`

### Description
Sets the opacity of the application window.

### Usage
```javascript
quartex.setwindowopacity({ value: 0.5 }); // Set opacity to 50%
```

### Parameters
- **value** (number): A decimal number between 0 (completely transparent) and 1 (completely opaque).

### Functionality
- Adjusts the visibility of the window. For example, a value of `0.5` will make the window 50% transparent.
- Useful for creating overlays or ensuring that the window blends with background content.

---

## Example Usage
Here is an example demonstrating how to utilize these commands in a script:

```javascript
function executeCommands() {
  quartex.top();
  quartex.minimize();
  quartex.togglefullscreen();
  quartex.setwindowopacity({ value: 0.75 });
}
```
